**super**: **[Object](../gravity/object.md)**

This class is reserved and cannot be directly instantiated.



### Events

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: **[Object](../gravity/object.md)**)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.



### Properties

* **var** **treeData**: **[Bool](../gravity/bool.md)**
Used to check if DataSet is representing complex hierarchical data. \(read-only\)

* **var** **value**: **[Object](../gravity/object.md)**
Used to retrieve current DataSet value. \(read-only\)

* **var** **serverError**: **[Object](../gravity/object.md)**
Original raw error value received from the server. \(read-only\)

* **var** **running**: **[Bool](../gravity/bool.md)**
Used to check if DataSet is running. \(read-only\)

* **var** **cancelled**: **[Bool](../gravity/bool.md)**
Used to check if DataSet has been cancelled. \(read-only\)

* **var** **error**: **[String](../gravity/string.md)**
Last Error message. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **run**()
Start current DataSet.

* **func** **stop**()
Stop current DataSet.

* **func** **valueForKeyPath**(**baseKeyPath**: **[String](../gravity/string.md)**, **row**: **[Int](../gravity/int.md)**, **keyPath**: **[String](../gravity/string.md)**)<strong>: [Object](../gravity/object.md)</strong> 
Retrieve DataSet value based on combination of key path.

* **func** **valueForIndex**(**row**: **[Int](../gravity/int.md)**, **column**: **[Int](../gravity/int.md)**)<strong>: [Object](../gravity/object.md)</strong> 
Retrieve DataSet value based on row/column indexes.





