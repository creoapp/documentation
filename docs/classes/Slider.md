**super**: [UISlider](UISlider.md) on iOS

A Slider object is a visual control used to select a single value from a continuous range of values. Sliders are always displayed as horizontal bars. An indicator, or thumb, notes the current value of the slider and can be moved by the user to change the setting.

#### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Changed**(**value**: <strong>[Float](../gravity/types.md)</strong>)
Use this event to be notified when value changes.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



#### Properties

* **var** **value**: **[Float](../gravity/types.md)**
Contains the receiver’s current value.

* **var** **minimumValue**: **[Float](../gravity/types.md)**
Contains the minimum value of the receiver.

* **var** **maximumValue**: **[Float](../gravity/types.md)**
Contains the maximum value of the receiver.

* **var** **continuous**: **[Bool](../gravity/types.md)**
Contains a Boolean value indicating whether changes in the sliders value generate continuous update events.

* **var** **minimumValueImage**: **[Image](image.md)**
Contains the image that is drawn on the side of the slider representing the minimum value.

* **var** **maximumValueImage**: **[Image](image.md)**
Contains the image that is drawn on the side of the slider representing the maximum value.

* **var** **minimumTrackTintColor**: **[Color](color.md)**
The color used to tint the standard minimum track images.

* **var** **maximumTrackTintColor**: **[Color](color.md)**
The color used to tint the standard maximum track images.

* **var** **thumbTintColor**: **[Color](color.md)**
The color used to tint the standard thumb images.

* **var** **currentMinimumTrackImage**: **[Image](image.md)**
Contains the minimum track image currently being used to render the receiver. \(read-only\)

* **var** **currentMaximumTrackImage**: **[Image](image.md)**
Contains the maximum track image currently being used to render the receiver. \(read-only\)

* **var** **currentThumbImage**: **[Image](image.md)**
Contains the thumb image currently being used to render the receiver. \(read-only\)



#### Methods

* **func** **setValueAnimated**(**value**: <strong>[Float](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
Sets the receiver’s current value, allowing you to animate the change visually.

* **func** **minimumTrackImageForState**(**state**: <strong><a href="#_enum_ControlState">ControlState</a></strong>): <strong>[Image](image.md)</strong> 
Returns the minimum track image associated with the specified control state.

* **func** **setMinimumTrackImageForState**(**image**: <strong>[Image](image.md)</strong>, **state**: <strong><a href="#_enum_ControlState">ControlState</a></strong>)
Assigns a minimum track image to the specified control states.

* **func** **maximumTrackImageForState**(**state**: <strong><a href="#_enum_ControlState">ControlState</a></strong>): <strong>[Image](image.md)</strong> 
Returns the maximum track image associated with the specified control state.

* **func** **setMaximumTrackImageForState**(**image**: <strong>[Image](image.md)</strong>, **state**: <strong><a href="#_enum_ControlState">ControlState</a></strong>)
Assigns a maximum track image to the specified control states.

* **func** **thumbImageForState**(**state**: <strong><a href="#_enum_ControlState">ControlState</a></strong>): <strong>[Image](image.md)</strong> 
Returns the thumb image associated with the specified control state.

* **func** **setThumbImageForState**(**image**: <strong>[Image](image.md)</strong>, **state**: <strong><a href="#_enum_ControlState">ControlState</a></strong>)
Assigns a thumb image to the specified control states.

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





#### Enumeration

#### ControlState
 * .Application
 * .Disabled
 * .Focused
 * .Highlighted
 * .Normal
 * .Selected
<br><br>#### AnimationOption
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

