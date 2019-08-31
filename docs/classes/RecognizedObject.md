**super**: **[Object](../gravity/object.md)**

The metadata of a recognized object.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **type**: **<a href="#_enum_MachineReadableObjectType">MachineReadableObjectType</a>**
The type of the metadata object. \(read-only\)

* **var** **frame**: **[Rect](Rect.md)**
The frame of the object in the camera preview. \(read-only\)

* **var** **value**: **[Rect](Rect.md)**
The string value created by decoding the binary payload according to the format of the machine readable code. Returns nil if a string representation cannot be created from the payload.. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





### Enums

<div id="_enum_MachineReadableObjectType"></div>

#### MachineReadableObjectType
 * .AztecCode
 * .Code128Code
 * .Code39Code
 * .Code39Mod43Code
 * .Code93Code
 * .DataMatrixCode
 * .EAN13Code
 * .EAN8Code
 * .ITF14Code
 * .Interleaved2of5Code
 * .PDF417Code
 * .QRCode
 * .UPCECode



