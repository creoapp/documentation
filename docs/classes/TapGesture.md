**super**: **[UITapGestureRecognizer](UITapGestureRecognizer.md)** (on iOS)

TapGesture is a concrete gesture recognizer that looks for single or multiple taps. For the gesture to be recognized, the specified number of fingers must tap the view a specified number of times. Although taps are discrete gestures, they are discrete for each state of the gesture recognizer; thus the associated action message is sent when the gesture begins and is sent for each intermediate state until (and including) the ending state of the gesture. Code that handles tap gestures should therefore test for the state of the gesture.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called when the object recognizes its gesture or, in some cases, a change in the gesture.

* **ShouldRecognizeSimultaneously**(**otherGesture**: **[UIGestureRecognizer](UIGestureRecognizer.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Asks if two gesture recognizers should be allowed to recognize gestures simultaneously. This event is called when recognition of a gesture by either this gesture recognizer or the other gesture recognizer passed as the parameter would block the other gesture recognizer from recognizing its gesture. Note that returning <i>true</i> is guaranteed to allow simultaneous recognition; returning <i>false</i>, on the other hand, is not guaranteed to prevent simultaneous recognition because the other gesture recognizer's event may return <i>true</i>. The default value is <i>false</i>.

* **ShouldBegin**(): <strong>[Bool](../gravity/types.md)</strong> 
Asks if a gesture recognizer should begin interpreting touches. This method is called when a gesture recognizer attempts to transition out of the GestureRecognizerState.Possible state. Returning <i>false</i> causes the gesture recognizer to transition to the GestureRecognizerState.Failed state. The default value is <i>true</i>.

* **ShouldReceiveTouch**(**touch**: **[UITouch](UITouch.md)**): <strong>[Bool](../gravity/types.md)</strong> 
Ask the delegate if a gesture recognizer should receive an object representing a touch. The default value is true.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **numberOfTapsRequired**: **[Int](../gravity/types.md)**
The number of taps for the gesture to be recognized. The default value is 1.

* **var** **numberOfTouchesRequired**: **[Int](../gravity/types.md)**
The number of fingers required to tap for the gesture to be recognized. The default value is 1.

* **var** **objectName**: **[String](../gravity/types.md)**
The name of the object.





