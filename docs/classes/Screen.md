**super**: [Object](Object.md)

An object that defines the properties associated with a hardware-based display.

#### Events

* None

#### Properties

* **var** **bounds**: **[Rect](rect.md)**
The bounding rectangle of the screen, measured in points. \(read-only\)

* **var** **nativeBounds**: **[Rect](rect.md)**
The bounding rectangle of the physical screen, measured in pixels. \(read-only\)

* **var** **scale**: **[Float](../gravity/types.md)**
The natural scale factor associated with the screen. This value reflects the scale factor needed to convert from the default logical coordinate space into the device coordinate space of this screen. The default logical coordinate space is measured using points. For standard-resolution displays, the scale factor is 1.0 and one point equals one pixel. For Retina displays, the scale factor is 2.0 and one point is represented by four pixels. \(read-only\)





