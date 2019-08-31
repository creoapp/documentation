**super**: **[UISwitch](UISwitch.md)** (on iOS)

You use the Toggle class to create and manage the On/Off buttons used, for example, in the Settings app for options such as Airplane Mode and Bluetooth. These objects are known as switches. The Toggle class declares a property and a method to control its on/off state. You can customize the appearance of the switch by changing the color used to tint the switch when it is on or off.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **Changed**(**value**: **[Bool](../gravity/bool.md)**)
Use this event to be notified when value changes.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **value**: **[Bool](../gravity/bool.md)**
A Boolean value that determines the off/on state of the switch. This property allows you to retrieve and set (without animation) a value determining whether the UISwitch object is on or off.

* **var** **onTintColor**: **[Color](Color.md)**
The color used to tint the appearance of the switch when it is turned on.

* **var** **thumbTintColor**: **[Color](Color.md)**
The color used to tint the appearance of the thumb.

* **var** **onImage**: **[Image](Image.md)**
The image displayed when the switch is in the on position.

* **var** **offImage**: **[Image](Image.md)**
The image displayed while the switch is in the off position.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **setOnAnimated**(**value**: **[Bool](../gravity/bool.md)**, **animated**: **[Bool](../gravity/bool.md)**)
Set the state of the switch to On or Off, optionally animating the transition.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control



* None

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



