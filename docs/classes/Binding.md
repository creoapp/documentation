**super**: **[Object](../gravity/object.md.md)**

This class is reserved and cannot be directly instantiated.

A Binding object is automatically created by the CREO runtime each time you bind two or more objects on the design board.

### Events

* **ConvertValue**(**value**: **[Object](../gravity/object.md)**): <strong>[Object](../gravity/object.md)</strong> 
Handle this event if you want to convert a value (or an array of values in case of multiple sources).

* **OnError**()
Handle this event if you want to take any action in case of binding error.



### Methods

* **func** **start**()
Manually start a binding

* **func** **stop**()
Manually stop a binding





