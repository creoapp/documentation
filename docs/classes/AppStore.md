**super**: **[Object](Object.md)**

The AppStore module provides support for in-app purchases and interactions with the App Store.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Methods

* **func** **requestReview**(): <strong>[Bool](../gravity/bool.md)</strong> 
Ask the user to rate or review your app, if appropriate. Although you should call this method when it makes sense in the user experience flow of your app, the actual display of a rating/review request view is governed by App Store policy. Because this method may or may not present an alert, it's not appropriate to call it in response to a button tap or other user action.





