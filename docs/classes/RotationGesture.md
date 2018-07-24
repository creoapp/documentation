**super**: [UIRotationGestureRecognizer](UIRotationGestureRecognizer.md) on iOS

RotationGesture is a concrete gesture recognizer that looks for rotation gestures involving two touches. When the user moves the fingers opposite each other in a circular motion, the underlying view should rotate in a corresponding direction and speed. Rotation is a continuous gesture. It begins when two touches have moved enough to be considered a rotation. The gesture changes when a finger moves while the two fingers are down. It ends when both fingers have lifted. At each stage in the gesture, the gesture recognizer sends its action message.

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

* **var** **rotation**: **[Float](../gravity/types.md)**
The rotation of the gesture in degrees. You may set the rotation value to an arbitrary value; however, setting the rotation resets the velocity. The rotation value is a single value that varies over time. It is not the delta value from the last time that the rotation was reported. Apply the rotation value to the state of the view when the gesture is first recognized—do not concatenate the value each time the handler is called.

* **var** **velocity**: **[Float](../gravity/types.md)**
The velocity of the rotation gesture in degrees per second. \(read-only\)





