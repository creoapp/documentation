**super**: **[Object](Object.md)**

The Crypto module provides cryptographic and encoding functionalities.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Methods

* **func** **md5**(**string**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Compute MD5 digest algorithm.

* **func** **sha1**(**string**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Compute SHA1 digest algorithm.

* **func** **sha256**(**string**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Compute SHA256 digest algorithm.

* **func** **sha512**(**string**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Compute SHA512 digest algorithm.

* **func** **UUID**(): <strong>[String](../gravity/string.md)</strong> 
Create and returns a new UUID with RFC 4122 version 4 random bytes.

* **func** **hmacSHA256**(**string**: **[String](../gravity/string.md)**, **key**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Compute HMAC-SHA256.

* **func** **encodeStringToBase64**(**string**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Encode string to base64 string.

* **func** **decodeStringFromBase64**(**string**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Decode string from base64 string.

* **func** **encodeDataToBase64**(**data**: **[Data](Data.md)**): <strong>[String](../gravity/string.md)</strong> 
Encode data to base64 string.

* **func** **decodeDataFromBase64**(**string**: **[String](../gravity/string.md)**): <strong>[Data](Data.md)</strong> 
Decode data from base64 string.





