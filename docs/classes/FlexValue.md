**super**: **[Object](../gravity/object.md)**



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Properties

* **var** **undefined**: **[Float](../gravity/float.md)**
Const undefined can be used as a value. \(read-only\)

* **var** **valueUndefined**: **[FlexValue](FlexValue.md)**
Const value undefined is a complex value used by flex methods \(read-only\)

* **var** **valueAuto**: **[FlexValue](FlexValue.md)**
Const value auto is a complex value used by flex methods \(read-only\)



### Properties

* **var** **unit**: **[Int](../gravity/int.md)**
Unit, point or percent \(read-only\)

* **var** **value**: **[Float](../gravity/float.md)**
Value

* **var** **isUndefined**: **[Bool](../gravity/bool.md)**
is undefined \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Initializers

* **func** **FlexValue**(**value**: **[Float](../gravity/float.md)**, **unit**: **<a href="#_enum_FlexUnit">FlexUnit</a>**)
Create a new FlexValue. The first argument is the value (Float), the second is the unit of the value (FlexUnit, Point or Percent)



### Methods

* **func** **setPoint**(**value**: **[Float](../gravity/float.md)**)
Set a new value with point as unit

* **func** **setPercent**(**value**: **[Float](../gravity/float.md)**)
Set a new value with percent as unit





### Enums

<div id="_enum_FlexUnit"></div>

#### FlexUnit
 * .Percent
 * .Point



