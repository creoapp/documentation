**super**: **[UITextField](UITextField.md)** (on iOS)

A TextField object displays an editable text area in your interface. You use text fields to gather text-based input from the user using the onscreen keyboard. The keyboard is configurable for many different types of input such as plain text, emails, numbers, and so on. Text fields use the target-action mechanism and a delegate object to report changes made during the course of editing. In addition to its basic text-editing behavior, you can add overlay views to a text field to display additional information and provide additional tappable controls. You might add custom overlay views for elements such as a bookmarks button or search icon. Text fields provide a built-in overlay view to clear the current text. The use of custom overlay views is optional.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **ShouldBeginEditing**(): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the user performs an action that would normally initiate the editing of the text field’s text. Return true if editing should begin or false if it should not. Most of the time, you should return true to allow editing to proceed. If you do not implement this method, the text field acts as if this method had returned true.

* **ShouldEndEditing**(): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the control is asked to resign the first responder status. Return true if editing should stop or false if it should continue. Normally, you would return true from this method to allow the text field to resign the first responder status. You might return false, however, in cases where your delegate detects invalid contents in the text field. Returning false prevents the user from switching to another control until the text field contains a valid value.

* **ShouldChangeText**(**text**: **[String](../gravity/types.md)**, **range**: **[Range](../gravity/types.md)**): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the control is asked to check if the specified text should be changed. Return true if you accept the change or false to reject the change. Returning false prevents the user from changing the text. If you do not implement this method, the text field acts as if this method had returned true.

* **DidTapReturn**()
Use this event to implement any custom behavior when the return button is tapped.

* **DidBeginEditing**()
Use this event to be notified when editing began in the specified text field.

* **DidEndEditing**()
Use this event to be notified when editing stopped for the specified text field.

* **Changed**()
Use this event to be notified when text changed in the specified text field.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **text**: **[String](../gravity/types.md)**
The text displayed by the text field.

* **var** **rawText**: **[String](../gravity/types.md)**
The raw text currently set in the text field. \(read-only\)

* **var** **textColor**: **[Color](Color.md)**
The color of the text.

* **var** **font**: **[Font](Font.md)**
The font of the text.

* **var** **textAlignment**: **TextAlignment**
The technique to use for aligning the text.

* **var** **borderStyle**: **TextBorderStyle**
The border style used by the text field.

* **var** **placeholder**: **[String](../gravity/types.md)**
The string that is displayed when there is no other text in the text field.

* **var** **clearsOnBeginEditing**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the text field removes old text when editing begins.

* **var** **clearsOnInsertion**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether inserting text replaces the previous contents.

* **var** **endEditingOnReturn**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether end editing when the user taps the return button.

* **var** **adjustsFontSizeToFitWidth**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the font size should be reduced in order to fit the text string into the text field’s bounding rectangle.

* **var** **textType**: **TextType**
A value that specifies how text must be interpreted and rendered.

* **var** **minimumFontSize**: **[Float](../gravity/types.md)**
The size of the smallest permissible font with which to draw the text field’s text.

* **var** **background**: **[Image](Image.md)**
The image that represents the background appearance of the text field when it is enabled.

* **var** **disabledBackground**: **[Image](Image.md)**
The image that represents the background appearance of the text field when it is disabled.

* **var** **editing**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the text field is currently in edit mode.

* **var** **clearButtonMode**: **TextFieldViewMode**
Controls when the standard clear button appears in the text field.

* **var** **inputView**: **[UIView](UIView.md)**
The custom input view to display when the text field becomes the first responder.

* **var** **inputAccessoryView**: **[UIView](UIView.md)**
The custom accessory view to display when the text field becomes the first responder.

* **var** **nextField**: **[UITextField](UITextField.md)**
Configures the next field to activate, or nil if there is no next field.

* **var** **leftView**: **[UIView](UIView.md)**
The overlay view displayed on the left (or leading) side of the text field.

* **var** **rightView**: **[UIView](UIView.md)**
The overlay view displayed on the right (or trailing) side of the text field.



### Methods

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### TextAlignment
 * .Center
 * .Justified
 * .Left
 * .Natural
 * .Right

#### TextBorderStyle
 * .Bezel
 * .Line
 * .None
 * .RoundedRect

#### TextType
 * .HTML
 * .Markdown
 * .Text

#### TextFieldViewMode
 * .Always
 * .Never
 * .UnlessEditing
 * .WhileEditing

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



