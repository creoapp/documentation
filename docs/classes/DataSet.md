**super**: [Object](Object.md)

This class is reserved and cannot be directly instantiated.



### Events

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: <strong>[Object](../gravity/types.md)</strong>)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.



### Properties

* **var** **treeData**: **[Bool](../gravity/types.md)**
Used to check if DataSet is representing complex hierarchical data. \(read-only\)

* **var** **value**: **[Object](../gravity/types.md)**
Used to retrieve current DataSet value. \(read-only\)

* **var** **running**: **[Bool](../gravity/types.md)**
Used to check if DataSet is running. \(read-only\)

* **var** **cancelled**: **[Bool](../gravity/types.md)**
Used to check if DataSet has been cancelled. \(read-only\)

* **var** **error**: **[String](../gravity/types.md)**
Last Error message. \(read-only\)



### Methods

* **func** **run**()
Start current DataSet.

* **func** **stop**()
Stop current DataSet.

* **func** **valueForKeyPath**(**baseKeyPath**: <strong>[String](../gravity/types.md)</strong>, **row**: <strong>[Int](../gravity/types.md)</strong>, **keyPath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Object](../gravity/types.md)</strong> 
Retrieve DataSet value based on combination of key path.





