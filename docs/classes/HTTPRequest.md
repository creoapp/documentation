**super**: [DataSet](DataSet.md)

The HTTPRequest class and the <a href="HTTPClient.html">HTTPClient</a> class enable you to downloading content via HTTP. An HTTPRequest is always part of an <a href="HTTPClient.html">HTTPClient</a> and defines the request specific properties like the HTTP method, the path of the resource with the possibility to use dynamic values for header, path, query and body parameters.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: <strong>[Object](../gravity/types.md)</strong>)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **path**: **[String](../gravity/types.md)**
A string that represents the path and query component of the request URL. The scheme and host (and optionally the port, user and password) components are defined by the parent HTTPClient object. You can set directly a path string, otherwise this property is calculated from the tokenized path configured in the HTTPRequest inspector and the current values of the pathParameters and queryParameters properties.

* **var** **url**: **[String](../gravity/types.md)**
Full URL of the request. \(read-only\)

* **var** **method**: **HTTPMethod**
HTTP method.

* **var** **headerParameters**: **[Map](../gravity/maps.md)**
The key-value pairs of this Map are added to the HTTP header section of the request. Values must be strings. Each value of the Map can also be accessed programmatically as a dynamic property of the HTTPRequest instance. The dynamic properties are automatically exposed using the Map key as the property name if the key contains only alphanumeric characters.

* **var** **pathParameters**: **[Map](../gravity/maps.md)**
A Map used to replace tokens in the path string. When you add a key-value pair from the inspector, a new token named after the key is added to path string. Values must be strings. Each value of the Map can also be accessed programmatically as a dynamic property of the HTTPRequest instance. The dynamic properties are automatically exposed using the Map key as the property name if the key contains only alphanumeric characters. For example, you can programmatically set the value of a token named "userid" with the following code:<p> <code>HTTPClient1.Request1.userid = "my_user_id";<br />HTTPClient1.Request1.run();</code></p>If you programmatically set a custom value for the path property the pathParameters property is ignored.

* **var** **queryParameters**: **[Map](../gravity/maps.md)**
The key-value pairs of this Map are used to create the query string part of the URL. For example, if the value is <code>["count" : "10", "screen_name" : "getcreo"] </code>, the HTTPRequest adds the following string to the original path: <code>?count=10&screen_name=getcreo</code>. Values must be strings. Each value of the Map can also be accessed programmatically as a dynamic property of the HTTPRequest instances. The dynamic properties are automatically exposed using the Map key as the property name if the key contains only alphanumeric characters. If you programmatically set a custom value for the path property the queryParameters property is ignored.

* **var** **bodyParameters**: **[Object](../gravity/types.md)**
The body parameters to be encoded according to the bodyMode property. The HTTPBodyMode.FormData and HTTPBodyMode.FormUrlencoded encoding require a Map value for this property, the HTTPBodyMode.Raw requires a string (if the value is a Map, the first value is used), with the HTTPBodyMode.JSON you can set this property to any JSON valid data type (List, Map, Boolean, String, Number, null value). If the value is a Map, each value of the Map can also be accessed programmatically as a dynamic property of the HTTPRequest instance. The dynamic properties are automatically exposed using the Map key as the property name if the key contains only alphanumeric characters.. Only used for the POST, PUT or PATCH method.

* **var** **bodyMode**: **HTTPBodyMode**
How to serialize the body parameters. Only used for the POST, PUT or PATCH method.

* **var** **responseSerializerType**: **HTTPResponseSerializer**
How to deserialize the response.

* **var** **timeoutInterval**: **[Float](../gravity/types.md)**
The timeout interval, in seconds, for created requests. The default timeout interval is 60 seconds.

* **var** **useAuthentication**: **[Bool](../gravity/types.md)**
A flag to enable/disable the authentication defined by the HTTPClient.

* **var** **redirectMode**: **HTTPRedirectMode**
Defines what to do when an HTTP request is attempting to perform a redirection to a different URL

* **var** **MIMEType**: **[String](../gravity/types.md)**
The MIME type of the response. The MIME type is often provided by the response’s originating source. However, that value may be changed or corrected by a protocol implementation if it can be determined that the response’s source reported the information incorrectly. If the response’s originating source does not provide a MIME type, an attempt to guess the MIME type may be made. \(read-only\)

* **var** **expectedContentLength**: **[Int](../gravity/types.md)**
The expected length of the response’s content. This property’s value is -1 if the length can’t be determined. Some protocol implementations report the content length as part of the response, but not all protocols guarantee to deliver that amount of data. Clients should be prepared to deal with more or less data. \(read-only\)

* **var** **textEncodingName**: **[String](../gravity/types.md)**
The name of the text encoding provided by the response’s originating source. If no text encoding was provided by the protocol, this property’s value is nil. \(read-only\)

* **var** **suggestedFilename**: **[String](../gravity/types.md)**
A suggested filename for the response data. Accessing this property attempts to generate a filename using the following information, in order: A filename specified using the content disposition header, the last path component of the URL, the host of the URL. If the host of URL can't be converted to a valid filename, the filename "unknown" is used. In most cases, this property appends the proper file extension based on the MIME type. Accessing this property always returns a valid filename regardless of whether the resource is saved to disk. \(read-only\)

* **var** **allHeaderFields**: **[Map](../gravity/maps.md)**
A dictionary containing all the HTTP header fields received as part of the server’s response. By examining this dictionary clients can see the “raw” header information returned by the HTTP server. The keys in this dictionary are the header field names, as received from the server. See RFC 2616 for a list of commonly used HTTP header fields. HTTP headers are case insensitive. To simplify your code, certain header field names are canonicalized into their standard form. For example, if the server sends a content-length header, it is automatically adjusted to be Content-Length. The returned dictionary of headers is configured to be case-preserving during the set operation (unless the key already exists with a different case), and case-insensitive when looking up keys. \(read-only\)

* **var** **statusCode**: **[Int](../gravity/types.md)**
The receiver’s HTTP status code. See RFC 2616 for details. \(read-only\)

* **var** **localizedStatusCodeString**: **[String](../gravity/types.md)**
Returns a localized string corresponding to the current HTTP status code. \(read-only\)

* **var** **countOfBytesReceived**: **[Int](../gravity/types.md)**
The number of bytes that the object has received from the server in the response body. \(read-only\)

* **var** **countOfBytesSent**: **[Int](../gravity/types.md)**
The number of bytes that the task has sent to the server in the request body. This byte count includes only the length of the request body itself, not the request headers. \(read-only\)

* **var** **countOfBytesExpectedToSend**: **[Int](../gravity/types.md)**
The number of bytes that the task expects to send in the request body. The URL loading system can determine the length of the upload data in three ways: From the length of the NSData object provided as the upload body, from the length of the file on disk provided as the upload body of an upload task (not a download task), or from the Content-Length in the request object, if you explicitly set it. Otherwise, the value is -1 if you provided a stream or body data object, or zero (0) if you did not. \(read-only\)

* **var** **countOfBytesExpectedToReceive**: **[Int](../gravity/types.md)**
The number of bytes that the task expects to receive in the response body. This value is determined based on the Content-Length header received from the server. If that header is absent, the value is -1LL. \(read-only\)



### Methods

* **func** **suspend**()
Suspending a request will prevent the session from continuing to load data. There may still be event calls made by this object (for instance, to report data received while suspending) but no further transmissions will be made on behalf of the request until -resume is sent.  The timeout timer associated with the request will be disabled while a request is suspended. -suspend and -resume are nestable.

* **func** **resume**()
Resumes a previously suspended request

* **func** **cancel**()
Cancel returns immediately, but marks a request as being canceled. The request will invoke a DidFail event. Cancel may be sent to a request that has been suspended





### Enumeration

#### HTTPMethod
 * .Delete
 * .Get
 * .Head
 * .Patch
 * .Post
 * .Put

<br><br>#### HTTPBodyMode
 * .FormData
 * .FormUrlencoded
 * .JSON
 * .Raw

<br><br>#### HTTPResponseSerializer
 * .Data
 * .Image
 * .JSON
 * .Plist
 * .Text
 * .XML

<br><br>#### HTTPRedirectMode
 * .Allow
 * .Reject
 * .RejectAndCancel
 * .WithHandler

<br><br>

