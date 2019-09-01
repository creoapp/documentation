**super**: **[UIWKWebView](UIWKWebView.md)** (on iOS)

A WebView object displays interactive web content, such as for an in-app browser. You can also use this class to move back and forward in the history of webpages, and you can even set some web content properties programmatically.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidStart**()
This event is called when a mainframe page load starts.

* **DidFail**(**error**: **[String](../gravity/string.md)**)
This event is called when an error occurs while starting to load data for the mainframe.

* **DidStartReceiving**()
This event is called when content starts arriving for the mainframe.

* **DidFinish**()
This event is called when a mainframe load completes.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **url**: **[String](../gravity/string.md)**
Navigates to a requested URL.

* **var** **html**: **[String](../gravity/string.md)**
Sets the webpage contents.

* **var** **title**: **[String](../gravity/string.md)**
The page title. \(read-only\)

* **var** **loading**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the view is currently loading content. \(read-only\)

* **var** **estimatedProgress**: **[Float](../gravity/float.md)**
An estimate of what fraction of the current navigation has been loaded. \(read-only\)

* **var** **hasOnlySecureContent**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether all resources on the page have been loaded through securely encrypted connections. \(read-only\)

* **var** **canGoBack**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether there is a back item in the back-forward list that can be navigated to. \(read-only\)

* **var** **canGoForward**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether there is a forward item in the back-forward list that can be navigated to. \(read-only\)

* **var** **allowsBackForwardNavigationGestures**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether horizontal swipe gestures will trigger back-forward list navigations.

* **var** **customUserAgent**: **[String](../gravity/string.md)**
The custom user agent string or null if no custom user agent string has been set.

* **var** **allowsLinkPreview**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether pressing on a link displays a preview of the destination for the link. In iOS this property is available on devices that support 3D Touch. Default value is false in iOS.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **goBack**()
Navigates to the back item in the back-forward list.

* **func** **goForward**()
Navigates to the forward item in the back-forward list.

* **func** **reload**()
Reloads the current page.

* **func** **reloadFromOrigin**()
Reloads the current page, performing end-to-end revalidation using cache-validating conditionals if possible.

* **func** **reset**()
Reset WebView content to blank page.

* **func** **stopLoading**()
Stops loading all resources on the current page.

* **func** **runJavaScript**(**javaScript**: **[String](../gravity/string.md)**, **onSuccess**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="onSuccess (obj: Object)" data-content="The onSuccess closure, if set, is executed when the when the command completes. The obj parameter is the result of the script evaluation.">Closure</a> = null**, **onError**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="onError (message: String)" data-content="The onError closure, if set, is executed when the script fails. Error string is returned as parameter.">Closure</a> = null**)
Evaluates a JavaScript code.

* **func** **loadHTML**(**html**: **[String](../gravity/string.md)**, **baseURL**: **[String](../gravity/string.md) = null**)
Sets the webpage contents and base URL.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **animations**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="animations ()" data-content="The animations closure, if set, contains the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value.">Closure</a>**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion (finished: Bool)" data-content="The completion closure, if set, is executed when the animation sequence ends. This block has no return value and takes a single Bool argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle.">Closure</a>**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_AnimationOption"></div>

#### AnimationOption
 * .AllowAnimatedContent
 * .AllowUserInteraction
 * .Autoreverse
 * .BeginFromCurrentState
 * .CurveEaseIn
 * .CurveEaseInOut
 * .CurveEaseOut
 * .CurveLinear
 * .LayoutSubviews
 * .OverrideInheritedCurve
 * .OverrideInheritedDuration
 * .OverrideInheritedOptions
 * .Repeat
 * .ShowHideTransitionViews
 * .TransitionCrossDissolve
 * .TransitionCurlDown
 * .TransitionCurlUp
 * .TransitionFlipFromBottom
 * .TransitionFlipFromLeft
 * .TransitionFlipFromRight
 * .TransitionFlipFromTop
 * .TransitionNone



