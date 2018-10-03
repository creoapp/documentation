The [HTTPClient class](../classes/HTTPClient.html) and [HTTPRequest class](../classes/HTTPRequest.html) enable you to download content via HTTP. With an HTTPClient object you can configure the common connection parameters that can be used by one or more HTTPRequest, each of which represents a request for a specific URL.

The HTTPClient defines the protocol, the server host, the authentication parameters and the configuration of the connection behavior, such as whether to allow connections over a cellular network, the cookie policy, the cache policy and so on.

An `HTTPRequest` is always part of an `HTTPClient` and defines the request specific properties like the HTTP method, the path of the resource with the possibility to use dynamic values for header, path, query and body parameters.

![HTTPClient](images/HTTPClient_main.png)

### How to use
1. Drop a `HTTPClient` control from the object panel to a `Window` or to the _Globals_ folder.
2. Use the `HTTPClient Inspector` to customize its properties like `Protocol`, `Host`, and `Authentication`.
3. Click on the subnode button (+) and add a _Request_
4. Use the `HTTPRequest Inspector` to customize its properties like `Method`, `Path`, and `Serializer`.

![`HTTPClient` inspector](images/HTTPClient_inspector.png)
The inspector where the `HTTPClient` class can be configured.

![`HTTPRequest` inspector](images/HTTPRequest_inspector.png)
The inspector where the `HTTPRequest` class can be configured.

![`Code Editor` where to interact with events and write custom code](images/HTTPRequest_code.png)
The `Code Editor` where to interact with events and write custom code and the `Log Panel` with a sample value after running the project in the `Simulator`.

### Example
1. Open the `Code Editor` (cmd + 6)
2. Select the `NewValue` item inside the `Events` group and write your custom code in the `Code Editor`
```
Console.write("HTTPRequest value: \(value)")
```
3. Select the `DidFail` item inside the `Events` group and write your custom code in the `Code Editor`
```
Console.write("HTTPRequest DidFail with error: \(self.error)")
```
4. Run the project in `Simulator` from the `Action Bar`

### Most important events
Most important events for an `HTTPRequest` object:
- `NewValue`: event raised when a new value becomes available.
- `DidFail`: event raised when an error response is received. Use the `self.error` property to get the error.

### Most important properties
Most important properties for `HTTPClient`:
- `Protocol`: choose between HTTP and HTTPS, the selection is reflected in the `Host` property.
- `Host`: the hostname of the HTTP server (the path part of the URL will be specified in the `HTTPRequest` subnode).
- `Authentication`: the type of authentication, choose between _No Auth_, _Basic Auth_ (`username` and `password`), _OAuth 1.0_ or _OAuth 2.0_.

The authentication details section depends on the selected authentication type.
The details are programmatically available through the `authDetails` property, the value of this property is a [Map](../gravity/map.html) where each key is a specific detail property for the selected authentication type.

- _No Auth_: no details are needed
- _Basic Auth_:
    - _username_
    - _password_
- _OAuth 1.0_:
    - _Callback URL_: The callback URL is used during the authorization process. After users authorize your application on the site, they'll be redirected back to your callback URL. The _schema_ of this URL must be added as a custom URL in the App's property list (ref: [Support URL TechNote](https://docs.creolabs.com/technotes/open-url.html)). Typically, you have to use a valid callback URL registered for your App's account in the developer page of your API. When the `HTTPClient` is run in the Creo Simulator or in the CreoPlayer, Creo uses the built-in callback URL *com.creolabs.creo://oauth1Callback* in order to be able to receive the callback, so you need to add this value in the API provider page if you want to test your App in these platforms. Your custom _Callback URL_ is used when your App is installed and executed in a real device. Example: "com.your-company-name.your-app-name://oauth1Callback"
    - _Request Token URL_: the URL, supplied by the site, used for acquiring temporary credentials in the first step of authorization flow (also known as a Request Token).
    - _Authorization URL_: the authorization URL supplied by the site.
    - _Access Token URL_: the token request endpoint supplied by the site.
    - _Signature Method_: **not yet supported**
    - _Consumer Key_:
    - _Consumer Secret_:
    - _Consumer Key Simulator_:
    - _Consumer Secret Simulator_:

### Dynamic properties



### References
- [HTTPClient class reference](../classes/HTTPClient.html) contains a complete list of properties and methods that can be used to customize a `HTTPClient` object.
- [HTTPRequest class reference](../classes/HTTPRequest.html) contains a complete list of properties and methods that can be used to customize a `HTTPRequest` object.

- [Spotify tutorial](../tutorials/spotify.html) contains an example of how to use a Web API with OAuth 2.0 user authentication.
