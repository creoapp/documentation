**super**: [UISegmentedControl](UISegmentedControl.md) on iOS

A SegmentedControl object is a horizontal control made of multiple segments, each segment functioning as a discrete button. A segmented control affords a compact means to group together a number of controls. A segmented control can display a title (an String object) or an image (Image object). The SegmentedControl object automatically resizes segments to fit proportionally within their superview unless they have a specific width set. When you add and remove segments, you can request that the action be animated with sliding and fading effects.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **numberOfSegments**: **[Int](../gravity/types.md)**
Returns the number of segments the receiver has. \(read-only\)

* **var** **index**: **[Int](../gravity/types.md)**
The index number identifying the selected segment (you can set this property to select an item by its index).

* **var** **momentary**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether segments in the receiver show selected state.

* **var** **adjustWidthsByContent**: **[Bool](../gravity/types.md)**
Indicates whether the control attempts to adjust segment widths based on their content widths.

* **var** **items**: **[List](../gravity/lists.md)**
Array of items presented by the SegmentedControl.



### Methods

* **func** **removeAllItems**()
Removes all items of the receiver.

* **func** **insertItem**(**item**: <strong>[SegmentedControlItem](SegmentedControlItem.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
Inserts the item at the specified position, optionally animating the transition.

* **func** **addItem**(**item**: <strong>[SegmentedControlItem](SegmentedControlItem.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
Inserts the item at the end of the existing items, optionally animating the transition.

* **func** **removeItemAtIndex**(**index**: <strong>[Int](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
Removes the specified item, optionally animating the transition.

* **func** **removeItem**(**item**: <strong>[SegmentedControlItem](SegmentedControlItem.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
Removes the specified item, optionally animating the transition.

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

