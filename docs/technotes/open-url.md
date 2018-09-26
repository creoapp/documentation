**Open an external App using a custom Url**
```
var url = "appname://message"
App.openURL(url)
```

**Process custom Urls sent by external Apps**
1. Select the App object inside the layout area
2. Place the code below into the OpenUrl ( url, options ) event

```
if (url.contains("message1")) {
    // process the message1 case 
    return true
}

if (url.contains("message2")) {
    // process the message2 case 
    return true
}

return false
```

**How to configure custom Urls in Creo**
1. Open the Properties window from the menu Project.
2. Configure the CFBundleURLTypes and LSApplicationQueriesSchemes main areas as represented into the example image.
3. Every item inside the CFBundleURLSchemes area represents the name to associate to  your app.
4. Every item inside the LSApplicationQueriesSchemes area represents the message name allowed to be processed by your app.

![OpenURL](../images/technotes/openurl.png)