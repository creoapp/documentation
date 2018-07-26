**super**: **[Object](Object.md)**

Represents a rectangle.

### Properties

* **var** **x**: **[Float](../gravity/types.md)**
Rect origin x coordinate.

* **var** **y**: **[Float](../gravity/types.md)**
Rect origin y coordinate.

* **var** **width**: **[Float](../gravity/types.md)**
Rect width size value.

* **var** **height**: **[Float](../gravity/types.md)**
Rect height size value.



### Initializers

* **func** **Rect**(**x**: **[Float](../gravity/types.md)**, **y**: **[Float](../gravity/types.md)**, **width**: **[Float](../gravity/types.md)**, **height**: **[Float](../gravity/types.md)**)
Create a new Rect object.



### Methods

* **func** **copy**(): <strong>[Rect](Rect.md)</strong> 
Copy a Rect object by value (duplicate).

* **func** **rectWithInset**(**point**: **[Point](Point.md)**): <strong>[Rect](Rect.md)</strong> 
Create a new Rect object with the specified inset.

* **func** **rectWithOffset**(**point**: **[Point](Point.md)**): <strong>[Rect](Rect.md)</strong> 
Create a new Rect object with the specified offset

* **func** **rectByUnion**(**rect**: **[Rect](Rect.md)**): <strong>[Rect](Rect.md)</strong> 
Create a new Rect object by performing the union operation between two specified Rect objects.

* **func** **rectByIntersection**(**rect**: **[Rect](Rect.md)**): <strong>[Rect](Rect.md)</strong> 
Create a new Rect object by performing intersection between two specified Rect objects.

* **func** **containsPoint**(**point**: **[Point](Point.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Check if it contains a specified Point.

* **func** **containsRect**(**rect**: **[Rect](Rect.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Check if it contains a specified Rect.

* **func** **intersectsRect**(**rect**: **[Rect](Rect.md)**): <strong>[Bool](../gravity/types.md)</strong> 
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





