**super**: **[Object](Object.md)**



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Properties

* **var** **undefined**: **[Float](../gravity/types.md)**
Const undefined can be used as a value. \(read-only\)

* **var** **valueUndefined**: **[FlexValue](FlexValue.md)**
Const value undefined is a complex value used by flex methods \(read-only\)

* **var** **valueAuto**: **[FlexValue](FlexValue.md)**
Const value auto is a complex value used by flex methods \(read-only\)



### Properties

* **var** **unit**: **[Int](../gravity/types.md)**
Unit, point or percent \(read-only\)

* **var** **value**: **[Float](../gravity/types.md)**
Value

* **var** **isUndefined**: **[Bool](../gravity/types.md)**
is undefined \(read-only\)

* **var** **objectName**: **[String](../gravity/types.md)**
The name of the object.



### Initializers

* **func** **FlexValue**(**value**: **[Float](../gravity/types.md)**, **unit**: **<a href="#_enum_FlexUnit">FlexUnit</a>**)
Create a new FlexValue. The first argument is the value (Float), the second is the unit of the value (FlexUnit, Point or Percent)



### Methods

* **func** **setPoint**(**value**: **[Float](../gravity/types.md)**)
Set a new value with point as unit

* **func** **setPercent**(**value**: **[Float](../gravity/types.md)**)
Set a new value with percent as unit





### Enumeration

#### FlexUnit
 * .Percent
 * .Point



