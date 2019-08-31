**super**: **[UISwipeGestureRecognizer](UISwipeGestureRecognizer.md)** (on iOS)

SwipeGesture is a concrete gesture recognizer that looks for swiping gestures in one or more directions. A swipe is a discrete gesture, and thus the associated action message is sent only once per gesture. SwipeGestureRecognizer recognizes a swipe when the specified number of touches (numberOfTouchesRequired) have moved mostly in an allowable direction (direction) far enough to be considered a swipe. Swipes can be slow or fast. A slow swipe requires high directional precision but a small distance; a fast swipe requires low directional precision but a large distance.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called when the object recognizes its gesture or, in some cases, a change in the gesture.

* **ShouldRecognizeSimultaneously**(**otherGesture**: **[UIGestureRecognizer](UIGestureRecognizer.md)**)<strong>: [Bool](../gravity/bool.md)</strong> 
Asks if two gesture recognizers should be allowed to recognize gestures simultaneously. This event is called when recognition of a gesture by either this gesture recognizer or the other gesture recognizer passed as the parameter would block the other gesture recognizer from recognizing its gesture. Note that returning <i>true</i> is guaranteed to allow simultaneous recognition; returning <i>false</i>, on the other hand, is not guaranteed to prevent simultaneous recognition because the other gesture recognizer's event may return <i>true</i>. The default value is <i>false</i>.

* **ShouldBegin**()<strong>: [Bool](../gravity/bool.md)</strong> 
Asks if a gesture recognizer should begin interpreting touches. This method is called when a gesture recognizer attempts to transition out of the GestureRecognizerState.Possible state. Returning <i>false</i> causes the gesture recognizer to transition to the GestureRecognizerState.Failed state. The default value is <i>true</i>.

* **ShouldReceiveTouch**(**touch**: **[UITouch](UITouch.md)**)<strong>: [Bool](../gravity/bool.md)</strong> 
Ask the delegate if a gesture recognizer should receive an object representing a touch. The default value is true.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **numberOfTouchesRequired**: **[Int](../gravity/int.md)**
The number of touches that must be present for the swipe gesture to be recognized. The default value is 1.

* **var** **direction**: **<a href="#_enum_SwipeGestureRecognizerDirection">SwipeGestureRecognizerDirection</a>**
The permitted direction of the swipe for this gesture recognizer. The default direction is SwipeGestureRecognizerDirection.Right.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





### Enums

<div id="_enum_SwipeGestureRecognizerDirection"></div>

#### SwipeGestureRecognizerDirection
 * .Down
 * .Left
 * .Right
 * .Up



