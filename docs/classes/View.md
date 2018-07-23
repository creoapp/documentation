**super**: [UIScrollView](UIScrollView.md) on iOS

The View class defines a rectangular area on the screen and the interfaces for managing the content in that area. At runtime, a view object handles the rendering of any content in its area and also handles any interactions with that content. The View class itself provides basic behavior for filling its rectangular area with a background color.

#### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Draw**(**rect**: <strong>[Rect](rect.md)</strong>)
Draws the receiver’s image within the passed-in rectangle.

* **TouchesBegan**(**touches**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when one or more new touches occurred in this view and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesMoved**(**touches**: <strong>[Object](../gravity/types.md)</strong>, **touchInside**: <strong>[Bool](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the location or force of a touch changes and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesEnded**(**touches**: <strong>[Object](../gravity/types.md)</strong>, **touchInside**: <strong>[Bool](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when one or more fingers are raised and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesCancelled**(**touches**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the sysyem receives a system interruption (such as a system alert) requiring cancellation of the touch sequence and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **DidScroll**()
This event is called when the user scrolls the content view.

* **DidEndDragging**(**decelerate**: <strong>[Bool](../gravity/types.md)</strong>)
This event is called when dragging ended in the scroll view. The scroll view sends this event when the user’s finger touches up after dragging content. The decelerating property of the scroll view controls deceleration. The decelerate value is true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is NO, scrolling stops immediately upon touch-up.

* **DidEndDecelerating**()
This event is called when the scroll view ends decelerating the scrolling movement.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



#### Properties

* **var** **autoContentSize**: **[Bool](../gravity/types.md)**
A Boolean value that specifies if template view instance must be kept in sync with current view frame, otherwise content view must be set manually.

* **var** **rowIndex**: **[Int](../gravity/types.md)**
Use this property to set row index in case of view used in a controls that require an array of views.

* **var** **customView**: **[CustomView](CustomView.md)**
Custom view template set in the View inspector.

* **var** **keyPath**: **[String](../gravity/types.md)**
The base keyPath to get a particular node of the <a href="DataSet.html">DataSet</a> value. The DataSet must provide a List of objects and each object represents a different item. The view shows an item at a time, depending on the rowIndex property value. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath defines the list of keys used to browse the data tree to get a List node. The values for each exposed property of the cell are retrieved by adding the current index and the cell property key to the base keyPath.



#### Methods

* **func** **reload**(**reloadDataSet**: <strong>[Bool](../gravity/types.md)</strong>)
Reloads the content of the view.

* **func** **image**(): <strong>[Image](image.md)</strong> 
Returns the rasterized Image of the current view.

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





#### Enumeration

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

