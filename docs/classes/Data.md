**super**: **[NSData](NSData.md)**

Data class provide object-oriented wrappers for byte buffers.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Initializers

* **func** **Data**()
Instantiate a new Data object.



### Methods

* **func** **bytes**(**range**: **[Range](range.md)**): <strong>[Data](data.md)</strong> 
Copies a range of bytes from the receiver’s data.

* **func** **append**(**value**: **[Object](../gravity/types.md)**)
Appends to the receiver a given number of bytes from a given buffer. It supports numbers (64 bits representation) strings and Data.

* **func** **writeUInt8**(**value**: **[Int](../gravity/types.md)**)
Writes a one-byte unsigned integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> property.

* **func** **writeUInt16**(**value**: **[Int](../gravity/types.md)**)
Writes a two-bytes unsigned integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **writeUInt32**(**value**: **[Int](../gravity/types.md)**)
Writes a four-bytes unsigned integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **writeUInt64**(**value**: **[Int](../gravity/types.md)**)
Writes a eight-bytes unsigned integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **writeInt8**(**value**: **[Int](../gravity/types.md)**)
Writes a one-byte signed integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> property.

* **func** **writeInt16**(**value**: **[Int](../gravity/types.md)**)
Writes a two-bytes signed integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **writeInt32**(**value**: **[Int](../gravity/types.md)**)
Writes a four-bytes signed integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **writeInt64**(**value**: **[Int](../gravity/types.md)**)
Writes a eight-bytes signed integer value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **writeFloat**(**value**: **[Float](../gravity/types.md)**)
Writes a four-bytes float value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **writeDouble**(**value**: **[Float](../gravity/types.md)**)
Writes a eight-bytes double value to the data. Replaces the previous byte if the current <code>position</code> of the receiver is equal to the receiver's length, otherwise appends the byte to the receiver. See also the <code>position</code> and the <code>littleEndian</code> properties.





