**super**: **[UIPanGestureRecognizer](UIPanGestureRecognizer.md)** (on iOS)

PanGesture is a concrete gesture recognizer that looks for panning (dragging) gestures. The user must be pressing one or more fingers on a view while they pan it. Clients implementing the action method for this gesture recognizer can ask it for the current translation and velocity of the gesture. A panning gesture is continuous. It begins (GestureRecognizerState.Began) when the minimum number of fingers allowed (minimumNumberOfTouches) has moved enough to be considered a pan. It changes (GestureRecognizerState.Changed) when a finger moves while at least the minimum number of fingers are pressed down. It ends (GestureRecognizerState.Ended) when all fingers are lifted.

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

* **var** **maximumNumberOfTouches**: **[Int](../gravity/types.md)**
The maximum number of fingers that can be touching the view for this gesture to be recognized.

* **var** **minimumNumberOfTouches**: **[Int](../gravity/types.md)**
The minimum number of fingers that can be touching the view for this gesture to be recognized. The default value is 1.



### Methods

* **func** **translationInView**(**view**: **[Object](../gravity/types.md)**): <strong>[Point](point.md)</strong> 
The translation of the pan gesture in the coordinate system of the specified view. The x and y values report the total translation over time.

* **func** **setTranslationInView**(**translation**: **[Point](point.md)**, **view**: **[Object](../gravity/types.md)**)
Sets the translation value in the coordinate system of the specified view. Changing the translation value resets the velocity of the pan.

* **func** **velocityInView**(**view**: **[Object](../gravity/types.md)**): <strong>[Point](point.md)</strong> 
The velocity of the pan gesture, expressed in points per second, in the coordinate system of the specified view. The velocity is broken into horizontal and vertical components.





