**super**: **[NetworkReachabilityManager](NetworkReachabilityManager.md)**

NetworkReachability monitors the reachability of domains, and addresses for both WWAN and WiFi network interfaces. It allows an application to determine the status of a system's current network configuration and the reachability of a target host. A remote host is considered reachable when a data packet, sent by an application into the network stack, can leave the local device. Reachability does not guarantee that the data packet will actually be received by the host. Reachability can be used to determine background information about why a network operation failed, or to trigger a network operation retrying when a connection is established. It should not be used to prevent a user from initiating a network request, as it's possible that an initial request may be required to establish reachability.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **status**: **[Int](../gravity/types.md)**
The current network reachability status. \(read-only\)

* **var** **reachable**: **[Bool](../gravity/types.md)**
Whether or not the network is currently reachable. \(read-only\)

* **var** **reachableViaWWAN**: **[Bool](../gravity/types.md)**
Whether or not the network is currently reachable via WWAN. \(read-only\)

* **var** **reachableViaWiFi**: **[Bool](../gravity/types.md)**
Whether or not the network is currently reachable via WiFi. \(read-only\)

* **var** **statusString**: **[String](../gravity/types.md)**
A localized string representation of the current network reachability status. \(read-only\)



### Class Methods

* **func** **allAddresses**(): <strong>[Map](../gravity/map.md)</strong> 
Returns all network interfaces and the their relative IPv4 or IPv6 address.

* **func** **ipAddress**(**IPv4**: **[Bool](../gravity/types.md) = true**): <strong>[String](../gravity/types.md)</strong> 
Returns the string representation of the IPv4 or IPv6 address of the device.

* **func** **ipAddressForInterface**(**NetworkInterface**: **[String](../gravity/types.md) = null**): <strong>[String](../gravity/types.md)</strong> 
Returns the string representation of the IPv4 or IPv6 address of the specified network interface.



### Initializers

* **func** **NetworkReachability**(**domain**: **[String](../gravity/types.md)**)
Returns an initialized network reachability manager for the specified domain.



### Methods

* **func** **start**()
Starts monitoring for changes in network reachability status.

* **func** **stop**()
Stops monitoring for changes in network reachability status.

* **func** **setOnStatusChange**(**closure**: **[Closure](../gravity/closure.md)**)
Sets a closure to be executed when the network availability host changes. The closure has no return value and takes two arguments: the NetworkReachability instance and the new reachability status.





