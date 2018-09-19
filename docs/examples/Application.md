If you do not set any First Window into Creo IDE then you are responsible to manually call this method passing the right parameter (probably in the DidStart or FinishLaunching event):
```
App.loadContainer(Window1);
```

#### Schedule a local notification
```
var id = "Identifier1"
var title = "Title"
var delay = 3

// id, title and delay (in seconds) are required parameters
App.scheduleNotification(id, title, delay)  
```

#### Schedule a local notification with all options set
```
var notificationIdentifier = "Identifier1" // required
var title = "Title"    // required
var delay = 3 // in seconds, required
var body = "Body" // optional
var subtitle = "Subtitle" // optional
var badge = 3 // optional
var userInfo = ["key1": "value1", "key2": "value2"] // optional
var threadIdentifier = "ThreadIdentifier1" // optional
var actions = [["identifier": "Identifier1", "title": "Action1"], ["identifier": "Identifier2", "title": "Action2"]] // optional
var repeats = false // optional

App.scheduleNotification(notificationIdentifier, title, delay, body, subtitle, badge, userInfo, threadIdentifier, actions, repeats)  
```

#### Remove a pending local notification
```
var notificationIdentifier = "Identifier1"
App.removePendingNotifications([notificationIdentifier])
```

#### Remove all pending local notifications
```
App.removeAllPendingNotifications()
```

#### Remove a delivered local notification
```
var notificationIdentifier = "Identifier1"
App.removeDeliveredNotifications([notificationIdentifier])
```

#### Remove all delivered local notifications
```
App.removeAllDeliveredNotifications()
```