**super**: **[Object](Object.md)**

A network service that broadcasts its availability using multicast DNS.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **hostName**: **[String](../gravity/string.md)**
A string containing the DNS hostname for this service. \(read-only\)

* **var** **domain**: **[String](../gravity/string.md)**
A string containing the domain for this service. \(read-only\)

* **var** **name**: **[String](../gravity/string.md)**
A string containing the name of this service. \(read-only\)

* **var** **type**: **[String](../gravity/string.md)**
The type of the published service. \(read-only\)

* **var** **port**: **[Int](../gravity/int.md)**
The port on which the service is listening for connections. \(read-only\)

* **var** **addresses**: **[List](../gravity/list.md)**
A read-only array containing NSData objects, each of which contains a socket address for the service. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



* None

