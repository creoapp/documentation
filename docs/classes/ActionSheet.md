**super**: **[Alert](Alert.md)**

The ActionSheet is a specific style of alert that appears in response to a control or action, and presents a set of two or more choices related to the current context. Use an action sheet to let people initiate tasks, or to request confirmation before performing a potentially destructive operation. NOTE: The ActionSheet class is not simulated in the Creo Simulator for Mac, an Alert is presented instead. You can test the real visualization of the ActionSheet by running the App in an Apple Simulator or in the CreoPlayer.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
Use this event to be notified when the ActionSheet is about to be added to a view hierarchy.

* **DidShow**()
Use this event to be notified when the ActionSheet was added to a view hierarchy.

* **DidShow**()
Use this event to be notified when the Alert was added to a view hierarchy.

* **Action**(**index**: **[Int](../gravity/int.md)**, **title**: **[String](../gravity/string.md)**)
Use this event to be notified when user selects a button.

* **WillHide**()
Use this event to be notified when the ActionSheet is about to be removed from a view hierarchy.

* **DidHide**()
Use this event to be notified when the ActionSheet was removed from a view hierarchy.

* **DidHide**()
Use this event to be notified when the Alert was removed from a view hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Constructors

* **func** **ActionSheet**(**title**: **[String](../gravity/string.md)**)
Create a new ActionSheet alert with a specified title.

* **func** **ActionSheet**(**title**: **[String](../gravity/string.md)**, **message**: **[String](../gravity/string.md)**)
Create a new ActionSheet alert with a specified title and message.

* **func** **ActionSheet**(**title**: **[String](../gravity/string.md)**, **message**: **[String](../gravity/string.md)**, **buttons**: **[List](../gravity/list.md)**)
Create a new ActionSheet alert with a specified title and message plus an array of buttons titles.

* **func** **ActionSheet**(**title**: **[String](../gravity/string.md)**, **message**: **[String](../gravity/string.md)**, **buttons**: **[List](../gravity/list.md)**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion (index: Int, title: String)" data-content="The completion closure, if set, is executed when the open action completes. Button index and title are passed as parameters.">Closure</a>**)
Create a new ActionSheet alert with a specified title and message plus an array of buttons titles. The completion closure (if set) enables you to specify an action to be executed when user press a button (button index is passed as parameter).



### Methods

* **func** **addActionWithTitle**(**title**: **[String](../gravity/string.md)**, **style**: **[Int](../gravity/int.md) = 0**)
Use this method to add a button to a an ActionSheet.

* **func** **show**()
Display the ActionSheet to the user.

* **func** **showFromView**(**view**: **[UIView](UIView.md)**, **rect**: **[Rect](Rect.md)**)
Display the ActionSheet to the user from a specific rect of the source view (iPad only). Use this method instead of the show method on iPad. The view parameter defines the view containing the anchor rectangle for the popover. The rect parameters defines the rectangle in the specified view in which to anchor the popover.





