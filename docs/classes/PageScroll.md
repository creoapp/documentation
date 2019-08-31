**super**: **[UIPageViewController](UIPageViewController.md)** (on iOS)

A page scroll view controller lets the user navigate between pages of content, where each page is managed by its own <a href="Window.html">Window</a> object. Navigation can be controlled programmatically by your app or directly by the user using gestures. When navigating from page to page, it displays a page-scrolling animation.

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

* **var** **windows**: **[List](../gravity/list.md)**
Array of windows currently managed by the PageScroll.

* **var** **selectedWindow**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**
Represents the current Window in the PageScroll.

* **var** **selectedIndex**: **[Int](../gravity/int.md)**
Represents the current window index inside the PageScroll.

* **var** **pageControlBackgroundColor**: **[Color](Color.md)**
Description not yet ready.

* **var** **pageControlOnColor**: **[Color](Color.md)**
Description not yet ready.

* **var** **pageControlOffColor**: **[Color](Color.md)**
Description not yet ready.

* **var** **pageControlIndicatorDiameter**: **[Float](../gravity/float.md)**
Description not yet ready.

* **var** **pageControlIndicatorSpace**: **[Float](../gravity/float.md)**
Description not yet ready.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **open**(**completion**: **[Closure](../gravity/closure.md) = null**)
Open window in currently displayed window or navigation using the destination object default behaviour .

* **func** **openIn**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **completion**: **[Closure](../gravity/closure.md) = null**)
<pre><code class="swift">TargetWindow.openIn(ContainerWindow);</code></pre>
Open callee object (TargetWindow) inside parameter object (ContainerWindow) using its default behaviour. Note that TargetWindow and/or ContainerWindow can be a Window or a Navigation.

* **func** **openWindow**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **completion**: **[Closure](../gravity/closure.md) = null**)
Add the Window to the PageScroll and set it as the selected Window.

* **func** **selectWindow**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **animated**: **[Bool](../gravity/bool.md) = true**, **completion**: **[Closure](../gravity/closure.md) = null**)
Set the Window as the new selected Window, optionally animating the scroll motion.

* **func** **selectIndex**(**index**: **[Int](../gravity/int.md)**, **animated**: **[Bool](../gravity/bool.md) = true**, **completion**: **[Closure](../gravity/closure.md) = null**)
Set the Window at the specified index as the new selected Window, optionally animating the scroll motion.

* **func** **openModal**(**TransitionStyle**: **<a href="#_enum_TransitionStyle">TransitionStyle</a>**, **completion**: **[Closure](../gravity/closure.md) = null**)
Open window modally usign the specified transition style.

* **func** **close**()
Close window if modally opened.





### Enums

<div id="_enum_StatusBarVisibility"></div>

#### StatusBarVisibility
 * .Default
 * .Hidden
 * .Visible

<div id="_enum_StatusBarStyle"></div>

#### StatusBarStyle
 * .DarkContent
 * .Default
 * .LightContent

<div id="_enum_TransitionStyle"></div>

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



