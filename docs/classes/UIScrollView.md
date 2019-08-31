**super**: **[UIView](UIView.md)** (on iOS)

This class is reserved and cannot be directly instantiated.



### Events

* **DidScroll**()
This event is called when the user scrolls the content view.

* **DidEndDragging**(**decelerate**: **[Bool](../gravity/bool.md)**)
This event is called when dragging ended in the scroll view. The scroll view sends this event when the user’s finger touches up after dragging content. The decelerating property of the scroll view controls deceleration. The decelerate value is true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is NO, scrolling stops immediately upon touch-up.

* **DidEndDecelerating**()
This event is called when the scroll view ends decelerating the scrolling movement.



### Properties

* **var** **contentOffset**: **[Point](Point.md)**
The point at which the origin of the content view is offset from the origin of the scroll view.

* **var** **contentSize**: **[Size](Size.md)**
The size of the content view.

* **var** **contentInset**: **[EdgeInsets](EdgeInsets.md)**
The custom distance that the content view is inset from the safe area or scroll view edges.

* **var** **adjustedContentInset**: **[EdgeInsets](EdgeInsets.md)**
The insets derived from the content insets and the safe area of the scroll view. Available on iOS 11.0+. \(read-only\)

* **var** **contentInsetAdjustmentBehavior**: **[Int](../gravity/int.md)**
The behavior for determining the adjusted content offsets. Available on iOS 11.0+. <code>Automatic</code>: Similar to ScrollableAxes, but for backward compatibility (iOS < 11.0) will also adjust the top & bottom contentInset when the scroll view is owned by a view controller with automaticallyAdjustsScrollViewInsets = YES inside a navigation controller, regardless of whether the scroll view is scrollable. <code>ScrollableAxes</code>: Adjust the insets only in the scrollable directions. <code>Never</code>: Do not adjust the scroll view insets. <code>Always</code>: Always include the safe area insets in the content adjustment.

* **var** **bounces**: **[Bool](../gravity/bool.md)**
Boolean value that controls whether the scroll view bounces past the edge of content and back again. Bouncing visually indicates that scrolling has reached an edge of the content.

* **var** **alwaysBounceVertical**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether bouncing always occurs when vertical scrolling reaches the end of the content.

* **var** **alwaysBounceHorizontal**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether bouncing always occurs when horizontal scrolling reaches the end of the content view.

* **var** **pagingEnabled**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether paging is enabled for the scroll view.

* **var** **scrollEnabled**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether scrolling is enabled. When scrolling is disabled, the scroll view does not accept touch events; it forwards them up the responder chain.

* **var** **showsHorizontalScrollIndicator**: **[Bool](../gravity/bool.md)**
A Boolean value that controls whether the horizontal scroll indicator is visible. The indicator is visible while tracking is underway and fades out after tracking.

* **var** **showsVerticalScrollIndicator**: **[Bool](../gravity/bool.md)**
A Boolean value that controls whether the vertical scroll indicator is visible. The indicator is visible while tracking is underway and fades out after tracking.

* **var** **scrollIndicatorInsets**: **[EdgeInsets](EdgeInsets.md)**
The distance the scroll indicators are inset from the edge of the scroll view.

* **var** **indicatorStyle**: **<a href="#_enum_ScrollViewIndicatorStyle">ScrollViewIndicatorStyle</a>**
The style of the scroll indicators.

* **var** **decelerating**: **[Bool](../gravity/bool.md)**
Returns whether the content is moving in the scroll view after the user lifted their finger. \(read-only\)

* **var** **keyboardDismissMode**: **[Int](../gravity/int.md)**
The manner in which the keyboard is dismissed when a drag begins in the scroll view.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **flashScrollIndicators**()
Displays the scroll indicators momentarily. You should call this method whenever you bring the scroll view to front.





### Enums

<div id="_enum_ScrollViewIndicatorStyle"></div>

#### ScrollViewIndicatorStyle
 * .Black
 * .Default
 * .White



