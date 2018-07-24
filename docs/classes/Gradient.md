**super**: [Object](Object.md)

The Gradient class provides support for drawing gradient fill colors, also known as shadings. This class provides convenience methods for drawing radial or linear (axial) gradients for rectangles and other objects. It also supports primitive methods that let you customize the shape of the gradient fill.
A gradient consists of two or more color changes over the range of the gradient shape. When creating a gradient object, you specify the colors and their locations relative to the start and end of the gradient. This combination of color and location is known as a color stop.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **colors**: **[List](../gravity/lists.md)**
Returns an array of colors \(read-only\)

* **var** **locations**: **[List](../gravity/lists.md)**
Returns an array of location \(read-only\)

* **var** **gradientType**: **GradientType**
Gradient type.



### Methods

* **func** **addColorStop**(**color**: <strong>[Color](color.md)</strong>, **location**: <strong>[Float](../gravity/types.md)</strong>): <strong>[Int](../gravity/types.md)</strong> 
Add a new color stop to the gradient at the specified location.

* **func** **removeColorStop**(**index**: <strong>[Int](../gravity/types.md)</strong>)
Remove color stop at the specified index.

* **func** **updateColor**(**index**: <strong>[Int](../gravity/types.md)</strong>, **color**: <strong>[Color](color.md)</strong>)
Update stop color at the specified index (with a new color).

* **func** **updateLocation**(**index**: <strong>[Int](../gravity/types.md)</strong>, **location**: <strong>[Float](../gravity/types.md)</strong>)
Update stop color at the specified index (with a new location).

* **func** **isEqual**(**gradient**: <strong>[Gradient](gradient.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Compare two Gradient objects.





### Enumeration

#### GradientType
 * .Linear
 * .Radial



