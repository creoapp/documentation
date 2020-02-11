**super**: **[Object](../gravity/object.md)**

Information about an observed iBeacon device and its relative distance to the user’s device.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **timestamp**: **[Date](Date.md)**
The time when this beacon was observed. \(read-only\)

* **var** **uuid**: **[String](../gravity/string.md)**
UUID associated with the beacon. \(read-only\)

* **var** **major**: **[Int](../gravity/int.md)**
Most significant value associated with the beacon. \(read-only\)

* **var** **minor**: **[Int](../gravity/int.md)**
Least significant value associated with the beacon. \(read-only\)

* **var** **proximity**: **[Int](../gravity/int.md)**
The value in this property gives a general sense of the relative distance to the beacon. Use it to quickly identify beacons that are nearer to the user rather than farther away. Values: Immediate (strong signal; usually up to a few centimeters), Near (medium signal; usually up to a few meters), Far (weak signal; more than a few meters), Unknown (not determined, usually when the signal is very weak) \(read-only\)

* **var** **accuracy**: **[Float](../gravity/float.md)**
The accuracy of the proximity value, measured in meters from the beacon. \(read-only\)

* **var** **rssi**: **[Int](../gravity/int.md)**
The received signal strength of the beacon, measured in decibels. This value is the average signal strength of the samples received since the last reported the range of the beacon to your app. Use this value for calibrating beacon transmission power. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





