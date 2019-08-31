**super**: **[Object](../gravity/object.md)**

This class is reserved and cannot be directly instantiated.

This is the base class for concrete gesture recognizers. A gesture-recognizer decouples the logic for recognizing a sequence of touches (or other input) and acting on that recognition. When one of these objects recognizes a common gesture or, in some cases, a change in the gesture, it sends an action event. The concrete subclasses of GestureRecognizer are the following: <ul><li><a href="./TapGesture.html">TapGesture</a></li><li><a href="./PinchGesture.html">PinchGesture</a></li><li><a href="./RotationGesture.html">RotationGesture</a></li><li><a href="./SwipeGesture.html">SwipeGesture</a></li><li><a href="./PanGesture.html">PanGesture</a></li><li><a href="./LongPressGesture.html">LongPressGesture</a></li></ul>

### Events

* **Action**()
This event is called when the object recognizes its gesture or, in some cases, a change in the gesture.

* **ShouldRecognizeSimultaneously**(**otherGesture**: **[UIGestureRecognizer](UIGestureRecognizer.md)**)<strong>: [Bool](../gravity/bool.md)</strong> 
Asks if two gesture recognizers should be allowed to recognize gestures simultaneously. This event is called when recognition of a gesture by either this gesture recognizer or the other gesture recognizer passed as the parameter would block the other gesture recognizer from recognizing its gesture. Note that returning <i>true</i> is guaranteed to allow simultaneous recognition; returning <i>false</i>, on the other hand, is not guaranteed to prevent simultaneous recognition because the other gesture recognizer's event may return <i>true</i>. The default value is <i>false</i>.

* **ShouldBegin**()<strong>: [Bool](../gravity/bool.md)</strong> 
Asks if a gesture recognizer should begin interpreting touches. This method is called when a gesture recognizer attempts to transition out of the GestureRecognizerState.Possible state. Returning <i>false</i> causes the gesture recognizer to transition to the GestureRecognizerState.Failed state. The default value is <i>true</i>.

* **ShouldReceiveTouch**(**touch**: **[UITouch](UITouch.md)**)<strong>: [Bool](../gravity/bool.md)</strong> 
Ask the delegate if a gesture recognizer should receive an object representing a touch. The default value is true.



### Properties

* **var** **enabled**: **[Bool](../gravity/bool.md)**
A Boolean property that indicates whether the gesture recognizer is enabled. Disables a gesture recognizers so it does not receive touches.

* **var** **state**: **<a href="#_enum_GestureRecognizerState">GestureRecognizerState</a>**
The current state of the gesture recognizer. Some of these states are not applicable to discrete gestures. \(read-only\)

* **var** **numberOfTouches**: **[Int](../gravity/int.md)**
Returns the number of touches involved in the gesture represented by the receiver. \(read-only\)

* **var** **view**: **[UIView](UIView.md)**
The view the gesture recognizer is attached to. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **locationInView**(**view**: **[UIView](UIView.md)**)<strong>: [Point](Point.md)</strong> 
Returns a generic single-point location for the gesture, usually the centroid of the touches involved, in the coordinate system of the given view.

* **func** **locationOfTouch**(**touchIndex**: **[Int](../gravity/int.md)**, **view**: **[UIView](UIView.md)**)<strong>: [Point](Point.md)</strong> 
Returns the location of one of the gesture’s touches in the local coordinate system of a given view.

* **func** **requireToFail**(**otherGestureRecognizer**: **[UIGestureRecognizer](UIGestureRecognizer.md)**)
This method creates a relationship with another gesture recognizer that delays the receiver’s transition out of GestureRecognizerState.Possible. The state that the receiver transitions to depends on what happens with otherGestureRecognizer: If otherGestureRecognizer transitions to UIGestureRecognizer.State.failed, the receiver transitions to its normal next state. If otherGestureRecognizer transitions to recognized or GestureRecognizerState.Began, the receiver transitions to GestureRecognizerState.Failed.  An example where this method might be called is when you want a single-tap gesture require that a double-tap gesture fail.





### Enums

<div id="_enum_GestureRecognizerState"></div>

#### GestureRecognizerState
 * .Began
 * .Cancelled
 * .Changed
 * .Ended
 * .Failed
 * .Possible



