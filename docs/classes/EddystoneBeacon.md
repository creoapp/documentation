**super**: **[Object](../gravity/object.md)**

Information about an observed EddystoneBeacon beacon and its relative distance to the user’s device.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **beaconID**: **[EddystoneBeaconID](EddystoneBeaconID.md)**
The beaconID for this Eddystone. \(read-only\)

* **var** **rssi**: **[Int](../gravity/int.md)**
The received signal strength of the beacon, measured in decibels. This value is the average signal strength of the samples received since the last reported the range of the beacon to your app. Use this value for calibrating beacon transmission power. \(read-only\)

* **var** **telemetry**: **[Data](Data.md)**
The telemetry that may or may not have been seen for this beacon. \(read-only\)

* **var** **txPower**: **[Int](../gravity/int.md)**
Transmission power reported by beacon, expressed in dB. \(read-only\)

* **var** **txPower**: **[Int](../gravity/int.md)**
Transmission power reported by beacon, expressed in dB. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





