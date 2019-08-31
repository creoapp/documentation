**super**: **[UIActivityIndicatorView](UIActivityIndicatorView.md)** (on iOS)

Use an activity indicator to show that a task is in progress. An activity indicator appears as a "gear" that is either spinning or stopped.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **color**: **[Color](Color.md)**
The color of the activity indicator.

* **var** **style**: **<a href="#_enum_ActivityIndicatorStyle">ActivityIndicatorStyle</a>**
The basic appearance of the activity indicator.

* **var** **hidesWhenStopped**: **[Bool](../gravity/bool.md)**
A Boolean value that controls whether the receiver is hidden when the animation is stopped.

* **var** **initiallyStarted**: **[Bool](../gravity/bool.md)**
A Boolean value that controls whether the ActivityIndicator should start in running state or not.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **startAnimating**()
Starts the animation of the activity indicator.

* **func** **stopAnimating**()
Stops the animation of the activity indicator.

* **func** **isAnimating**()<strong>: [Bool](../gravity/bool.md)</strong> 
Returns true if the animation is active, false if it isn't.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_ActivityIndicatorStyle"></div>

#### ActivityIndicatorStyle
 * .Gray
 * .White
 * .WhiteLarge

<div id="_enum_AnimationOption"></div>

#### AnimationOption
 * .AllowAnimatedContent
 * .AllowUserInteraction
 * .Autoreverse
 * .BeginFromCurrentState
 * .CurveEaseIn
 * .CurveEaseInOut
 * .CurveEaseOut
 * .CurveLinear
 * .LayoutSubviews
 * .OverrideInheritedCurve
 * .OverrideInheritedDuration
 * .OverrideInheritedOptions
 * .Repeat
 * .ShowHideTransitionViews
 * .TransitionCrossDissolve
 * .TransitionCurlDown
 * .TransitionCurlUp
 * .TransitionFlipFromBottom
 * .TransitionFlipFromLeft
 * .TransitionFlipFromRight
 * .TransitionFlipFromTop
 * .TransitionNone



