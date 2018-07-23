# BluetoothPeripheral

**super**: [Object](Object.md)

The BluetoothPeripheral class enables you to publish services and to advertise these services to central devices which support Bluetooth 4.0 low-energy.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **UpdatedState**(**state**: <strong><a href="#_enum_BluetoothState">BluetoothState</a></strong>)
Event raised when the blueetooth central changes its state

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).

</ul>

### Properties

* **var** **state**: **BluetoothState**
Represents the current state of the peripheral manager. The PoweredOn state indicates that Bluetooth is currently powered on and available to use.

* **var** **isAdvertising**: **[Bool](../gravity/types.md)**
Represents the current state of the peripheral manager. A Boolean value indicating whether the peripheral is currently advertising data. \(read-only\)

</ul>

### Methods

* **func** **run**()
Activates the configured services and starts advertising them

* **func** **stop**()
Stops advertising and removes the active services.

* **func** **write**(**value**: <strong>[Object](../gravity/types.md)</strong>, **characteristicUUID**: <strong>[String](../gravity/types.md)</strong>)
Sets the value for the specified characteristic and notify the change if needed. If the value is a Data object it is written as is, otherwise (Number, String, etc.) the BluetoothPeripheral tries to encode the value for known characteristis.

</ul>

</ul>

### Enumeration

### BluetoothState* .PoweredOff
* .PoweredOn
* .Resetting
* .Unauthorized
* .Unknown
* .Unsupported
<br><br></ul>

