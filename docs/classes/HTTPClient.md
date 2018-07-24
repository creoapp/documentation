**super**: **[Object](Object.md)**

The HTTPClient class and <a href="HTTPRequest.html">HTTPRequest</a> class enable you to downloading content via HTTP. With an HTTPClient object you can configure the common connection parameters that can be used by one or more HTTPRequest, each of which represents a request for a specific URL.

The HTTPClient defines the protocol, the server host, the authenticaion parameters and the configuration of the connection behavior, such as whether to allow connections over a cellular network, the cookie policy, the cache policy and so on.

An <a href="HTTPRequest.html">HTTPRequest</a> is always part of an HTTPClient and defines the request specific properties like the HTTP method, the path of the resource with the possibility to use dynamic values for header, path, query and body parameters.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **protocol**: **HTTPProtocol**
URL scheme.

* **var** **host**: **[String](../gravity/types.md)**
Hostname of the HTTP server.

* **var** **authType**: **HTTPAuth**
Type of authentication.

* **var** **authDetails**: **[Map](../gravity/maps.md)**
A dictionary containing the authentication details.

* **var** **requestCachePolicy**: **HTTPRequestCachePolicy**
Cache policy for requests.

* **var** **timeoutIntervalForRequest**: **[Float](../gravity/types.md)**
Default timeout for requests.  This will cause a timeout if no data is transmitted for the given timeout value, and is reset whenever data is transmitted.

* **var** **timeoutIntervalForResource**: **[Float](../gravity/types.md)**
Default timeout for requests.  This will cause a timeout if a resource is not able to be retrieved within a given timeout.

* **var** **networkServiceType**: **HTTPRequestNetworkServiceType**
The service type is used to provide the network layers with a hint as to the purpose of the request.  Most clients should not need to use this method.

* **var** **allowsCellularAccess**: **[Bool](../gravity/types.md)**
Allow NO if the receiver should not be allowed to use the built in cellular radios to satisfy the request, YES otherwise. The default is YES.

* **var** **HTTPShouldSetCookies**: **[Bool](../gravity/types.md)**
Allow the session to set cookies on requests.

* **var** **HTTPCookieAcceptPolicy**: **HTTPCookieAcceptPolicy**
Policy for accepting cookies. This overrides the policy otherwise specified by the cookie storage.





### Enumeration

#### HTTPProtocol
 * .HTTP
 * .HTTPS

#### HTTPAuth
 * .Basic
 * .Digest
 * .Nothing
 * .OAuth1
 * .OAuth2

#### HTTPRequestCachePolicy
 * .ReloadIgnoringCache
 * .ReloadIgnoringLocalAndRemoteCache
 * .ReloadIgnoringLocalCache
 * .ReturnCacheDataDontLoad
 * .ReturnCacheDataElseLoad
 * .RevalidatingCacheData
 * .UseProtocol

#### HTTPRequestNetworkServiceType
 * .Background
 * .Default
 * .Video
 * .VoIP
 * .Voice

#### HTTPCookieAcceptPolicy
 * .Always
 * .Never
 * .OnlyFromMainDocumentDomain



