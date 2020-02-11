**super**: **[Object](../gravity/object.md)**

BeaconID and type (UID or EID) of the Eddyston beacon

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **beaconID**: **[Data](Data.md)**
The raw beaconID data. \(read-only\)

* **var** **beaconType**: **[Int](../gravity/int.md)**
The type of the beacon. Currently only a couple of types are supported, UID and EID. \(read-only\)

* **var** **stringRepresentation**: **[String](../gravity/string.md)**
The raw beaconID string representation. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





