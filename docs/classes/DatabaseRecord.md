**super**: **[Object](Object.md)**

A DatabaseRecord is a data structure that represent values to be used within the addRecord or updateRecord methods.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Methods

* **func** **bindNull**(**name**: **[String](../gravity/types.md)**)
Bind null value.

* **func** **bindText**(**name**: **[String](../gravity/types.md)**, **value**: **[String](../gravity/types.md)**)
Bind String value.

* **func** **bindBool**(**name**: **[String](../gravity/types.md)**, **value**: **[Bool](../gravity/types.md)**)
Bind Bool value.

* **func** **bindInt**(**name**: **[String](../gravity/types.md)**, **value**: **[Int](../gravity/types.md)**)
Bind Int value.

* **func** **bindInt64**(**name**: **[String](../gravity/types.md)**, **value**: **[Int](../gravity/types.md)**)
Bind Int64 value.

* **func** **bindDouble**(**name**: **[String](../gravity/types.md)**, **value**: **[Float](../gravity/types.md)**)
Bind Double value.

* **func** **bindData**(**name**: **[String](../gravity/types.md)**, **value**: **[Data](Data.md)**)
Bind Data value.





