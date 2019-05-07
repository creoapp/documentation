**super**: **[UISearchBar](UISearchBar.md)** (on iOS)

The SearchBar class implements a text field control for text-based searches. The control provides a text field for entering text, a search button, a bookmark button, and a cancel button. The SearchBar object does not actually perform any searches. You use the events to implement the actions when text is entered and buttons are clicked.



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidBeginEditing**()
This event is called when the user begins editing the search text.

* **DidEndEditing**()
This event is called when user finished editing the search text.

* **Changed**(**searchText**: **[String](../gravity/types.md)**)
This event is called to notify that the user changed the search text

* **Action**(**action**: **<a href="#_enum_SearchBarAction">SearchBarAction</a>**)
This event is called when a button  was tapped.

* **DidSelectCell**(**selectedScopeIndex**: **[Int](../gravity/types.md)**)
This event is called when the scope button selection changed.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **searchBarStyle**: **SearchBarStyle**
A search bar style that specifies the search bar’s appearance.

* **var** **barStyle**: **BarStyle**
A bar style that specifies the search bar’s appearance.

* **var** **text**: **[String](../gravity/types.md)**
The current or starting search text.

* **var** **prompt**: **[String](../gravity/types.md)**
A single line of text displayed at the top of the search bar.

* **var** **placeholder**: **[String](../gravity/types.md)**
The string that is displayed when there is no other text in the text field.

* **var** **showsBookmarkButton**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the bookmark button is displayed.

* **var** **showsCancelButton**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the cancel button is displayed.

* **var** **showsSearchResultsButton**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the search results button is displayed.

* **var** **searchResultsButtonSelected**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the search results button is selected.

* **var** **translucent**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether the search bar is translucent (true) or not (false).

* **var** **barTintColor**: **[Color](Color.md)**
The tint color to apply to the search bar background.

* **var** **autocapitalizationType**: **TextAutocapitalizationType**
The auto-capitalization style for the text object.

* **var** **autocorrectionType**: **TextAutocorrectionType**
The autocorrection style for the text object.

* **var** **spellCheckingType**: **TextSpellCheckingType**
The spell-checking style for the text object.

* **var** **keyboardType**: **KeyboardType**
The keyboard style associated with the text object.

* **var** **scopeButtonTitles**: **[List](../gravity/list.md)**
An array of strings indicating the titles of the scope buttons.

* **var** **selectedScopeButtonIndex**: **[Int](../gravity/types.md)**
The index of the selected scope button.

* **var** **showsScopeBar**: **[Bool](../gravity/types.md)**
Specifies whether the scope bar is displayed.

* **var** **backgroundImage**: **[Image](Image.md)**
The background image for the search bar.

* **var** **scopeBarBackgroundImage**: **[Image](Image.md)**
The background image for the scope bar.

* **var** **searchFieldBackgroundPositionAdjustment**: **[Offset](Offset.md)**
The offset of the search text field background in the search bar.

* **var** **searchTextPositionAdjustment**: **[Offset](Offset.md)**
The offset of the text within the search text field background.

* **var** **inputAccessoryView**: **[UIView](UIView.md)**
The custom accessory view to display when the text field becomes the first responder.

* **var** **objectName**: **[String](../gravity/types.md)**
The name of the object.



### Methods

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### SearchBarAction
 * .Bookmark
 * .Cancel
 * .ResultsList
 * .Search

#### SearchBarStyle
 * .Default
 * .Minimal
 * .Prominent

#### BarStyle
 * .Black
 * .BlackOpaque
 * .BlackTranslucent
 * .Default

#### TextAutocapitalizationType
 * .AllCharacters
 * .None
 * .Sentences
 * .Words

#### TextAutocorrectionType
 * .Default
 * .No
 * .Yes

#### TextSpellCheckingType
 * .Default
 * .No
 * .Yes

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



