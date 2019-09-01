**super**: **[UISegmentedControl](UISegmentedControl.md)** (on iOS)

A SegmentedControl object is a horizontal control made of multiple segments, each segment functioning as a discrete button. A segmented control affords a compact means to group together a number of controls. A segmented control can display a title (an String object) or an image (Image object). The SegmentedControl object automatically resizes segments to fit proportionally within their superview unless they have a specific width set. When you add and remove segments, you can request that the action be animated with sliding and fading effects.

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

* **var** **numberOfSegments**: **[Int](../gravity/int.md)**
Returns the number of segments the receiver has. \(read-only\)

* **var** **index**: **[Int](../gravity/int.md)**
The index number identifying the selected segment (you can set this property to select an item by its index).

* **var** **momentary**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether segments in the receiver show selected state.

* **var** **adjustWidthsByContent**: **[Bool](../gravity/bool.md)**
Indicates whether the control attempts to adjust segment widths based on their content widths.

* **var** **items**: **[List](../gravity/list.md)**
Array of items presented by the SegmentedControl.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **removeAllItems**()
Removes all items of the receiver.

* **func** **insertItem**(**item**: **[SegmentedControlItem](SegmentedControlItem.md)**, **index**: **[Int](../gravity/int.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Inserts the item at the specified position, optionally animating the transition.

* **func** **addItem**(**item**: **[SegmentedControlItem](SegmentedControlItem.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Inserts the item at the end of the existing items, optionally animating the transition.

* **func** **removeItemAtIndex**(**index**: **[Int](../gravity/int.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Removes the specified item, optionally animating the transition.

* **func** **removeItem**(**item**: **[SegmentedControlItem](SegmentedControlItem.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Removes the specified item, optionally animating the transition.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **animations**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="animations ()" data-content="The animations closure, if set, contains the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value.">Closure</a>**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion (finished: Bool)" data-content="The completion closure, if set, is executed when the animation sequence ends. This block has no return value and takes a single Bool argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle.">Closure</a>**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

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



