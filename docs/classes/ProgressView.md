**super**: **[UIProgressView](UIProgressView.md)** (on iOS)

You use the ProgressView class to depict the progress of a task over time. An example of a progress bar is the one shown at the bottom of the Mail application when it’s downloading messages. The ProgressView class provides properties for managing the style of the progress bar and for getting and setting values that are pinned to the progress of a task. For an indeterminate progress indicator—or, informally, a “spinner”—use an instance of the <a href="ActivityIndicator.html">ActivityIndicator</a> class.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **progressViewStyle**: **ProgressViewStyle**
The current graphical style of the receiver.

* **var** **value**: **[Float](../gravity/types.md)**
The current progress shown by the receiver. The current progress is represented by a floating-point value between 0.0 and 1.0, inclusive, where 1.0 indicates the completion of the task. The default value is 0.0. Values less than 0.0 and greater than 1.0 are pinned to those limits.

* **var** **progressTintColor**: **[Color](color.md)**
The color shown for the portion of the progress bar that is filled.

* **var** **trackTintColor**: **[Color](color.md)**
The color shown for the portion of the progress bar that is not filled.

* **var** **progressImage**: **[Image](image.md)**
An image to use for the portion of the progress bar that is filled.

* **var** **trackImage**: **[Image](image.md)**
An image to use for the portion of the track that is not filled.



### Methods

* **func** **setProgress**(**progress**: **[Float](../gravity/types.md)**, **animated**: **[Bool](../gravity/types.md) = true**)
Adjusts the current progress shown by the receiver, optionally animating the change.

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closures.md)**, **completion**: **[Closure](../gravity/closures.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### ProgressViewStyle
 * .Bar
 * .Default

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



