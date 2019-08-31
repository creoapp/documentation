**super**: **[UIPinchGestureRecognizer](UIPinchGestureRecognizer.md)** (on iOS)

PinchGesture is a concrete gesture recognizer that looks for pinching gestures involving two touches. When the user moves the two fingers toward each other, the conventional meaning is zoom-out; when the user moves the two fingers away from each other, the conventional meaning is zoom-in. Pinching is a continuous gesture. The gesture begins (GestureRecognizerState.Began) when the two touches have moved enough to be considered a pinch gesture. The gesture changes (GestureRecognizerState.Changed) when a finger moves (with both fingers remaining pressed). The gesture ends (GestureRecognizerState.Ended) when both fingers lift from the view.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called when the object recognizes its gesture or, in some cases, a change in the gesture.

* **ShouldRecognizeSimultaneously**(**otherGesture**: **[UIGestureRecognizer](UIGestureRecognizer.md)**)-> <strong>[Bool](../gravity/bool.md)</strong> 
Asks if two gesture recognizers should be allowed to recognize gestures simultaneously. This event is called when recognition of a gesture by either this gesture recognizer or the other gesture recognizer passed as the parameter would block the other gesture recognizer from recognizing its gesture. Note that returning <i>true</i> is guaranteed to allow simultaneous recognition; returning <i>false</i>, on the other hand, is not guaranteed to prevent simultaneous recognition because the other gesture recognizer's event may return <i>true</i>. The default value is <i>false</i>.

* **ShouldBegin**()-> <strong>[Bool](../gravity/bool.md)</strong> 
Asks if a gesture recognizer should begin interpreting touches. This method is called when a gesture recognizer attempts to transition out of the GestureRecognizerState.Possible state. Returning <i>false</i> causes the gesture recognizer to transition to the GestureRecognizerState.Failed state. The default value is <i>true</i>.

* **ShouldReceiveTouch**(**touch**: **[UITouch](UITouch.md)**)-> <strong>[Bool](../gravity/bool.md)</strong> 
Ask the delegate if a gesture recognizer should receive an object representing a touch. The default value is true.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **scale**: **[Float](../gravity/float.md)**
The scale factor relative to the points of the two touches in screen coordinates. The scale value is an absolute value that varies over time. It is not the delta value from the last time that the scale was reported. Apply the scale value to the state of the view when the gesture is first recognized—do not concatenate the value each time the handler is called.

* **var** **velocity**: **[Float](../gravity/float.md)**
The velocity of the pinch in scale factor per second. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





