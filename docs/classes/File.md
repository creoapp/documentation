**super**: **[Object](Object.md)**

The File class is an object-oriented wrapper for a file descriptor. You use file handle objects to access data associated with files. You can read, write, and seek within the file.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **path**: **[String](../gravity/string.md)**
File full path. \(read-only\)

* **var** **name**: **[String](../gravity/string.md)**
File name. \(read-only\)

* **var** **extension**: **[String](../gravity/string.md)**
File extension. \(read-only\)

* **var** **error**: **[String](../gravity/string.md)**
Current error as String (if any). \(read-only\)

* **var** **offset**: **[Int](../gravity/int.md)**
File current offset. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **open**(**filePath**: **[Object](../gravity/object.md)**, **mode**: **<a href="#_enum_FileMode">FileMode</a> = 0**): <strong>[File](File.md)</strong> 
Opens the specified file using the optional FileMode and returns a File object.



### Methods

* **func** **seekToEnd**(): <strong>[Int](../gravity/int.md)</strong> 
Puts the file pointer at the end of the file referenced by the receiver and returns the new file offset.

* **func** **close**()
Disallows further access to the represented file.

* **func** **readData**(): <strong>[Data](Data.md)</strong> 
Reads the available data up to the end of file or maximum number of bytes. Returns a Data object.

* **func** **readString**(): <strong>[String](../gravity/string.md)</strong> 
Reads the available data up to the end of file or maximum number of bytes. Returns a String object.

* **func** **seekTo**(**position**: **[Int](../gravity/int.md)**)
Moves the file pointer to the specified offset within the file represented by the receiver.

* **func** **readDataOfLength**(**length**: **[Int](../gravity/int.md)**): <strong>[Data](Data.md)</strong> 
Reads data up to the specified number of bytes. Returns a Data object.

* **func** **readStringOfLength**(**length**: **[Int](../gravity/int.md)**): <strong>[String](../gravity/string.md)</strong> 
Reads data up to the specified number of bytes. Returns a String object.

* **func** **writeData**(**data**: **[Data](Data.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
Writes the specified data to the receiver. Returns true if the operation was successfully.

* **func** **writeString**(**string**: **[String](../gravity/string.md)**): <strong>[Bool](../gravity/bool.md)</strong> 
Writes the specified string to the receiver. Returns true if the operation was successfully.



* None

### Enumeration

<div name="_enum_FileMode"></div>
#### FileMode
 * .Read
 * .Update
 * .Write



