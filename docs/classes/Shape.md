**super**: [UIView](UIView.md) on iOS

Base class for <a href="LineShape.html">LineShape</a>, <a href="RectShape.html">RectShape</a>, <a href="OvalShape.html">OvalShape</a> and <a href="PolyShape.html">PolyShape</a> shapes.

#### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **TouchesBegan**(**touches**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when one or more new touches occurred in this view and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesMoved**(**touches**: <strong>[Object](../gravity/types.md)</strong>, **touchInside**: <strong>[Bool](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the location or force of a touch changes and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesEnded**(**touches**: <strong>[Object](../gravity/types.md)</strong>, **touchInside**: <strong>[Bool](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when one or more fingers are raised and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesCancelled**(**touches**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the sysyem receives a system interruption (such as a system alert) requiring cancellation of the touch sequence and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



#### Properties

* **var** **fillColor**: **[Color](color.md)**
Color used to fill the shape.

* **var** **fillGradient**: **[Gradient](gradient.md)**
Gradient used to fill the shape.

* **var** **strokeColor**: **[Color](color.md)**
Color used to stoke shape border.

* **var** **strokeThickness**: **[Float](../gravity/types.md)**
Border thickness.

* **var** **regularShape**: **[Bool](../gravity/types.md)**
If true then shape is forced to have same width and height.





