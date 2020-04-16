**super**: **[Window](Window.md)**

A SafariView object includes Safari features such as Reader, AutoFill, Fraudulent Website Detection, and content blocking..

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidShow**()
Use this event to be notified when window was added to a view hierarchy.

* **DidShake**()
Use this event to be notified when a shake event occurred.

* **KeyboardWillShow**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately prior to the display of the keyboard.

* **KeyboardDidShow**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately after the display of the keyboard.

* **KeyboardWillHide**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately prior to the dismissal of the keyboard.

* **KeyboardDidHide**(**keyboard**: **[Map](../gravity/map.md)**)
Posted immediately after the dismissal of the keyboard.

* **WillRotate**(**toOrientation**: **[Int](../gravity/int.md)**, **duration**: **[Float](../gravity/float.md)**)
Posted immediately prior to rotation of the interface.

* **DidRotate**(**fromOrientation**: **[Int](../gravity/int.md)**)
Posted immediately after the rotation of the interface.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **DidHide**()
Use this event to be notified when navigation was removed from a view hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Constructors

* **func** **SafariView**(**url**: **[String](../gravity/string.md)**)
.





