**super**: **[UIResponder](UIResponder.md)** (on iOS)

This class is reserved and cannot be directly instantiated.



### Events

* None

### Properties

* **var** **supportedInterfaceOrientations**: **InterfaceOrientationMask**
Returns all of the interface orientations that the Window supports.

* **var** **title**: **[String](../gravity/types.md)**
A String that provides the current title of the window or navigation.

* **var** **interfaceOrientation**: **InterfaceOrientation**
Convenience property that provides the current orientation of the interface. \(read-only\)

* **var** **editing**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the view currently allows the user to edit the contents.

* **var** **automaticallyAdjustsScrollViewInsets**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether the view should automatically adjust its scroll view insets.

* **var** **objectName**: **[String](../gravity/types.md)**
The name of the object.



### Methods

* **func** **isViewLoaded**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether the view is currently loaded into memory, it does not attempt to load the view if it is not already in memory.

* **func** **updateStatusBar**()
Indicates to the system that the status bar attributes have changed.





### Enumeration

#### InterfaceOrientationMask
 * .All
 * .AllButUpsideDown
 * .Landscape
 * .LandscapeLeft
 * .LandscapeRight
 * .Portrait
 * .PortraitUpsideDown

#### InterfaceOrientation
 * .LandscapeLeft
 * .LandscapeRight
 * .Portrait
 * .PortraitUpsideDown



