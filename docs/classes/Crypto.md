**super**: [Object](Object.md)

The Crypto module provides cryptographic functionality.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Methods

* **func** **md5**(**string**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Compute MD5 digest algorithm.

* **func** **sha1**(**string**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Compute SHA1 digest algorithm.

* **func** **sha256**(**string**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Compute SHA256 digest algorithm.

* **func** **sha512**(**string**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Compute SHA512 digest algorithm.

* **func** **UUID**(): <strong>[String](../gravity/types.md)</strong> 
Create and returns a new UUID with RFC 4122 version 4 random bytes.





