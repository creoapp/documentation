A `Window` present and manage a hierarchy of views and controls. Each `Window` owns a portion of your app’s user interface. For example, one Window might display a table of items while a different `Window` displays the selected item from that table. Usually, only the views from one `Window` are visible at a time. A `Window` can be presented by another window as a modal window or inside a window container.

![A simple Window inside a Navigation](images/Window1.png)
A simple `Window` inside a `Navigation`.

### How to use

### Create a new Window

### Open a Window

Windows can be accessed in Gravity through a variable with the name of the `Window` which is unique in the project. These `Window` variables are globally defined and are created during the launching of the App so a `Window` instance can be used anywhere and anytime from Gravity code.
For example, if your project has two Windows, named `Window1` and `Window2`, you can use the following code to open the `Window2` from the code of an event (for example the `Action` event of a `Button`) inside `Window1`:

```
Window2.open()
```

#### Window's content

The `Window` instance is created during the loading of the App and its properties are immediately configured with the  values specified through its inspectors. All its properties and methods can be used anytime inside the App.

The content of a `Window` - the subnodes inside the `Window`'s hierarchy - are divided in two groups that are loaded at different times:
1. TabBar items and Navigation Bar items are immediately loaded after the creation of the `Window` instance because the container (`TabBar` or `Navigation`) needs to use these objects before presenting the visible content of the `Window`.
2. The other objects configured inside the `Window`'s hierarchy (controls, views, databases, sensors, gestures, network objects, etc.) are loaded when the `Window` is about to be presented for the first time.

The TabBar items and Navigation Bar items can be added to a `Window` by pressing the '+' button near the window's name in the project's layout:

![How to add TabBar items and Navigation Bar items](images/Window2.png)
How to add TabBar items and Navigation Bar items

Controls, views and other non-UI objects can be added by dragging the desired object class from the Objects collection in the bottom-right section of the Creo interface.

If you want to open a `Window` and get/set a property of an object of the second group, you have to be sure that `Window` has been presented at least once before accessing that object. You can achieve this by writing the code in the `WillShow` event of the `Window` or in the completion [closure]({{github_raw_link}}/gravity/closure.html) of the `open` method. The following example shows how to reliably set the `text` of a `Label` in `Window2`:

```
func completion() {
	Window2.Label1.text = "New Text"
}

Window2.open(completion)
```

The `open` method returns immediately - it doesn't wait the presentation of the `Window` to complete - so it is not safe to write any code that uses subnodes of the opening `Window` below the `open(completion)` if the `Window2` has not yet been presented before.

The following sequence of steps is performed during the presentation of a `Window`:
1. if the Window's content has not yet been loaded (the first time that the `Window` is presented) all its subnodes are created and added to the `Window`'s hierarchy if needed.
2. the `WillShow` event of the `Window` is called.
3. if a completion closure has been set as a parameter of the open method, it is executed.
4. the `Window` is added to a view hierarchy and the presenting animation is performed.
5. when the presenting animation ends the `DidShow` event of the `Window` is called.

For the complete list of the open methods, please refer to the documentation of the [Window]({{github_raw_link}}/classes/Window.md) class and to the documentation of the window containers.

### References

#### Classes
- [Window]({{github_raw_link}}/classes/Window.md)
- [Navigation](./Navigation.md) | [Navigation class]({{github_raw_link}}/classes/Navigation.md)
- [TabBar class]({{github_raw_link}}/classes/Window.md)
- [PageScroll class]({{github_raw_link}}/classes/PageScroll.md)
- [PageCurl class]({{github_raw_link}}/classes/PageCurl.md)
- [PageSplit class]({{github_raw_link}}/classes/PageSplit.md)

#### Tutorials
- [ToDo]({{github_raw_link}}/tutorials/todo.html)
- [Lets Cook Navigation]({{github_raw_link}}/tutorials/lets-cook-nav.html)

#### Apple
- [UIViewController](https://developer.apple.com/documentation/uikit/uiviewcontroller)
- [Human Interface Guidelines - App Architecture](https://developer.apple.com/design/human-interface-guidelines/ios/app-architecture/navigation/)
- [View Controller Catalog](https://developer.apple.com/library/archive/documentation/WindowsViews/Conceptual/ViewControllerCatalog/Introduction.html#//apple_ref/doc/uid/TP40011313-CH1-SW1)
