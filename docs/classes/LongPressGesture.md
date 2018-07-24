**super**: [UILongPressGestureRecognizer](UILongPressGestureRecognizer.md) on iOS

LongPressGesture is a concrete gesture recognizer that looks for long-press gestures. The user must press one or more fingers on a view and hold them there for a minimum period of time before the action triggers. While down, the user’s fingers may not move more than a specified distance; if they move beyond the specified distance, the gesture fails. Long-press gestures are continuous. The gesture begins (GestureRecognizerState.Began) when the number of allowable fingers (numberOfTouchesRequired) have been pressed for the specified period (minimumPressDuration) and the touches do not move beyond the allowable range of movement (allowableMovement). The gesture recognizer transitions to the Change state whenever a finger moves, and it ends (GestureRecognizerState.Ended) when any of the fingers are lifted.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called when the object recognizes its gesture or, in some cases, a change in the gesture.

* **ShouldRecognizeSimultaneously**(**otherGesture**: <strong>[UIGestureRecognizer](UIGestureRecognizer.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Asks if two gesture recognizers should be allowed to recognize gestures simultaneously. This event is called when recognition of a gesture by either this gesture recognizer or the other gesture recognizer passed as the parameter would block the other gesture recognizer from recognizing its gesture. Note that returning <i>true</i> is guaranteed to allow simultaneous recognition; returning <i>false</i>, on the other hand, is not guaranteed to prevent simultaneous recognition because the other gesture recognizer's event may return <i>true</i>. The default value is <i>false</i>.

* **ShouldBegin**(): <strong>[Bool](../gravity/types.md)</strong> 
Asks if a gesture recognizer should begin interpreting touches. This method is called when a gesture recognizer attempts to transition out of the GestureRecognizerState.Possible state. Returning <i>false</i> causes the gesture recognizer to transition to the GestureRecognizerState.Failed state. The default value is <i>true</i>.

* **ShouldReceiveTouch**(**touch**: <strong>[UITouch](UITouch.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Ask the delegate if a gesture recognizer should receive an object representing a touch. The default value is true.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **minimumPressDuration**: **[Float](../gravity/types.md)**
The minimum time (in seconds) that the mouse button must be held down in the view for the gesture to be recognized. The default value of this property is the same as the current double-click interval.

* **var** **numberOfTapsRequired**: **[Int](../gravity/types.md)**
The number of taps on the view required for the gesture to be recognized. The default number of taps is 0.

* **var** **numberOfTouchesRequired**: **[Int](../gravity/types.md)**
The number of fingers that must be pressed on the view for the gesture to be recognized. The default number of fingers is 1.

* **var** **allowableMovement**: **[Float](../gravity/types.md)**
The maximum movement of the mouse in the view before the gesture fails. The mouse must move by the specified amount along either axis for the gesture to fail. The distance is measured in points. The default value of this property is the same as the double-click distance.





