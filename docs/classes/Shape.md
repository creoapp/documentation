**super**: **[UIView](UIView.md)** (on iOS)

Base class for <a href="LineShape.html">LineShape</a>, <a href="RectShape.html">RectShape</a>, <a href="OvalShape.html">OvalShape</a> and <a href="PolyShape.html">PolyShape</a> shapes.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **TouchesBegan**(**touches**: **[Object](../gravity/object.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when one or more new touches occurred in this view and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesMoved**(**touches**: **[Object](../gravity/object.md)**, **touchInside**: **[Bool](../gravity/bool.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when the location or force of a touch changes and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesEnded**(**touches**: **[Object](../gravity/object.md)**, **touchInside**: **[Bool](../gravity/bool.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when one or more fingers are raised and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesCancelled**(**touches**: **[Object](../gravity/object.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when the sysyem receives a system interruption (such as a system alert) requiring cancellation of the touch sequence and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **fillColor**: **[Color](Color.md)**
Color used to fill the shape.

* **var** **fillGradient**: **[Gradient](Gradient.md)**
Gradient used to fill the shape.

* **var** **strokeColor**: **[Color](Color.md)**
Color used to stoke shape border.

* **var** **strokeThickness**: **[Float](../gravity/float.md)**
Border thickness.

* **var** **regularShape**: **[Bool](../gravity/bool.md)**
If true then shape is forced to have same width and height.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





