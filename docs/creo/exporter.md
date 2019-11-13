Creo exporter generates a __readable__, __simple-to-mantain__ native project that can be opened and built with XCode. The exporter generates two set of class files, the private ones containing the exported views and their customisation. These files acts as a base class for the public ones that can be freely edited by the user because they are are not overwritten by future exports. **Exporting more than once is a safe operation if you don’t modify the private files.**

### Exported objects

Creo can export a __Swift__ project where that includes all views and windows. **Logic is not exported** yet, just the view hierarchies.  Logic export will be added soon.

- Views becomes native `UIKit` views (ie. `UILabel`, `UITextField` etc) and have all native properties set one by one as configured in Creo inspectors.

- Windows are exported as native view controllers inherited from `UIViewController` and eventually configured to support different orientations (*landscape*, *portrait*) and device idioms (*iPhone*, *iPad*).

- Navigation windows are exported to match their native counteparts ie `Navigation` windows become `UINavigationController` or a `TabBar` become a `UUITabBarController`. Also, all navigation windows are exported with the code to load and setup their children relationships.

- Images are exported as `xcassets` and can referenced by name or by variable via generated `UIImage` extensions.

- Favourite colors are exported as an `UIColor` extension and referenced via `UIColor.CREO`

### Supported real use scenarios

Two prominent scenarios have emerged so far during the beta phase:

- The exported code can be used to create the **starting template of a native a application** and it is expecially usefull when there are many different `Window` objects for different _orientations_ and _idioms_. Building a universal skeleton is significantly easier with Creo than with XCode. The code is easy to read and extend because whole views/windows are exported as self contained code with no external dependencies.

- View code can be easily copied from the generated project to other projects. Creo can be used to **mantain a library of pre-configured UI views** and export them ready for use with your native projects. You have a designer importing from Sketch into Creo, configuring native buttons, labels, composing complex tableview cells, and then export them as code into you project. All native properties are mantained and they compile without additional effort.

## How to export a project

To export to an `XCode` project, just open the `Creo` project and click `File` -> `Export Source Code...`

You are then askend to select a folder where the exported files are written.

An export output consists of:
- an __XCode__ project folder, ie. __Test.xcodeproj__. This is what you open using `XCode`
- as __Assets.xcassets__ folder, it contains the exported images.
- the generated `swift` files, usually one per `Window`.

### Note 1
The exporter will overwrite all generated files but other files are not overwritten or deleted.

### Note 2
`.swift` file's header __Author Name__ and __Organization Name__ can be customized from the `Preferences` -> `Exporter` panel: 

```
//
//  UIColors+CREO.swift
//  test
//
//  Exported with Creo by Spiderman on 25/09/2018.
//  Copyright © 2018 Mary Jane Watson All rights reserved.
//
```

### Examples of exported hierarchies and classes

Given a simple hierarchy:

```
Navigation1
  - Window1
    - Button1
```

Once exported the generated code contains a `NavigationController` that pushes `Window1` as the first visible controller:

```
import UIKit

class Navigation1: UINavigationController {

    override func viewDidLoad() {
        super.viewDidLoad()
        title = "Navigation1"

        let rootVC = Window1()
        pushViewController(rootVC, animated: false)

    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }

}
```

`Window1` is a native view controller configured with the child view `Button1`:

```
 class Window1: UIViewController {

    lazy var Button1: UIButton = {
        let frame = CGRect(x: 0.0, y: 119.0, width: 74.0, height: 44.0)
        let view = UIButton(type: .system)
        view.frame = frame
        view.autoresizingMask = [.flexibleRightMargin, .flexibleBottomMargin]
        view.isOpaque = false
        view.setTitle("Button", for: .normal)
        view.titleLabel?.font = UIFont.systemFont(ofSize: 15.0)
        view.titleLabel?.textColor = UIColor(red: 0.0, green: 0.0, blue: 0.0, alpha: 1.0)
        return view
    }()

    override func viewDidLoad() {
        super.viewDidLoad()
        title = "Window1"

        view.addSubview(Button1)

    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }

}
```

`Button1` properties are exported as well and the view is configured in a single place. The variable name is the same for both `Creo` and the native project; this means you can access the `Button1` variable like in __gravity__:


```
...
Window1.Button1.text = ...
...
```

The same holds true for more complex scenarios, ie

```
Window1
 - View1
   - Button1
   - Label1
   - TableView1
```

The generated Swift code makes use of the `extension` concept to avoid polluting the `Window1` class, it also use __object oriented programming__ to inherit `View1` from `UIView` to fill it with its children;. The code in this case is:

```
extension Window1 {

    class View1: UIView {

        lazy var Button1: UIButton = {
            let frame = CGRect(x: 0.0, y: 0.0, width: 74.0, height: 44.0)
            let view = UIButton(type: .system)
            view.frame = frame
            view.autoresizingMask = [.flexibleRightMargin, .flexibleBottomMargin]
            view.isOpaque = false
            view.setTitle("Button", for: .normal)
            view.titleLabel?.font = UIFont.systemFont(ofSize: 15.0)
            view.titleLabel?.textColor = UIColor(red: 0.0, green: 0.0, blue: 0.0, alpha: 1.0)
            return view
        }()

        lazy var Label1: UILabel = {
            let frame = CGRect(x: 0.0, y: 0.0, width: 100.0, height: 44.0)
            let view = UILabel(frame: frame)
            view.isOpaque = false
            view.text = "Label"
            view.font = UIFont.systemFont(ofSize: 17.0)
            return view
        }()

        lazy var TableView1: Window1.View1.TableView1 = {
            let frame = CGRect(x: 0.0, y: 0.0, width: 375.0, height: 320.0)
            let view = Window1.View1.TableView1(frame: frame)
            return view
        }()


        override init(frame: CGRect) {
            super.init(frame: frame)
            self.isOpaque = false
            addSubview(Button1)
            addSubview(Label1)
            addSubview(self.TableView1)
        }

        required init?(coder aDecoder: NSCoder) {
            fatalError("init(coder:) has not been implemented")
        }
    }

}
```

Note how the `TableView1` type name is a chain of extensions and the implementation is:

```
extension Window1.View1 {

    class TableView1: UITableView {

        override init(frame: CGRect, style: UITableViewStyle) {
            super.init(frame: frame, style: style)
            self.isOpaque = false
            self.separatorStyle = .none
            self.register(TableView1.Cell1.self, forCellReuseIdentifier: "Cell1")
        }

        required init?(coder aDecoder: NSCoder) {
            fatalError("init(coder:) has not been implemented")
        }
    }

}
```

Notice how `TableView` cells, and `CollectionView` cells, are exported and automatically registered as well:

```
    class Cell1: UITableViewCell {

        lazy var CustomView1: Window1.TableView1.Cell1.CustomView1 = {
            let frame = CGRect(x: 0.0, y: 0.0, width: 375.0, height: 44.0)
            let view = Window1.TableView1.Cell1.CustomView1(frame: frame)
            return view
        }()


        override init(style: UITableViewCellStyle, reuseIdentifier: String?) {
            super.init(style: .subtitle, reuseIdentifier: reuseIdentifier)
            self.isOpaque = false
            self.accessoryType = .disclosureIndicator
            self.editingAccessoryType = .disclosureIndicator
            self.backgroundColor = UIColor(red: 1.0, green: 1.0, blue: 1.0, alpha: 1.0)
            contentView.addSubview(self.CustomView1)
        }

        required init?(coder aDecoder: NSCoder) {
            fatalError("init(coder:) has not been implemented")
        }

        override func prepareForReuse() {
            super.prepareForReuse()
            // this is called just before the cell is returned from the table view method dequeueReusableCellWithIdentifier
        }
    }
}
```

### A note about naming convetion and supporting orientations and idimos

By default all views and windows retain the name they have in Creo, but there are case where a postfix is added to a window name to explain and declare its special meaing. This is true when a window has orientation or idiom variations.

For example, this hierarchy has a Window with 2 variations, one for iPad devices and one for iPhone devices.

```
- Window
  - iPad
    - Views ...
  - iPhone 
    - Views ...
```

The exporter create 3 classes:
1. `Window` to act as a generic container
1. `WindowiPad` is the iPad variation of `Window`
1. `WindowiPhone` is the iPhone variation of `Window`

then inside the generated code for `Window` it loads and uses the proper controller based on the interface _idioms_ informations provided at runtime by iOS.

The same happens for _orientations_:

```
- Window
  - Portrait
    - Views ...
  - Landscape
    - Views ...
```

The exporter create 3 classes:
1. `Window` to act as a generic container
1. `WindowLandscape` is the landscape variation of `Window`
1. `WindowPortrait` is the portrait variation of `Window`

then inside the generated code for `Window` it tracks the device orientation and present the proper controller.

To complete the cases, when a `Window` has both an orientation variation and an idiom variation then the postfix is the orientation first and the idiom later, ie:

`WindowLandscapeiPad`, `WindowLandscapeiPhone`, `WindowPortraitiPad`, `WindowPortraitiPhone`.

### Media

Images used to setup buttons and so on are exported into `Assets.xcassets` and therefore can be referenced by name:

```
var image = UIImage(named: "min")
```

A generated `UIImage` extension provides and handy way to access them as variables as well:

```
extension UIImage {
    struct CREOResources {
        var min: UIImage {
            return UIImage(named: "min")!
        }

        var max: UIImage {
            return UIImage(named: "max")!
        }
    }

    static var CREO = CREOResources()
}
```

For instance all generated objects that are configured using images make use of this extension automatically

```
...
view.setImage(UIImage.CREO.min, for: .normal)
...
```

### Limits

The exporter is under  development and is changing quickly.  Non-native __UIKit__ views will be exported as simple empty `UIView` until the release of __CREOFramework__

- _CREOCamera_
- _CREOMoviePlayer_
- _CREOChartView_
- _CREOCarousel_
- _CREOPageContainer_
- _Animations_

<!--
### Year 2019 Roadmap

The general roadmap is the following:

- exporting to __Swift__ code, layout and window controllers. **Done**
- improving quality of exported code
- exporting auto-layout logic
- exporting to __ObjC__ code, layout and window controllers.
- exporting to __kotlin__ (Android) code, layout and window controllers.
- exporting *animations*
- transcompiling __gravity__ code to __Swift__.
- transcompiling __gravity__ code to __kotlin__ (Android).
- exposing and exporting for __CREOFramework__; this will achieve a complete fully functional app.
-->
