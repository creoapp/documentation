**super**: **[UIToolbar](UIToolbar.md)** (on iOS)

A toolbar is a control that displays one or more buttons, called toolbar items. A toolbar momentarily highlights or does not change the appearance of an item when tapped. Toolbar images that represent normal and highlighted states of an item derive from the image you set, the image is automatically colored with the toolbar’s tintColor.

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

* **var** **barStyle**: **<a href="#_enum_BarStyle">BarStyle</a>**
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

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **animations**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="animations ()" data-content="The animations closure, if set, contains the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value.">Closure</a>**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion (finished: Bool)" data-content="The completion closure, if set, is executed when the animation sequence ends. This block has no return value and takes a single Bool argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle.">Closure</a>**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_BarStyle"></div>

#### BarStyle
 * .Black
 * .BlackOpaque
 * .BlackTranslucent
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



