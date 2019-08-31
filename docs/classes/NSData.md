**super**: **[Object](../gravity/object.md)**

This class is reserved and cannot be directly instantiated.





### Properties

* **var** **length**: **[Int](../gravity/int.md)**
The number of bytes contained by the data object. \(read-only\)

* **var** **position**: **[Int](../gravity/int.md)**
The position used for the Read and Write methods. This proprerty is automatically incremented by all of the Read and Write methods.

* **var** **littleEndian**: **[Int](../gravity/int.md)**
The byte order used by the Read and Write methods. If true, values are stored with the least-significant bytes first. The default value is true.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **readUInt8**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a one-byte value from the data and returns it as a UInt8. See also the <code>position</code> property.

* **func** **readUInt16**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a two-bytes value from the data and returns it as a UInt16. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **readUInt32**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a four-bytes value from the data and returns it as a UInt32. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **readUInt64**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a eight-bytes value from the data and returns it as a UInt64. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **readInt8**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a one-byte value from the data and returns it as a Int8. See also the <code>position</code> property.

* **func** **readInt16**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a two-bytes value from the data and returns it as a Int16. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **readInt32**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a four-bytes value from the data and returns it as a Int32. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **readInt64**()<strong>: [Int](../gravity/int.md)</strong> 
Reads a eight-bytes value from the data and returns it as a Int64. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **readFloat**()<strong>: [Float](../gravity/float.md)</strong> 
Reads a four-bytes value from the data and returns it as a Float. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **readDouble**()<strong>: [Float](../gravity/float.md)</strong> 
Reads a eight-bytes value from the data and returns it as a Double. See also the <code>position</code> and the <code>littleEndian</code> properties.

* **func** **md5**()<strong>: [String](../gravity/string.md)</strong> 
Compute MD5 digest algorithm.

* **func** **sha1**()<strong>: [String](../gravity/string.md)</strong> 
Compute SHA1 digest algorithm.

* **func** **sha256**()<strong>: [String](../gravity/string.md)</strong> 
Compute SHA256 digest algorithm.

* **func** **sha512**()<strong>: [String](../gravity/string.md)</strong> 
Compute SHA512 digest algorithm.

* **func** **base64**()<strong>: [String](../gravity/string.md)</strong> 
Encode data to base64 string.





