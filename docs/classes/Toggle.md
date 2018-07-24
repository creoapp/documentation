**super**: [UISwitch](UISwitch.md) on iOS

You use the Toggle class to create and manage the On/Off buttons used, for example, in the Settings app for options such as Airplane Mode and Bluetooth. These objects are known as switches. The Toggle class declares a property and a method to control its on/off state. You can customize the appearance of the switch by changing the color used to tint the switch when it is on or off.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Changed**(**value**: <strong>[Bool](../gravity/types.md)</strong>)
Use this event to be notified when value changes.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **value**: **[Bool](../gravity/types.md)**
A Boolean value that determines the off/on state of the switch. This property allows you to retrieve and set (without animation) a value determining whether the UISwitch object is on or off.

* **var** **onTintColor**: **[Color](color.md)**
The color used to tint the appearance of the switch when it is turned on.

* **var** **thumbTintColor**: **[Color](color.md)**
The color used to tint the appearance of the thumb.

* **var** **onImage**: **[Image](image.md)**
The image displayed when the switch is in the on position.

* **var** **offImage**: **[Image](image.md)**
The image displayed while the switch is in the off position.



### Methods

* **func** **setOnAnimated**(**value**: <strong>[Bool](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md)</strong>)
Set the state of the switch to On or Off, optionally animating the transition.

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

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

<br><br>

