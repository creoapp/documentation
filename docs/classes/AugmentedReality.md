**super**: **[UIView](UIView.md)** (on iOS)

Augmented reality is the integration of digital information with the user's environment in real time. Unlike virtual reality, which creates a totally artificial environment, augmented reality uses the existing environment and overlays new information on top of it. CREO offers a built-in and ready to use control to easely add Augmented reality capabilities to your app.



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **LocationDidChange**(**location**: **[Location](Location.md)**)
This event is called when the current location changes.

* **DidReload**()
This event is called when the dataSet of the table completes a reload.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **radius**: **[Float](../gravity/float.md)**
Defines the distance (in meters) within which to ask to the datasource for markers (default 1000).

* **var** **latitude**: **[Float](../gravity/float.md)**
The latitude currenly used by the control. \(read-only\)

* **var** **longitude**: **[Float](../gravity/float.md)**
The longitude currenly used by the control. \(read-only\)

* **var** **radarPosition**: **[Point](Point.md)**
Radar position inside the control.

* **var** **showRadar**: **[Bool](../gravity/bool.md)**
A Boolean indicating whether the augmented reality control displays radar information.

* **var** **isRunning**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the control is running. \(read-only\)

* **var** **angleOfView**: **[Size](Size.md)**
The angle of view of the device. \(read-only\)

* **var** **keyPath**: **[String](../gravity/string.md)**
The base keyPath to get a particular node of the <a href="DataSet.html">DataSet</a> value. The DataSet must provide a List of objects and each object represents a different marker. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath defines the list of keys used to browse the data tree to get a List node. The values for each exposed property of the cell are retrieved by adding the current index and the cell property key to the base keyPath.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **start**()
Start processing DataSet data.

* **func** **stop**()
Stop execution.

* **func** **pause**()
Pause execution.



* None

