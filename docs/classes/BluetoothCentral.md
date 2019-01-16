**super**: **[BaseDataSet](BaseDataSet.md)**

The BluetoothCentral class enables you to discover, connect to and communicate with Bluetooth 4.0 low-energy devices.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **NewValue**(**value**: **[Map](../gravity/map.md)**)
Event raised when a new value becomes available. The value parameter is map.

* **UpdatedState**(**state**: **<a href="#_enum_BluetoothState">BluetoothState</a>**)
Event raised when the blueetooth central changes its state

* **ShouldConnect**(**peripheralName**: **[String](../gravity/types.md)**, **peripheralUUID**: **[String](../gravity/types.md)**, **RSSI**: **[Int](../gravity/types.md)**): <strong>[Bool](../gravity/types.md)</strong> 
The bluetooth central has discovered a peripheral that are advertising one of the configured services. Return true if the central should connect to this peripheral. If not implemented, the central will connect to any discovered peripheral.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **state**: **BluetoothState**
Returns the current state of the central manager. The PoweredOn state indicates that the central device (your iPhone or iPad, for instance) supports Bluetooth low energy and that Bluetooth is on and available to use.

* **var** **data**: **[Data](Data.md)**
Returs the row data of the last value received from a pheripheral. \(read-only\)

* **var** **characteristicUUID**: **[String](../gravity/types.md)**
Returs the characteristic UUID of the last value received from a pheripheral. \(read-only\)

* **var** **characteristicName**: **[String](../gravity/types.md)**
Returs the characteristic name of the last value received from a pheripheral. \(read-only\)

* **var** **serviceUUID**: **[String](../gravity/types.md)**
Returs the service UUID of the last value received from a pheripheral. \(read-only\)

* **var** **serviceName**: **[String](../gravity/types.md)**
Returs the service name of the last value received from a pheripheral. \(read-only\)

* **var** **peripheralId**: **[String](../gravity/types.md)**
Returs the peripheral ID of the last value received from a pheripheral. \(read-only\)

* **var** **peripheralName**: **[String](../gravity/types.md)**
Returs the peripheral name of the last value received from a pheripheral. \(read-only\)

* **var** **decodedValue**: **[Object](../gravity/types.md)**
Returs the decoded value of the last value received from a pheripheral. \(read-only\)



### Methods

* **func** **scanForPeripherals**()
Scans for peripherals that are advertising the configured services.

* **func** **stopScan**()
Stops scanning for peripherals.

* **func** **readValue**(**peripheral**: **[String](../gravity/types.md)**, **service**: **[String](../gravity/types.md)**, **characteristic**: **[String](../gravity/types.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Retrieves the value of a specified characteristic. Return true if the peripheral, service and characteristic are valid, false otherwise. If the value of the characteristic is successfully retrieved, you will be notified with a <code>NewValue</code> event.

* **func** **writeValue**(**value**: **[Object](../gravity/types.md)**, **peripheral**: **[String](../gravity/types.md)**, **service**: **[String](../gravity/types.md)**, **characteristic**: **[String](../gravity/types.md)**, **type**: **<a href="#_enum_CharacteristicWriteType">CharacteristicWriteType</a>**): <strong>[Bool](../gravity/types.md)</strong> 
Writes the value of a characteristic. If the value is a Data object it is written as is, otherwise (Number, String, etc.) the BluetoothCentral tries to encode the value for known characteristis. Return true if the peripheral, service and characteristic are valid, false otherwise. If the <code>WriteWithResponse</code> type is specified, <code>NewValue</code> event is called with the result of the write request.

* **func** **setNotifyValue**(**enabled**: **[Bool](../gravity/types.md)**, **peripheral**: **[String](../gravity/types.md)**, **service**: **[String](../gravity/types.md)**, **characteristic**: **[String](../gravity/types.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Enables or disables notifications/indications for the characteristic. If <i>characteristic</i> allows both, notifications will be used. When notifications/indications are enabled, updates to the characteristic value will be received via <code>NewValue</code> event.





### Enumeration

#### BluetoothState
 * .PoweredOff
 * .PoweredOn
 * .Resetting
 * .Unauthorized
 * .Unknown
 * .Unsupported

#### CharacteristicWriteType
 * .WriteWithResponse
 * .WriteWithoutResponse



