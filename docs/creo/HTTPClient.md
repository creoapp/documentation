The [HTTPClient class](../classes/HTTPClient.html) and [HTTPRequest class](../classes/HTTPRequest.html) enable you to download content via HTTP. With an HTTPClient object you can configure the common connection parameters that can be used by one or more HTTPRequest, each of which represents a request for a specific URL.

The HTTPClient defines the protocol, the server host, the authentication parameters and the configuration of the connection behavior, such as whether to allow connections over a cellular network, the cookie policy, the cache policy and so on.

An `HTTPRequest` is always part of an `HTTPClient` and defines the request specific properties like the HTTP method, the path of the resource with the possibility to use dynamic values for header, path, query and body parameters.

![HTTPClient](../images/creo/HTTPClient_main.png)

### How to use
1. Drop a `HTTPClient` control from the object panel to a `Window` or to the _Globals_ folder.
2. Use the `HTTPClient Inspector` to customize its properties like `Protocol`, `Host`, and `Authentication`.
3. Click on the subnode button (+) and add a _Request_
4. Use the `HTTPRequest Inspector` to customize its properties like `Method`, `Path`, and `Serializer`.

![`HTTPClient` inspector](../images/creo/HTTPClient_inspector.png)
The inspector where the `HTTPClient` class can be configured.

![`HTTPRequest` inspector](../images/creo/HTTPRequest_inspector.png)
The inspector where the `HTTPRequest` class can be configured.

![`Code Editor` where to interact with events and write custom code](../images/creo/HTTPRequest_code.png)
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
- `NewValue`: Event raised when a new value becomes available.
- `DidFail`: Event raised when an error response is received. Use the `self.error` property to get the error.

### Most important properties
Most important properties for `HTTPClient`:
- `Protocol`: Choose between HTTP and HTTPS, the selection is reflected in the `Host` property.
- `Host`: The hostname of the HTTP server (the path component of the URL will be specified in the `HTTPRequest` subnode). Add here the _:port_ value if needed.
- `Authentication`: The type of authentication, choose between _No Auth_, _Basic Auth_ (`username` and `password`), _OAuth 1.0_ or _OAuth 2.0_.

The authentication details section depends on the selected authentication type.
The details are programmatically available through the `authDetails` property, the value of this property is a [Map](../gravity/map.html) where each key is a specific detail property for the selected authentication type.

- _No Auth_: no details are needed
- _Basic Auth_:
    - _username_
    - _password_
- _OAuth 1.0_:
    - _Callback URL_: The callback URL is used during the authorization process. After users authorize your application on the site, they'll be redirected back to your callback URL. The _schema_ of this URL must be added as a custom URL in the App's property list (ref: [Support URL TechNote](https://docs.creolabs.com/technotes/open-url.html)). Typically, you have to use a valid callback URL registered for your App's account in the developer page of your API. When the `HTTPClient` is run in the Creo Simulator or in the CreoPlayer, Creo uses the built-in callback URL *com.creolabs.creo://oauth1Callback* in order to be able to receive the callback, so you need to add this value in the API provider page if you want to test your App in these platforms. Your custom _Callback URL_ is used when your App is installed and executed in a real device. Example: "com.your-company-name.your-app-name://oauth1Callback"
    - _Request Token URL_: The URL, supplied by the site, used for acquiring temporary credentials in the first step of authorization flow (also known as a Request Token).
    - _Authorization URL_: The authorization URL supplied by the site.
    - _Access Token URL_: The token request endpoint supplied by the site.
    - _Signature Method_: **not yet supported**
    - _Consumer Key_: The client key supplied by the API provider.
    - _Consumer Secret_: The client secret supplied by the API provider.
    - _Consumer Key Simulator_: If the API provider doesn't allow to authorize two different callback URLs, you can create two different App accounts for the API, one for the built App with your personal callback URL and one for the Creo Simulator/CreoPlayer with the Creo built-in callback URL. Use this property to set the client _key_ related to the Creo built-in callback URL. If this property has an empty value, the _Consumer Key_ is used in the Creo Simulator and in the CreoPlayer.
    - _Consumer Secret Simulator_: If the API provider doesn't allow to authorize two different callback URLs, you can create two different App accounts for the API, one for the built App with your personal callback URL and one for the Creo Simulator/CreoPlayer with the Creo built-in callback URL. Use this property to set the client _secret_ related to the Creo built-in callback URL. If this property has an empty value, the _Consumer Secret_ is used in the Creo Simulator and in the CreoPlayer.
- _OAuth 2.0_:
    - _Response Type_: Informs the Authorization Server of the desired authorization processing flow, including what parameters are returned from the endpoints used.
    - _Redirect URI_: Where the service redirects the user-agent after an authorization code is granted. The _schema_ of this URL must be added as a custom URL in the App's property list (ref: [Support URL TechNote](https://docs.creolabs.com/technotes/open-url.html)). Typically, you have to use a valid redirect URI registered for your App's account in the developer page of your API. When the `HTTPClient` is run in the Creo Simulator or in the CreoPlayer, Creo uses the built-in redirect URI *com.creolabs.creo://oauth2Callback* in order to be able to receive the callback, so you need to add this value in the API provider page if you want to test your App in these platforms. Your custom _Redirect URI_ is used when your App is installed and executed in a real device. Example: "com.your-company-name.your-app-name://oauth2Callback".
    - _Authorization URL_: The API authorization endpoint.
    - _Access Token URL_: The API token endpoint.
    - _Scope_: The authorization and token endpoints allow the client to specify the
   scope of the access request.
    - _Client ID_: Once your application is registered, the service will issue "client credentials" in the form of a client identifier and a client secret. The Client ID is a publicly exposed string that is used by the service API to identify the application.
    - _Client Secret_: The Client Secret is used to authenticate the identity of the application to the service API when the application requests to access a user's account.
    - _Client ID Simulator_: If the API provider doesn't allow to authorize two different redirect URIs, you can create two different App accounts for the API, one for the built App with your personal callback URL and one for the Creo Simulator/CreoPlayer with the Creo built-in Redirect URI. Use this property to set the client ID related to the Creo built-in redirect URI. If this property has an empty value, the _Client ID_ is used in the Creo Simulator and in the CreoPlayer.
    - _Client Secret Simulator_: If the API provider doesn't allow to authorize two different redirect URIs, you can create two different App accounts for the API, one for the built App with your personal callback URL and one for the Creo Simulator/CreoPlayer with the Creo built-in Redirect URI. Use this property to set the client secret related to the Creo built-in redirect URI. If this property has an empty value, the _Client Secret_ is used in the Creo Simulator and in the CreoPlayer.

![`HTTPClient` inspector for OAuth 1.0](../images/creo/HTTPClient_OAuth1.0.png)
The inspector where the details for the OAuth 1.0 authentication of the `HTTPClient` class can be configured.

![`HTTPClient` inspector for OAuth 1.0](../images/creo/HTTPClient_OAuth2.0.png)
The inspector where the details for the OAuth 2.0 authentication of the `HTTPClient` class can be configured.

Most important properties for `HTTPRequest`:
- `Method`: Choose between _Get_, _Post_, _Head_, _Put_, _Patch_ or _Delete_.
- `Path`: The path component of the URL (the host part of the URL is defined by the HTTPClient parent node).
- `Serializer`: The response serializer used to validate and decode the server response and set the `self.value` property. Choose between the following values:
    - JSON: The `self.value` property with the JSON object (a combination of [Map](../gravity/map.html), [List](../gravity/list.html), [String](../gravity/types.html), [Numeric](../gravity/types.html), [Bool](../gravity/types.html) and [null](../gravity/types.html) objects) corresponding to the JSON representation from the response.
    - Data: set the `self.value` property with the [Data](../classes/Data.html) representation of the response.
    - Image: set the `self.value` property with [String](../gravity/types.html) representation of the response.
    - XML:
    - Plist: set the `self.value` property with the property list object corresponding to the Plist representation from the response.
    - Text: set  the `self.value` property with [String](../gravity/types.html) representation of the response.
- `Header Parameters`: each key/value pair is set as a field of the HTTP header of the request.
- `Path Parameters`: each segment of the path, separated by a slash, is automatically added to this [Map](../gravity/map.html). When the request is performed, the `HTTPRequest` replaces each path segment from the `Path` property with the value associated with path segment key. This feature let you change dynamically one or more path segments. For example, if your API have the URL 'https://www.your-api.com/USER_ID/request?' and the 'USER_ID' segment depends on an input value from your user, you can set the 'USER_ID/request' string in the `Path` property and the 'USER_ID' : '123' pair in the `Path Parameters` property; in this example the 'USER_ID' path segment will be replaced with the '123' value or with another custom value if dynamically changed during the execution of the App (ref: [Dynamic properties section](#Dynamic-properties)).
- `Query Parameters`: key/value pairs used to compose the query component of the URL. This property is automatically syncronized with the content of the `Path` property.  
- `Body Parameters` (only available for _Post_, _Put_ and _Patch_ methods): each key/value pair is added to the body of the request. The IDE inspector of this property let you just configure [String](../gravity/types.html) values, if you need to set object values (bool, numbers, maps, lists, null) you can do it programmatically by overriding the `bodyParameters` property or the [dynamic properties](#Dynamic-properties).

### <a id="Dynamic-properties"></a>Dynamic properties

The values of the following [Map](../gravity/map.html) parameters can also be accessed programmatically as a dynamic property of the HTTPRequest instance.

| Class | Property |
| ---------- | --------- |
| HTTPClient | Auth Details |
| HTTPRequest | Header Parameters |
| HTTPRequest | Path Parameters |
| HTTPRequest | Query Parameters |
| HTTPRequest | Body Parameters |

The dynamic properties are automatically exposed using the Map key as the property name if the key is a valid property name in Gravity (starts with a letter and contains only alphanumeric characters).

For example, if you have an `HTTPClient` named _HTTPClient1_ with an `HTTPRequest` named _Request1_ as a subnode and the _Request1_ as the `['userid' : 'xxx']` value for the `Path Parameters` property, you can programmatically set a new value for the 'userid' with the following code:
```
// Update the value of the 'userid' dynamic property.
// For example, if the Path property has value '/userid/request'
// and 'userid' is a key in the Path Paramentes property,
// then the next time the Request1 is executed its composed URL will be:
// '<protocol>://<host>/123/request' (where the <protocol> and <host> are defined
// by the HTTPClient1 parent object)
HTTPClient1.Request1.userid = "123"

// Force the execution of the HTTPRequest
if (HTTPClient1.Request1.running) HTTPClient1.Request1.stop()
HTTPClient1.Request1.run()
```

### References
- [HTTPClient class reference](../classes/HTTPClient.html) contains a complete list of properties and methods that can be used to customize a `HTTPClient` object.
- [HTTPRequest class reference](../classes/HTTPRequest.html) contains a complete list of properties and methods that can be used to customize a `HTTPRequest` object.

- [Spotify tutorial](../tutorials/spotify.html) contains an example of how to use a Web API with OAuth 2.0 user authentication.
