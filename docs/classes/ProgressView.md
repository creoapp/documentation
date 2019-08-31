**super**: **[UIProgressView](UIProgressView.md)** (on iOS)

You use the ProgressView class to depict the progress of a task over time. An example of a progress bar is the one shown at the bottom of the Mail application when it’s downloading messages. The ProgressView class provides properties for managing the style of the progress bar and for getting and setting values that are pinned to the progress of a task. For an indeterminate progress indicator—or, informally, a “spinner”—use an instance of the <a href="ActivityIndicator.html">ActivityIndicator</a> class.

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

* **var** **progressViewStyle**: **<a href="#_enum_ProgressViewStyle">ProgressViewStyle</a>**
The current graphical style of the receiver.

* **var** **value**: **[Float](../gravity/float.md)**
The current progress shown by the receiver. The current progress is represented by a floating-point value between 0.0 and 1.0, inclusive, where 1.0 indicates the completion of the task. The default value is 0.0. Values less than 0.0 and greater than 1.0 are pinned to those limits.

* **var** **progressTintColor**: **[Color](Color.md)**
The color shown for the portion of the progress bar that is filled.

* **var** **trackTintColor**: **[Color](Color.md)**
The color shown for the portion of the progress bar that is not filled.

* **var** **progressImage**: **[Image](Image.md)**
An image to use for the portion of the progress bar that is filled.

* **var** **trackImage**: **[Image](Image.md)**
An image to use for the portion of the track that is not filled.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **setProgress**(**progress**: **[Float](../gravity/float.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Adjusts the current progress shown by the receiver, optionally animating the change.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_ProgressViewStyle"></div>

#### ProgressViewStyle
 * .Bar
 * .Default

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



