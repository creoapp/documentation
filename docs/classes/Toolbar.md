**super**: **[UIToolbar](UIToolbar.md)** (on iOS)

A toolbar is a control that displays one or more buttons, called toolbar items. A toolbar momentarily highlights or does not change the appearance of an item when tapped. Toolbar images that represent normal and highlighted states of an item derive from the image you set, the image is automatically colored with the toolbar’s tintColor.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **barStyle**: **BarStyle**
The toolbar style that specifies its appearance.

* **var** **translucent**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the toolbar is translucent (true) or not (false). If the toolbar has a custom background image, the default is true if any pixel of the image has an alpha value of less than 1.0, and false otherwise. If you set this property to true on a toolbar with an opaque custom background image, the toolbar will apply a system opacity less than 1.0 to the image.

* **var** **barTintColor**: **[Color](Color.md)**
The tint color to apply to the toolbar background. This color is made translucent by default unless you set the translucent property to false.

* **var** **items**: **[List](../gravity/list.md)**
The items displayed on the toolbar.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control



* None

### Enumeration

<div name="_enum_BarStyle"></div>

#### BarStyle
 * .Black
 * .BlackOpaque
 * .BlackTranslucent
 * .Default

<div name="_enum_AnimationOption"></div>

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



