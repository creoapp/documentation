**super**: **[UIButton](UIButton.md)** (on iOS)

A Button object is a view that executes your custom code in response to user interactions. You communicate the purpose of a button using a text label, an image, or both.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **Action**()
This event is called when a touch is released (touch-up) inside the bounds of the button

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **title**: **[String](../gravity/types.md)**
The title of the button. Use this property instead of the titleForState and setTitleForState methods if you want to use the same title for all the button states.

* **var** **font**: **[Font](Font.md)**
The font used for the button’s title string.

* **var** **type**: **ButtonType**
Returns the button type. \(read-only\)

* **var** **currentTitle**: **[String](../gravity/types.md)**
Returns the title for the current button state. \(read-only\)

* **var** **currentTitleColor**: **[Color](Color.md)**
Returns the color of the title for the current button state. \(read-only\)

* **var** **currentTitleShadowColor**: **[Color](Color.md)**
Returns the color of the title shadow for the current button state. \(read-only\)

* **var** **currentImage**: **[Image](Image.md)**
Returns the image for the current button state. \(read-only\)

* **var** **currentBackgroundImage**: **[Image](Image.md)**
Returns the background image for the current button state. \(read-only\)



### Initializers

* **func** **Button**(**buttonType**: **<a href="#_enum_ButtonType">ButtonType</a>**)
Creates and returns a new button of the specified type.



### Methods

* **func** **titleForState**(**state**: **<a href="#_enum_ControlState">ControlState</a>**): <strong>[String](../gravity/types.md)</strong> 
Returns the title associated with the specified state.

* **func** **setTitleForState**(**title**: **[String](../gravity/types.md)**, **state**: **<a href="#_enum_ControlState">ControlState</a>**)
Sets the title associated with the specified state. At a minimum, you should set the value for the normal state. If a title is not specified for a state, the default behavior is to use the title associated with the normal state. If the value for normal is not set, then the property defaults to a system value.

* **func** **titleColorForState**(**state**: **<a href="#_enum_ControlState">ControlState</a>**): <strong>[Color](Color.md)</strong> 
Returns the title color used for the specified state.

* **func** **setTitleColorForState**(**color**: **[Color](Color.md)**, **state**: **<a href="#_enum_ControlState">ControlState</a>**)
Sets the color of the title to use for the specified state.

* **func** **titleShadowColorForState**(**state**: **<a href="#_enum_ControlState">ControlState</a>**): <strong>[Color](Color.md)</strong> 
Returns the shadow color of the title used for the specified state.

* **func** **setTitleShadowColorForState**(**color**: **[Color](Color.md)**, **state**: **<a href="#_enum_ControlState">ControlState</a>**)
Sets the color of the title shadow to use for the specified state.

* **func** **imageForState**(**state**: **<a href="#_enum_ControlState">ControlState</a>**): <strong>[Image](Image.md)</strong> 
Returns the image used for the specified state.

* **func** **setImageForState**(**image**: **[Image](Image.md)**, **state**: **<a href="#_enum_ControlState">ControlState</a>**)
Sets the image to use for the specified state.

* **func** **backgroundImageForState**(**state**: **<a href="#_enum_ControlState">ControlState</a>**): <strong>[Image](Image.md)</strong> 
Returns the background image used for the specified state.

* **func** **setBackgroundImageForState**(**image**: **[Image](Image.md)**, **state**: **<a href="#_enum_ControlState">ControlState</a>**)
Sets the background image to use for the specified state.

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### ButtonType
 * .ContactAdd
 * .Custom
 * .DetailDisclosure
 * .InfoDark
 * .InfoLight
 * .RoundedRect
 * .System

#### ControlState
 * .Application
 * .Disabled
 * .Focused
 * .Highlighted
 * .Normal
 * .Selected

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



