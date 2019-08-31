**super**: **[BaseDataSet](BaseDataSet.md)**

A DataSet is a programmatically customizable BaseDataSet. You can customize the number of rows, columns and the value of each row/column by implementing the specific Event.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Rows**(): <strong>[Int](../gravity/int.md)</strong> 
This event lets you specify the number of rows of the DataSet.

* **Columns**(): <strong>[Int](../gravity/int.md)</strong> 
This event lets you specify the number of columns of the DataSet.

* **NameForColumn**(**column**: **[Int](../gravity/int.md)**): <strong>[String](../gravity/string.md)</strong> 
This event lets you specify the name of each column. The column names are used in the control inspectors to set source column for each property of the template view.

* **Value**(**row**: **[Int](../gravity/int.md)**, **column**: **[Int](../gravity/int.md)**): <strong>[Object](../gravity/object.md)</strong> 
This event lets you specify the value for each row/column pair.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: **[Object](../gravity/object.md)**)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



* None

