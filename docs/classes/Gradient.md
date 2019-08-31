**super**: **[Object](../gravity/object.md)**

The Gradient class provides support for drawing gradient fill colors, also known as shadings. This class provides convenience methods for drawing radial or linear (axial) gradients for rectangles and other objects. It also supports primitive methods that let you customize the shape of the gradient fill.
A gradient consists of two or more color changes over the range of the gradient shape. When creating a gradient object, you specify the colors and their locations relative to the start and end of the gradient. This combination of color and location is known as a color stop.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **colors**: **[List](../gravity/list.md)**
Returns an array of colors \(read-only\)

* **var** **locations**: **[List](../gravity/list.md)**
Returns an array of location \(read-only\)

* **var** **gradientType**: **GradientType**
Gradient type.

* **var** **minPosition**: **[Point](Point.md)**
The coordinate that defines the starting point of the gradient (from 0.0 to 1.0).

* **var** **maxPosition**: **[Point](Point.md)**
The coordinate that defines the ending point of the gradient (from 0.0 to 1.0).

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **addColorStop**(**color**: **[Color](Color.md)**, **location**: **[Float](../gravity/float.md)**)<strong>: [Int](../gravity/int.md)</strong> 
Add a new color stop to the gradient at the specified location.

* **func** **removeColorStop**(**index**: **[Int](../gravity/int.md)**)
Remove color stop at the specified index.

* **func** **updateColor**(**index**: **[Int](../gravity/int.md)**, **color**: **[Color](Color.md)**)
Update stop color at the specified index (with a new color).

* **func** **updateLocation**(**index**: **[Int](../gravity/int.md)**, **location**: **[Float](../gravity/float.md)**)
Update stop color at the specified index (with a new location).

* **func** **isEqual**(**gradient**: **[Gradient](Gradient.md)**)<strong>: [Bool](../gravity/bool.md)</strong> 
Compare two Gradient objects.





### Enums

<div id="_enum_GradientType"></div>

#### GradientType
 * .Linear
 * .Radial



