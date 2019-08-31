**super**: **[UIDatePicker](UIDatePicker.md)** (on iOS)

A DatePicker object is a control used for the inputting of date and time values. You can use a date picker to allow a user to enter either a point in time (calendar date, time value or both) or a time interval (for example for a timer).

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **Changed**()
This event is called to notify that the user changed the date/time value

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **datePickerMode**: **DatePickerMode**
The date picker mode. Determines whether the date picker should display a time, a date, a time and date or a countdown interval. For modes that include date or time values, you can also configure the locale, calendar, and time zone information as appropriate.

* **var** **date**: **[Date](Date.md)**
The date displayed by the date picker.

* **var** **localDate**: **[String](../gravity/string.md)**
The date displayed by the date picker computed with timezone and locale.

* **var** **minimumDate**: **[Date](Date.md)**
The minimum date that a date picker can show.

* **var** **maximumDate**: **[Date](Date.md)**
The maximum date that a date picker can show.

* **var** **countDownDuration**: **[Float](../gravity/float.md)**
The seconds from which the countdown timer counts down (when the mode property is set to countDownTimer).

* **var** **minuteInterval**: **[Int](../gravity/int.md)**
The interval at which the date picker should display minutes. You can use this property to set the interval displayed by the minutes wheel (for example, 15 minutes). The interval value must be evenly divided into 60; if it is not, the default value is used. The default and minimum values are 1; the maximum value is 30.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **setDateAnimated**(**date**: **[Date](Date.md)**, **animated**: **[Bool](../gravity/bool.md)**)
Sets the date to display in the date picker, with an option to animate the setting.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control



* None

### Enums

<div id="_enum_DatePickerMode"></div>

#### DatePickerMode
 * .CountDownTimer
 * .Date
 * .DateAndTime
 * .Time

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



