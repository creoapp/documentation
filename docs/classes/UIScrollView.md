**super**: [UIView](UIView.md) on iOS

This class is reserved and cannot be directly instantiated.



### Events

* **DidScroll**()
This event is called when the user scrolls the content view.

* **DidEndDragging**(**decelerate**: <strong>[Bool](../gravity/types.md)</strong>)
This event is called when dragging ended in the scroll view. The scroll view sends this event when the user’s finger touches up after dragging content. The decelerating property of the scroll view controls deceleration. The decelerate value is true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is NO, scrolling stops immediately upon touch-up.

* **DidEndDecelerating**()
This event is called when the scroll view ends decelerating the scrolling movement.



### Properties

* **var** **contentOffset**: **[Point](point.md)**
The point at which the origin of the content view is offset from the origin of the scroll view.

* **var** **contentSize**: **[Size](size.md)**
The size of the content view.

* **var** **contentInset**: **[EdgeInsets](edgeinsets.md)**
The distance that the content view is inset from the enclosing scroll view. Use this property to add to the scrolling area around the content.

* **var** **bounces**: **[Bool](../gravity/types.md)**
Boolean value that controls whether the scroll view bounces past the edge of content and back again. Bouncing visually indicates that scrolling has reached an edge of the content.

* **var** **alwaysBounceVertical**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether bouncing always occurs when vertical scrolling reaches the end of the content.

* **var** **alwaysBounceHorizontal**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether bouncing always occurs when horizontal scrolling reaches the end of the content view.

* **var** **pagingEnabled**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether paging is enabled for the scroll view.

* **var** **scrollEnabled**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether scrolling is enabled. When scrolling is disabled, the scroll view does not accept touch events; it forwards them up the responder chain.

* **var** **showsHorizontalScrollIndicator**: **[Bool](../gravity/types.md)**
A Boolean value that controls whether the horizontal scroll indicator is visible. The indicator is visible while tracking is underway and fades out after tracking.

* **var** **showsVerticalScrollIndicator**: **[Bool](../gravity/types.md)**
A Boolean value that controls whether the vertical scroll indicator is visible. The indicator is visible while tracking is underway and fades out after tracking.

* **var** **scrollIndicatorInsets**: **[EdgeInsets](edgeinsets.md)**
The distance the scroll indicators are inset from the edge of the scroll view.

* **var** **indicatorStyle**: **ScrollViewIndicatorStyle**
The style of the scroll indicators.

* **var** **decelerating**: **[Bool](../gravity/types.md)**
Returns whether the content is moving in the scroll view after the user lifted their finger. \(read-only\)



### Methods

* **func** **flashScrollIndicators**()
Displays the scroll indicators momentarily. You should call this method whenever you bring the scroll view to front.





### Enumeration

#### ScrollViewIndicatorStyle
 * .Black
 * .Default
 * .White



