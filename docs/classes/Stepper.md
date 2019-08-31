**super**: **[UIStepper](UIStepper.md)** (on iOS)

A stepper control provides a user interface for incrementing or decrementing a value. A stepper displays two buttons, one with a minus (“–”) symbol and one with a plus (“+”) symbol. If you set stepper behavior to “autorepeat” (which is the default), pressing and holding one of its buttons increments or decrements the stepper’s value repeatedly. The rate of change depends on how long the user continues pressing the control. The maximum value must be greater than or equal to the minimum value. If you set a maximum or minimum value that would make break this invariant, both values are set to the new value. For example, if the minimum value is 200 and you set a maximum value of 100, then both the minimum and maximum become 200.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **Changed**(**value**: **[Float](../gravity/float.md)**)
Use this event to be notified when value changes.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **value**: **[Float](../gravity/float.md)**
The numeric value of the stepper.

* **var** **minimumValue**: **[Float](../gravity/float.md)**
The lowest possible numeric value for the stepper.

* **var** **maximumValue**: **[Float](../gravity/float.md)**
The highest possible numeric value for the stepper.

* **var** **stepValue**: **[Float](../gravity/float.md)**
The step, or increment, value for the stepper.

* **var** **continuous**: **[Bool](../gravity/bool.md)**
The continuous vs. noncontinuous state of the stepper. If true, value change events are sent immediately when the value changes during user interaction. If false, a value change event is sent when user interaction ends. The default value for this property is true.

* **var** **autorepeat**: **[Bool](../gravity/bool.md)**
The automatic vs. nonautomatic repeat state of the stepper. If true, the user pressing and holding on the stepper repeatedly alters value. The default value for this property is true.

* **var** **wraps**: **[Bool](../gravity/bool.md)**
The wrap vs. no-wrap state of the stepper. If true, incrementing beyond maximumValue sets value to minimumValue; likewise, decrementing below minimumValue sets value to maximumValue. If false, the stepper does not increment beyond maximumValue nor does it decrement below minimumValue but rather holds at those values.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **backgroundImageForState**(**state**: **[Int](../gravity/int.md)**)-> <strong>[Image](Image.md)</strong> 
Returns the background image associated with the specified control state.

* **func** **setBackgroundImageForState**(**image**: **[Image](Image.md)**, **state**: **[Int](../gravity/int.md)**)
Sets the background image for the control when it is in the specified state.

* **func** **incrementImageForState**(**state**: **[Int](../gravity/int.md)**)-> <strong>[Image](Image.md)</strong> 
Returns the image used for the increment glyph of the control.

* **func** **setIncrementImageForState**(**image**: **[Image](Image.md)**, **state**: **[Int](../gravity/int.md)**)
Sets the image to use for the increment glyph of the control.

* **func** **decrementImageForState**(**state**: **[Int](../gravity/int.md)**)-> <strong>[Image](Image.md)</strong> 
Returns the image used for the decrement glyph of the control.

* **func** **setDecrementImageForState**(**image**: **[Image](Image.md)**, **state**: **[Int](../gravity/int.md)**)
Sets the image to use for the decrement glyph of the control.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

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



