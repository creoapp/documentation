**super**: **[BaseDataSet](BaseDataSet.md)**

A FileDataSet is a DataSet that reads data from a file. The supported file formats are JSON, Plist, CSV and XML.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: **[Object](../gravity/types.md)**)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **filePath**: **[String](../gravity/types.md)**
A string that represents the path of the file.

* **var** **type**: **[Int](../gravity/types.md)**
A string that represents the path of the file.

* **var** **hasHeader**: **[Bool](../gravity/types.md)**
Defines if the CSV file contains the column names in the first row (CSV type only).

* **var** **separator**: **[String](../gravity/types.md)**
The delimiter character to be used when parsing the fields of the CSV file (CSV type only).

* **var** **objectName**: **[String](../gravity/types.md)**
The name of the object.





