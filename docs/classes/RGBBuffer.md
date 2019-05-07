**super**: **[Object](Object.md)**

A RGBBuffer object is used for Image direct-color pixel manipulations. A pixel can be read or written by setting its red, green, blue and alpha components.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **width**: **[Int](../gravity/types.md)**
The width of the RGBBuffer. \(read-only\)

* **var** **height**: **[Int](../gravity/types.md)**
The height of the RGBBuffer. \(read-only\)

* **var** **image**: **[Image](Image.md)**
Create an Image from the RGBBuffer values. \(read-only\)

* **var** **objectName**: **[String](../gravity/types.md)**
The name of the object.



### Class Methods

* **func** **valueFromRGB**(**red**: **[Int](../gravity/types.md)**, **green**: **[Int](../gravity/types.md)**, **blue**: **[Int](../gravity/types.md)**, **alpha**: **[Int](../gravity/types.md) = 255**): <strong>[Int](../gravity/types.md)</strong> 
Convert parameters to a 32bit packet value.



### Initializers

* **func** **RGBBuffer**(**width**: **[Int](../gravity/types.md)**, **height**: **[Int](../gravity/types.md)**)
Initializes and returns a new RGBSurface with the specified width and height.



### Methods

* **func** **getColor**(**x**: **[Int](../gravity/types.md)**, **y**: **[Int](../gravity/types.md)**): <strong>[Color](Color.md)</strong> 
Get Color component at the specified x, y coordinates.

* **func** **getValue**(**x**: **[Int](../gravity/types.md)**, **y**: **[Int](../gravity/types.md)**): <strong>[Int](../gravity/types.md)</strong> 
Get packet 32bit value at the specified x, y coordinates.

* **func** **setColor**(**x**: **[Int](../gravity/types.md)**, **y**: **[Int](../gravity/types.md)**, **color**: **[Color](Color.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Set Color component at the specified x, y coordinates.

* **func** **setValue**(**x**: **[Int](../gravity/types.md)**, **y**: **[Int](../gravity/types.md)**, **value**: **[Int](../gravity/types.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Set packet 32bit value at the specified x, y coordinates.

* **func** **setRGB**(**x**: **[Int](../gravity/types.md)**, **y**: **[Int](../gravity/types.md)**, **red**: **[Int](../gravity/types.md)**, **green**: **[Int](../gravity/types.md)**, **blue**: **[Int](../gravity/types.md)**, **alpha**: **[Int](../gravity/types.md) = 255**): <strong>[Bool](../gravity/types.md)</strong> 
Set RGBA values at the specified x, y coordinates.





