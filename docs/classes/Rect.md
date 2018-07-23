**super**: [Object](Object.md)

Represents a rectangle.

#### Properties

* **var** **x**: **[Float](../gravity/types.md)**
Rect origin x coordinate.

* **var** **y**: **[Float](../gravity/types.md)**
Rect origin y coordinate.

* **var** **width**: **[Float](../gravity/types.md)**
Rect width size value.

* **var** **height**: **[Float](../gravity/types.md)**
Rect height size value.



#### Initializers

* **func** **Rect**(**x**: <strong>[Float](../gravity/types.md)</strong>, **y**: <strong>[Float](../gravity/types.md)</strong>, **width**: <strong>[Float](../gravity/types.md)</strong>, **height**: <strong>[Float](../gravity/types.md)</strong>)
Create a new Rect object.



#### Methods

* **func** **copy**(): <strong>[Rect](rect.md)</strong> 
Copy a Rect object by value (duplicate).

* **func** **rectWithInset**(**point**: <strong>[Point](point.md)</strong>): <strong>[Rect](rect.md)</strong> 
Create a new Rect object with the specified inset.

* **func** **rectWithOffset**(**point**: <strong>[Point](point.md)</strong>): <strong>[Rect](rect.md)</strong> 
Create a new Rect object with the specified offset

* **func** **rectByUnion**(**rect**: <strong>[Rect](rect.md)</strong>): <strong>[Rect](rect.md)</strong> 
Create a new Rect object by performing the union operation between two specified Rect objects.

* **func** **rectByIntersection**(**rect**: <strong>[Rect](rect.md)</strong>): <strong>[Rect](rect.md)</strong> 
Create a new Rect object by performing intersection between two specified Rect objects.

* **func** **containsPoint**(**point**: <strong>[Point](point.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Check if it contains a specified Point.

* **func** **containsRect**(**rect**: <strong>[Rect](rect.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Check if it contains a specified Rect.

* **func** **intersectsRect**(**rect**: <strong>[Rect](rect.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns whether two rectangles intersect.

* **func** **minX**(): <strong>[Float](../gravity/types.md)</strong> 
Returns the smallest value for the x-coordinate of the rectangle.

* **func** **maxX**(): <strong>[Float](../gravity/types.md)</strong> 
Returns the largest value of the x-coordinate for the rectangle.

* **func** **minY**(): <strong>[Float](../gravity/types.md)</strong> 
Returns the smallest value for the y-coordinate of the rectangle.

* **func** **maxY**(): <strong>[Float](../gravity/types.md)</strong> 
Returns the largest value for the y-coordinate of the rectangle.

* **func** **midX**(): <strong>[Float](../gravity/types.md)</strong> 
Returns the x- coordinate that establishes the center of a rectangle.

* **func** **midY**(): <strong>[Float](../gravity/types.md)</strong> 
Returns the y-coordinate that establishes the center of the rectangle.





