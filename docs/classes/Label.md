**super**: **[UILabel](UILabel.md)** (on iOS)

The Label class implements a read-only text view. You can use this class to draw one or multiple lines of static text, such as those you might use to identify other parts of your user interface. The base Label class provides support for both simple and complex styling of the label text. You can also control over aspects of appearance, such as whether the label uses a shadow or draws with a highlight.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **TouchesBegan**(**touches**: **[Object](../gravity/object.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when one or more new touches occurred in this view and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesMoved**(**touches**: **[Object](../gravity/object.md)**, **touchInside**: **[Bool](../gravity/bool.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when the location or force of a touch changes and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesEnded**(**touches**: **[Object](../gravity/object.md)**, **touchInside**: **[Bool](../gravity/bool.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when one or more fingers are raised and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesCancelled**(**touches**: **[Object](../gravity/object.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when the sysyem receives a system interruption (such as a system alert) requiring cancellation of the touch sequence and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **heightThatFits**: **[Float](../gravity/float.md)**
Calculates and returns a height value that best fits the text. \(read-only\)

* **var** **text**: **[String](../gravity/string.md)**
The text displayed by the label.

* **var** **rawText**: **[String](../gravity/string.md)**
The raw text currently set in the label. \(read-only\)

* **var** **font**: **[Font](Font.md)**
The font of the text.

* **var** **textColor**: **[Color](Color.md)**
The color of the text.

* **var** **textAlignment**: **TextAlignment**
The technique to use for aligning the text.

* **var** **lineBreakMode**: **LineBreakMode**
The technique to use for wrapping and truncating the label’s text.

* **var** **textType**: **TextType**
A value that specifies how text must be interpreted and rendered.

* **var** **enabled**: **[Bool](../gravity/bool.md)**
The enabled state to use when drawing the label’s text.

* **var** **numberOfLines**: **[Int](../gravity/int.md)**
The maximum number of lines to use for rendering text.

* **var** **adjustsFontSizeToFitWidth**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the font size should be reduced in order to fit the title string into the label’s bounding rectangle.

* **var** **adjustsLetterSpacingToFitWidth**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether spacing between letters should be adjusted to fit the string within the label’s bounds rectangle.

* **var** **baselineAdjustment**: **BaselineAdjustment**
Controls how text baselines are adjusted when text needs to shrink to fit in the label.

* **var** **minimumScaleFactor**: **[Float](../gravity/float.md)**
The minimum scale factor supported for the label’s text. Use this property to specify the smallest multiplier for the current font size that yields an acceptable font size to use when displaying the label’s text. If you specify a value of 0 for this property, the current font size is used as the smallest font size.

* **var** **preferredMaxLayoutWidth**: **[Float](../gravity/float.md)**
he preferred maximum width (in points) for a multiline label.

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

### Enums

<div id="_enum_TextAlignment"></div>

#### TextAlignment
 * .Center
 * .Justified
 * .Left
 * .Natural
 * .Right

<div id="_enum_LineBreakMode"></div>

#### LineBreakMode
 * .CharWrapping
 * .Clipping
 * .TruncatingHead
 * .TruncatingMiddle
 * .TruncatingTail
 * .WordWrapping

<div id="_enum_TextType"></div>

#### TextType
 * .HTML
 * .Markdown
 * .Text

<div id="_enum_BaselineAdjustment"></div>

#### BaselineAdjustment
 * .AlignBaselines
 * .AlignCenters
 * .None

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



