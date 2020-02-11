**super**: **[ESSBeaconScanner](ESSBeaconScanner.md)**

The EddystoneScanner object allows you to detect nearby EddistoneBeacon beacons.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidFindBeacon**(**beacon**: **[EddystoneBeacon](EddystoneBeacon.md)**)
Event raised when a monitored beacon comes in range. Not available on the iOS simulator.

* **DidLoseBeacon**(**beacon**: **[EddystoneBeacon](EddystoneBeacon.md)**)
Event raised when the user left the range of a monitored beacon. iOS delays exit notifications in undocumented ways. This built-in, non-adjustable delay prevents false “exit” events. The exit notification usually occurs between 30 and 60 seconds after the iBeacon is out of range. Not available on the iOS simulator.

* **DidUpdateBeacon**(**beacon**: **[EddystoneBeacon](EddystoneBeacon.md)**)
Event raised when the scanner receives a new UID frame from a previously recognized beacon. Not available on the iOS simulator.

* **DidFindURL**(**URL**: **[String](../gravity/string.md)**)
Event raised when a new set of beacons are available. The beacons parameter is an array of iBeacon objects. If beacons is empty, it may be assumed no beacons that match the specified region are nearby. Similarly if a specific beacon no longer appears in beacons, it may be assumed the beacon is no longer received by the device. Not available on the iOS simulator.

* **DidUpdateState**()
Event raised when the blueetooth sensor changes its state.

* **DidFail**(**error**: **[String](../gravity/string.md)**)
Event raised when an error has occurred.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **onLostTimeout**: **[Float](../gravity/float.md)**
If no messages has been received from a beacon for more than the specified timeout interval, the beacon is considered out of reach and a DidExitRegion event is raised for that beacon.

* **var** **bluethoothState**: **[Int](../gravity/int.md)**
Returns the current state of the bluetooth manager. The PoweredOn state indicates that the device (your iPhone or iPad, for instance) supports Bluetooth low energy and that Bluetooth is on and available to use. \(read-only\)

* **var** **isScanning**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether the EddystoneScanner is currently scanning. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **start**()
Start scanning for Eddystone beacons. The DidEnterRegion and DidExitRegion event are raised when the region is entered or exited. Not available on the iOS simulator and on the Creo simulator for Mac.

* **func** **stop**()
Stops scanning for Eddystone beacons. Not available on the iOS simulator and on the Creo simulator for Mac.





