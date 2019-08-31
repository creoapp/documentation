**super**: **[BaseDataSet](BaseDataSet.md)**

A network service browser that finds published services on a network using multicast DNS.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidFindService**(**bonjourService**: **[BonjourService](BonjourService.md)**)
Event raised when a searchForServices() request finds a service.

* **DidRemoveService**(**bonjourService**: **[BonjourService](BonjourService.md)**)
Event raised when a service has disappeared or has become unavailable during the execution of a searchForServices() search.

* **DidFail**(**error**: **[Map](../gravity/map.md)**)
Event raised when a searchForServices() request fails.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: **[Object](../gravity/object.md)**)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **resolveTimeout**: **[Float](../gravity/float.md)**
The maximum number of seconds to attempt to resolve the address for a given service. A value of 0.0 indicates no timeout and a resolve process of indefinite duration.

* **var** **domain**: **[String](../gravity/string.md)**
Default domain name in which to perform a searchForServices() request if the domainName parameter is not specified. The domainName argument can be an explicit domain name, the generic local domain "local." (note trailing period, which indicates an absolute name), or the empty string (@), which indicates the default registration domains. Usually, you pass in an empty string.

* **var** **serviceType**: **[String](../gravity/string.md)**
Default service type used when performing a searchForServices() request if the serviceType parameter is not specified. The serviceType must contain both the service type and transport layer information. To ensure that the mDNS responder searches for services, rather than hosts, make sure to prefix both the service name and transport layer name with an underscore character (“_”). For example, to search for an HTTP service on TCP, you would use the type string “_http._tcp.“. Note that the period character at the end is required.

* **var** **discoveredServices**: **[List](../gravity/list.md)**
List of discovered network services. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **searchForDomains**(**didFindDomain**: **[Closure](../gravity/closure.md) = null**, **didRemoveDomain**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)
Initiates a search for domains visible to the host.

* **func** **searchForServices**(**serviceType**: **[String](../gravity/string.md) = null**, **domainName**: **[String](../gravity/string.md) = null**, **didFindService**: **[Closure](../gravity/closure.md) = null**, **didRemoveService**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)
Starts a search for services of a particular type within a specific domain. The serviceType parameter defines the type of service to search for, if empty the BonjourBrowser uses the value from the inspector. The <code>serviceType</code> argument must contain both the service type and transport layer information. To ensure that the mDNS responder searches for services, rather than hosts, make sure to prefix both the service name and transport layer name with an underscore character (“_”). For example, to search for an HTTP service on TCP, you would use the type string “_http._tcp.“. Note that the period character at the end is required. The <code>domainName</code> parameter defines the domain in which to perform the search, if empty the BonjourBrowser uses the value from the inspector. The domainName argument can be an explicit domain name, the generic local domain "local." (note trailing period, which indicates an absolute name), or the empty string (@), which indicates the default registration domains. Usually, you pass in an empty string. The optional <code>didFindService</code> <a href="../gravity/closure.html">closures</a> is executed when the BonjourBrowser found a service; this closure is invoked with one arguments: the discovered BonjourService object. The optional <code>paramDidRemoveService</code> <a href="../gravity/closure.html">closures</a> is executed when a service has disappeared or has become unavailable; it is invoked with one arguments: the disappeared BonjourService object. The optional <code>paramOnError</code> <a href="../gravity/closure.html">closures</a> is executed when a search fails; it is invoked with one arguments: a <a href="../gravity/map.html">map</a> with the details of the error.

* **func** **stop**()
Halts a currently running search or resolution.





