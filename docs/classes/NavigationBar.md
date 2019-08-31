**super**: **[UINavigationController](UINavigationController.md)** (on iOS)

The NavigationBar class implements a specialized view controller that manages the navigation of hierarchical content. This navigation interface makes it possible to present your data efficiently and makes it easier for the user to navigate that content. You generally use this class as-is but you may also subclass to customize the class behavior.

The screens presented by a navigation interface typically mimic the hierarchical organization of your data. At each level of the hierarchy, you provide an appropriate Window to display the content at that level.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
Use this event to be notified when navigation is about to be added to a view hierarchy.

* **DidShow**()
Use this event to be notified when navigation was added to a view hierarchy.

* **WillHide**()
Use this event to be notified when navigation is about to be removed from a view hierarchy.

* **DidHide**()
Use this event to be notified when navigation was removed from a view hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **bounds**: **[Rect](Rect.md)**
The bounds rectangle, which describes the view’s location and size in its own coordinate system.

* **var** **frame**: **[Rect](Rect.md)**
The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

* **var** **statusBarVisibility**: **StatusBarVisibility**
A value indicating whether the status bar should be visible.

* **var** **statusBarStyle**: **StatusBarStyle**
The style of the status bar.

* **var** **topWindow**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**
Returns Window/Navigation positioned on top of the receiver’s stack. \(read-only\)

* **var** **windows**: **[List](../gravity/list.md)**
Array of windows currently managed by the NavigationBar.

* **var** **navigationBarHidden**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the navigation bar is hidden.

* **var** **navigationBarTranslucent**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the navigation bar is translucent (true) or not (false).

* **var** **navigationBarTintColor**: **[Color](Color.md)**
The tint color to apply to the navigation bar background.

* **var** **selectedWindow**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**
Returns the currently selected Window or Navigation. \(read-only\)

* **var** **prefersLargeTitles**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the title should be displayed in a large format in the navigation bar. When this property is set to true, the navigation bar allows the title to be displayed out-of-line and using a larger font. The top window must specify whether it wants its title displayed in the large or small format. Use the largeTitleDisplayMode property of the <a href="Window.html">Window</a> to configure the title's appearance. When the property is set to false, the navigation bar displays the title inline with the other bar button items.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **open**(**completion**: **[Closure](../gravity/closure.md) = null**)
Open window in currently displayed window or navigation using the destination object default behaviour .

* **func** **openIn**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **completion**: **[Closure](../gravity/closure.md) = null**)
Open callee object (TargetWindow) inside parameter object (ContainerWindow) using its default behaviour. Note that TargetWindow and/or ContainerWindow can be a Window or a Navigation. Example: <code class="swift">TargetWindow.openIn(ContainerWindow);</code>

* **func** **openWindow**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **animated**: **[Bool](../gravity/bool.md) = true**, **completion**: **[Closure](../gravity/closure.md) = null**)
Pushes a Window/Navigation onto the receiver’s stack and updates the display.

* **func** **openModal**(**TransitionStyle**: **<a href="#_enum_TransitionStyle">TransitionStyle</a>**, **completion**: **[Closure](../gravity/closure.md) = null**)
Open window modally usign the specified transition style.

* **func** **close**()
Close window if modally opened.

* **func** **pop**(**animated**: **[Bool](../gravity/bool.md) = true**)
Pops the top Windows/Navigations from the navigation stack and updates the display.

* **func** **popToWindow**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Pops Windows/Navigations until the specified Window is at the top of the navigation stack.

* **func** **popToRootWindow**(**animated**: **[Bool](../gravity/bool.md) = true**)
Pops all the Windows/Navigations on the stack except the root Window/Navigation and updates the display.

* **func** **setNavigationBarHidden**(**hidden**: **[Bool](../gravity/bool.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Sets whether the navigation bar is hidden.



* None

### Enumeration

<div name="_enum_StatusBarVisibility"></div>
#### StatusBarVisibility
 * .Default
 * .Hidden
 * .Visible

<div name="_enum_StatusBarStyle"></div>
#### StatusBarStyle
 * .DarkContent
 * .Default
 * .LightContent

<div name="_enum_TransitionStyle"></div>
#### TransitionStyle
 * .Cards
 * .CoverVertical
 * .CrossDissolve
 * .Crossfade
 * .Cube
 * .Default
 * .Explode
 * .Flip
 * .FlipHorizontal
 * .Fold
 * .NatGeo
 * .NotAnimated
 * .PartialCurl
 * .Portal
 * .Turn



