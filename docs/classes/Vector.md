**super**: **[Object](Object.md)**

A container for coordinate values, direction vectors, matrices, and other non-scalar values, typically used for parameters in ImageFilter objects.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **count**: **[Int](../gravity/int.md)**
The number of items in the vector. \(read-only\)

* **var** **X**: **[Float](../gravity/float.md)**
The value located in the first position in the vector. \(read-only\)

* **var** **Y**: **[Float](../gravity/float.md)**
The value located in the second position in the vector. \(read-only\)

* **var** **Z**: **[Float](../gravity/float.md)**
The value located in the third position in the vector. \(read-only\)

* **var** **W**: **[Float](../gravity/float.md)**
The value located in the fourth position in the vector. \(read-only\)

* **var** **pointValue**: **[Point](Point.md)**
The values in the vector as a Point object. \(read-only\)

* **var** **rectValue**: **[Rect](Rect.md)**
The values in the vector as a Rect object. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Initializers

* **func** **Vector**(**values**: **[List](../gravity/list.md)**)
Initializes a vector with the provided values.



### Methods

* **func** **valueAtIndex**(**index**: **[Int](../gravity/int.md)**): <strong>[Float](../gravity/float.md)</strong> 
Returns a value from a specific position in the vector.





