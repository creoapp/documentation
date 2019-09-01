**super**: **[UITextView](UITextView.md)** (on iOS)

The TextView class implements the behavior for a scrollable, multiline text region. The class supports the display of text using custom style information and also supports text editing. You typically use a text view to display multiple lines of text, such as when displaying the body of a large text document.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidBeginEditing**()
Use this event to be notified when editing began in the specified text field.

* **DidEndEditing**()
Use this event to be notified when editing stopped for the specified text field.

* **Changed**()
Use this event to be notified when text changed in the specified text field.

* **DidChangeSelection**()
Use this event to be notified when text selection changed in the specified text field.

* **DidScroll**()
This event is called when the user scrolls the content view.

* **DidEndDragging**(**decelerate**: **[Bool](../gravity/bool.md)**)
This event is called when dragging ended in the scroll view. The scroll view sends this event when the user’s finger touches up after dragging content. The decelerating property of the scroll view controls deceleration. The decelerate value is true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is NO, scrolling stops immediately upon touch-up.

* **DidEndDecelerating**()
This event is called when the scroll view ends decelerating the scrolling movement.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **text**: **[String](../gravity/string.md)**
The text displayed by the text view.

* **var** **rawText**: **[String](../gravity/string.md)**
The raw text currently set in the text view. \(read-only\)

* **var** **textColor**: **[Color](Color.md)**
The color of the text.

* **var** **textType**: **<a href="#_enum_TextType">TextType</a>**
A value that specifies how text must be interpreted and rendered.

* **var** **font**: **[Font](Font.md)**
The font of the text.

* **var** **textAlignment**: **<a href="#_enum_TextAlignment">TextAlignment</a>**
The technique to use for aligning the text.

* **var** **selectedRange**: **[Range](../gravity/range.md)**
The current selection range of the receiver.

* **var** **editable**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the receiver is editable.

* **var** **dataDetectorTypes**: **<a href="#_enum_DataDetectorTypes">DataDetectorTypes</a>**
The types of data converted to tappable URLs in the text view.

* **var** **clearsOnInsertion**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether inserting text replaces the previous contents.

* **var** **inputView**: **[UIView](UIView.md)**
The custom input view to display when the text view becomes the first responder.

* **var** **inputAccessoryView**: **[UIView](UIView.md)**
The custom accessory view to display when the text view becomes the first responder.

* **var** **autocapitalizationType**: **<a href="#_enum_TextAutocapitalizationType">TextAutocapitalizationType</a>**
The auto-capitalization style for the text object.

* **var** **autocorrectionType**: **<a href="#_enum_TextAutocorrectionType">TextAutocorrectionType</a>**
The autocorrection style for the text object.

* **var** **spellCheckingType**: **<a href="#_enum_TextSpellCheckingType">TextSpellCheckingType</a>**
The spell-checking style for the text object.

* **var** **keyboardType**: **<a href="#_enum_KeyboardType">KeyboardType</a>**
The keyboard style associated with the text object. The keyboard style identifies what keys are available on the keyboard and which ones appear by default.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **hasText**()<strong>: [Bool](../gravity/bool.md)</strong> 
Returns a Boolean value indicating whether the text view currently contains any text.

* **func** **appendText**(**text**: **[String](../gravity/string.md)**)
Appends a given string to the receiver.

* **func** **scrollRangeToVisible**(**range**: **[Range](../gravity/range.md)**)
Scrolls the receiver until the text in the specified range is visible.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **animations**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="animations ()" data-content="The animations closure, if set, contains the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value.">Closure</a>**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion (finished: Bool)" data-content="The completion closure, if set, is executed when the animation sequence ends. This block has no return value and takes a single Bool argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle.">Closure</a>**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_TextType"></div>

#### TextType
 * .HTML
 * .Markdown
 * .Text

<div id="_enum_TextAlignment"></div>

#### TextAlignment
 * .Center
 * .Justified
 * .Left
 * .Natural
 * .Right

<div id="_enum_DataDetectorTypes"></div>

#### DataDetectorTypes
 * .Address
 * .All
 * .CalendarEvent
 * .Link
 * .None
 * .PhoneNumber

<div id="_enum_TextAutocapitalizationType"></div>

#### TextAutocapitalizationType
 * .AllCharacters
 * .None
 * .Sentences
 * .Words

<div id="_enum_TextAutocorrectionType"></div>

#### TextAutocorrectionType
 * .Default
 * .No
 * .Yes

<div id="_enum_TextSpellCheckingType"></div>

#### TextSpellCheckingType
 * .Default
 * .No
 * .Yes

<div id="_enum_KeyboardType"></div>

#### KeyboardType
 * .ASCIICapable
 * .ASCIICapableNumberPad
 * .DecimalPad
 * .Default
 * .EmailAddress
 * .NamePhonePad
 * .NumberPad
 * .NumbersAndPunctuation
 * .PhonePad
 * .Twitter
 * .URL
 * .WebSearch

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



