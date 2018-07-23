# HTTPServer

**super**: [Object](Object.md)

The HTTPServer class provides a small, lightweight, embeddable HTTP server for your applications.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidStart**()
The server has been successfully started.

* **DidFail**()
The attempt to start the server has failed.

* **DidStop**()
The server has been successfully stopped.

* **DidReceiveRequest**(**method**: <strong>[String](../gravity/types.md)</strong>, **path**: <strong>[String](../gravity/types.md)</strong>, **body**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Object](../gravity/types.md)</strong> 
This event is called to get a response for a request. You may return a String containing the HTML code of the response, an url or a file path to redirect the request or the Data to send. If the return value is invalid or null, the HTTPServer will use the default behavior, looking for the requested path in the specified document root.

* **WillSendResponse**(**host**: <strong>[String](../gravity/types.md)</strong>, **method**: <strong>[String](../gravity/types.md)</strong>, **path**: <strong>[String](../gravity/types.md)</strong>, **statusCode**: <strong>[Int](../gravity/types.md)</strong>, **contentLength**: <strong>[Int](../gravity/types.md)</strong>)
Notifies that the server is about to send a respose for a successful request.

* **WillSendResponseError**(**host**: <strong>[String](../gravity/types.md)</strong>, **method**: <strong>[String](../gravity/types.md)</strong>, **path**: <strong>[String](../gravity/types.md)</strong>, **statusCode**: <strong>[Int](../gravity/types.md)</strong>)
The server is about to send an error response.

* **DidPublishBonjour**(**domain**: <strong>[String](../gravity/types.md)</strong>, **type**: <strong>[String](../gravity/types.md)</strong>, **name**: <strong>[String](../gravity/types.md)</strong>)
The service has been successfully published via Bonjour.

* **DidFailBonjour**(**domain**: <strong>[String](../gravity/types.md)</strong>, **type**: <strong>[String](../gravity/types.md)</strong>, **name**: <strong>[String](../gravity/types.md)</strong>, **errorCode**: <strong>[String](../gravity/types.md)</strong>, **errorDomain**: <strong>[String](../gravity/types.md)</strong>)
The attempt to publish the service via Bonjour has failed.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).

</ul>

### Properties

* **var** **shouldAcceptWebDAV**: **[Bool](../gravity/types.md)**
Defines if the server should support WebDAV connections.

* **var** **shouldAcceptPostMethod**: **[Bool](../gravity/types.md)**
Defines if the server should support POST requests.

* **var** **maxRequestContentLength**: **[Int](../gravity/types.md)**
Defines the maximum size of POST requests to be accepted. By default it is 1 MB (1024 * 1024).

* **var** **interface**: **[String](../gravity/types.md)**
Set what interface you'd like the server to listen on. By default this is nil, which causes the server to listen on all available interfaces like en1, wifi etc. The interface may be specified by name (e.g. "en1" or "lo0") or by IP address (e.g. "192.168.4.34"). You may also use the special strings "localhost" or "loopback" to specify that the socket only accept connections from the local machine.

* **var** **port**: **[Int](../gravity/types.md)**
The default port number is zero, meaning the server will automatically use any available port. This is the recommended port value, as it avoids possible port conflicts with other applications. Technologies such as Bonjour can be used to allow other applications to automatically discover the port number. Note: As is common on most OS's, you need root privledges to bind to port numbers below 1024.

* **var** **listeningPort**: **[Int](../gravity/types.md)**
The listeningPort method will always return the port number the running server is listening for connections on. If the server is not running this method returns 0. \(read-only\)

* **var** **name**: **[String](../gravity/types.md)**
The name to use for this service via Bonjour. The default name is an empty string, which should result in the published name being the host name of the computer.

* **var** **publishedName**: **[String](../gravity/types.md)**
The name actually published via Bonjour. \(read-only\)

* **var** **type**: **[String](../gravity/types.md)**
The type of service to publish via Bonjour. No type is set by default, and one must be set in order for the service to be published.

</ul>

### Methods

* **func** **start**()
Attempts to starts the server on the configured port, interface, etc. On succes the <i>DidStart</i> event is fired, otherwise it fires a <i>DidFail</i> event.

* **func** **stop**()
Stops the server preventing it from accepting any new connections and closes the existing client connections.

* **func** **publishBonjour**()
Publishes the service via bonjour if the server is running. If the service was previously published, this method will unpublish and then republish it (if the server is running). See the <i>DidPublishBonjour</i> and <i>DidFailBonjour</i> events.

</ul>

</ul>

