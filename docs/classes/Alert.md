**super**: [UIAlertController](UIAlertController.md) on iOS

The Alert class displays a customizable alert message to the user.

#### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
Use this event to be notified when navigation is about to be added to a view hierarchy.

* **DidShow**()
Use this event to be notified when navigation was added to a view hierarchy.

* **Action**(**index**: <strong>[Int](../gravity/types.md)</strong>, **title**: <strong>[String](../gravity/types.md)</strong>)
Use this event to be notified when user selects a button.

* **WillHide**()
Use this event to be notified when navigation is about to be removed from a view hierarchy.

* **DidHide**()
Use this event to be notified when navigation was removed from a view hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



#### Initializers

* **func** **Alert**(**title**: <strong>[String](../gravity/types.md)</strong>)
Create a new Alert message with a specified title.

* **func** **Alert**(**title**: <strong>[String](../gravity/types.md)</strong>, **message**: <strong>[String](../gravity/types.md)</strong>)
Create a new Alert message with a specified title and message.

* **func** **Alert**(**title**: <strong>[String](../gravity/types.md)</strong>, **message**: <strong>[String](../gravity/types.md)</strong>, **buttons**: <strong>[List](../gravity/lists.md)</strong>)
Create a new Alert message with a specified title and message plus an array of buttons titles.

* **func** **Alert**(**title**: <strong>[String](../gravity/types.md)</strong>, **message**: <strong>[String](../gravity/types.md)</strong>, **buttons**: <strong>[List](../gravity/lists.md)</strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>)
Create a new Alert message with a specified title and message plus an array of buttons titles. The closure parameter enables you to specify an action to be executed when user press a button (button index is passed as parameter).



#### Methods

* **func** **addActionWithTitle**(**title**: <strong>[String](../gravity/types.md)</strong>)
Use this method to add a button to a newly created Alert.

* **func** **show**()
Display Alert to the user.





