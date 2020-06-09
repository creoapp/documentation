**super**: **[UIViewController](UIViewController.md)** (on iOS)

A Window object provides the backdrop for your app's user interface and provides important event-handling behaviors. It is responsible for loading and disposing of contained views, for managing interactions with those views, and for coordinating responses with any appropriate data objects. Windows also coordinate their efforts with other controller objects—including other windows and help manage your app's overall interface.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
Use this event to be notified when window is about to be added to a view hierarchy.

* **DidShow**()
Use this event to be notified when window was added to a view hierarchy.

* **DidShake**()
Use this event to be notified when a shake event occurred.

* **KeyboardWillShow**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately prior to the display of the keyboard.

* **KeyboardDidShow**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately after the display of the keyboard.

* **KeyboardWillHide**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately prior to the dismissal of the keyboard.

* **KeyboardDidHide**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately after the dismissal of the keyboard.

* **WillRotate**(**toOrientation**: **[Int](../gravity/int.md)**, **duration**: **[Float](../gravity/float.md)**)
Posted immediately prior to rotation of the interface.

* **DidRotate**(**fromOrientation**: **[Int](../gravity/int.md)**)
Posted immediately after the rotation of the interface.

* **WillHide**()
Use this event to be notified when navigation is about to be removed from a view hierarchy.

* **DidHide**()
Use this event to be notified when navigation was removed from a view hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **bounds**: **[Rect](Rect.md)**
The bounds rectangle, which describes the view’s location and size in its own coordinate system.

* **var** **view**: **[UIView](UIView.md)**
The root view hierarchy.

* **var** **frame**: **[Rect](Rect.md)**
The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

* **var** **transitionStyle**: **<a href="#_enum_TransitionStyle">TransitionStyle</a>**
The style used to transition between windows.

* **var** **statusBarVisibility**: **<a href="#_enum_StatusBarVisibility">StatusBarVisibility</a>**
A value indicating whether the status bar should be visible.

* **var** **statusBarStyle**: **<a href="#_enum_StatusBarStyle">StatusBarStyle</a>**
The style of the status bar.

* **var** **firstResponder**: **[UIView](UIView.md)**
Returns the subview that is now the first-responder, null if none. \(read-only\)

* **var** **subviews**: **[List](../gravity/list.md)**
The array of subviews. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **open**(**completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion ()" data-content="The completion closure, if set, is executed when the open action completes. The self value points to the container being opened, so you can safely perform setup operation in this context.">Closure</a> = null**)
Open window in currently displayed window or navigation using the destination object default behaviour.

* **func** **close**(**animated**: **[Bool](../gravity/bool.md) = true**)
Close window (and remove from current navigation if any).

* **func** **openIn**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion ()" data-content="The completion closure, if set, is executed when the open action completes. The self value points to the container being opened, so you can safely perform setup operation in this context.">Closure</a> = null**)
<pre><code class="swift">TargetWindow.openIn(ContainerWindow);</code></pre>
Open callee object (TargetWindow) inside parameter object (ContainerWindow) using its default behaviour. Note that TargetWindow and/or ContainerWindow can be a Window or a Navigation.

* **func** **openModal**(**TransitionStyle**: **<a href="#_enum_TransitionStyle">TransitionStyle</a> = 0**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion ()" data-content="The completion closure, if set, is executed when the open action completes. The self value points to the container being opened, so you can safely perform setup operation in this context.">Closure</a> = null**)
Open window modally usign the specified transition style.

* **func** **moveToNextField**()
Move the focus to the next field.

* **func** **convertFrom**(**rect**: **[Rect](Rect.md)**, **view**: **[UIView](UIView.md)**)<strong>: [Rect](Rect.md)</strong> 
Converts a rectangle from the coordinate system of another view to that of the Window.

* **func** **convertTo**(**rect**: **[Rect](Rect.md)**, **view**: **[UIView](UIView.md)**)<strong>: [Rect](Rect.md)</strong> 
Converts a rectangle from the Window’s coordinate system to that of another view.

* **func** **reset**(**forceGarbageCollector**: **[Bool](../gravity/bool.md) = true**)
Free the content of the Window, you can call this method on unused Windows to save memory. If the Window is used after calling the reset method, the content is reloaded just before presenting (before the execution of the WillShow event.

* **func** **addSubview**(**view**: **[UIView](UIView.md)**)
Adds a view to the end of the list of subviews.

* **func** **insertSubview**(**view**: **[UIView](UIView.md)**, **index**: **[Int](../gravity/int.md)**)
Inserts a subview at the specified index.





### Enums

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



