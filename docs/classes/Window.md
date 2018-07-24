**super**: [UIViewController](UIViewController.md) on iOS

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

* **KeyboardWillShow**(**keyboard**: <strong>[Map](../gravity/maps.md)</strong>)
Posted immediately prior to the display of the keyboard.

* **KeyboardDidShow**(**keyboard**: <strong>[Map](../gravity/maps.md)</strong>)
Posted immediately after the display of the keyboard.

* **KeyboardWillHide**(**keyboard**: <strong>[Map](../gravity/maps.md)</strong>)
Posted immediately prior to the dismissal of the keyboard.

* **KeyboardDidHide**(**keyboard**: <strong>[Map](../gravity/maps.md)</strong>)
Posted immediately after the dismissal of the keyboard.

* **WillHide**()
Use this event to be notified when navigation is about to be removed from a view hierarchy.

* **DidHide**()
Use this event to be notified when navigation was removed from a view hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **bounds**: **[Rect](rect.md)**
The bounds rectangle, which describes the view’s location and size in its own coordinate system.

* **var** **frame**: **[Rect](rect.md)**
The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

* **var** **transitionStyle**: **TransitionStyle**
The style used to transition between windows.

* **var** **statusBarVisibility**: **StatusBarVisibility**
A value indicating whether the status bar should be visible.

* **var** **statusBarStyle**: **StatusBarStyle**
The style of the status bar.

* **var** **firstResponder**: **[UIView](UIView.md)**
Returns the subview that is now the first-responder, null if none. \(read-only\)



### Methods

* **func** **open**(**completion**: <strong>[Closure](../gravity/closures.md) = null</strong>)
Open window in currently displayed window or navigation using the destination object default behaviour.

* **func** **close**()
Close window (and remove from current navigation if any).

* **func** **openIn**(**window**: <strong>[Window](window.md) or [Navigation](navigation.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md) = null</strong>)
<pre><code class="swift">TargetWindow.openIn(ContainerWindow);</code></pre>
Open callee object (TargetWindow) inside parameter object (ContainerWindow) using its default behaviour. Note that TargetWindow and/or ContainerWindow can be a Window or a Navigation.

* **func** **openModal**(**TransitionStyle**: <strong><a href="#_enum_TransitionStyle">TransitionStyle</a></strong>, **completion**: <strong>[Closure](../gravity/closures.md) = null</strong>)
Open window modally usign the specified transition style.

* **func** **moveToNextField**()
Move the focus to the next field.

* **func** **convertFrom**(**rect**: <strong>[Rect](rect.md)</strong>, **view**: <strong>[UIView](UIView.md)</strong>): <strong>[Rect](rect.md)</strong> 
Converts a rectangle from the coordinate system of another view to that of the Window.

* **func** **convertTo**(**rect**: <strong>[Rect](rect.md)</strong>, **view**: <strong>[UIView](UIView.md)</strong>): <strong>[Rect](rect.md)</strong> 
Converts a rectangle from the Window’s coordinate system to that of another view.





### Enumeration

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

<br><br>#### StatusBarVisibility
 * .Default
 * .Hidden
 * .Visible

<br><br>#### StatusBarStyle
 * .DarkContent
 * .Default
 * .LightContent

<br><br>

