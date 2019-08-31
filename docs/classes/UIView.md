**super**: **[UIResponder](UIResponder.md)** (on iOS)

This class is reserved and cannot be directly instantiated.



### Events

* None

### Properties

* **var** **rotationAngle**: **[Float](../gravity/float.md)**
Set the transform applied to the view with an affine transformation matrix constructed from the provided rotation value.

* **var** **backgroundColor**: **[Color](Color.md)**
The view’s background color.

* **var** **backgroundObject**: **[Object](../gravity/object.md)**
The view’s background color or gradient.

* **var** **borderWidth**: **[Float](../gravity/float.md)**
The width of the view's border. When this value is greater than 0.0, the layer draws a border using the current borderColor value. The border is drawn inset from the receiver’s bounds by the value specified in this property. It is composited above the receiver’s contents and sublayers and includes the effects of the cornerRadius property.

* **var** **borderColor**: **[Color](Color.md)**
The color of the view’s border.

* **var** **cornerRadius**: **[Float](../gravity/float.md)**
The radius to use when drawing rounded corners for the view’s background. Setting the radius to a value greater than 0.0 causes the view to begin drawing rounded corners on its background.

* **var** **hidden**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether the view is hidden. A hidden view disappears from its window and does not receive input events. It remains in its superview’s list of subviews, however, and participates in autoresizing as usual. Hiding a view with subviews has the effect of hiding those subviews and any view descendants they might have. This effect is implicit and does not alter the hidden state of the receiver’s descendants.

* **var** **alpha**: **[Float](../gravity/float.md)**
The view’s alpha value. The value of this property is a floating-point number in the range 0.0 to 1.0, where 0.0 represents totally transparent and 1.0 represents totally opaque. This value affects only the current view and does not affect any of its embedded subviews.

* **var** **opaque**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether the view is opaque. An opaque view is expected to fill its bounds with entirely opaque content—that is, the content should have an alpha value of 1.0. If the view is opaque and either does not fill its bounds or contains wholly or partially transparent content, the results are unpredictable. You should always set the value of this property to false if the view is fully or partially transparent.

* **var** **tintColor**: **[Color](Color.md)**
The first nondefault tint color value in the view’s hierarchy, ascending from and starting with the view itself. If the system cannot find a nondefault color in the hierarchy, this property’s value is a system-defined color instead.

* **var** **bounds**: **[Rect](Rect.md)**
The bounds rectangle, which describes the view’s location and size in its own coordinate system. On the screen, the bounds rectangle represents the same visible portion of the view as its frame rectangle. By default, the origin of the bounds rectangle is set to (0, 0) but you can change this value to display different portions of the view. The size of the bounds rectangle is coupled to the size of the frame rectangle, so that changes to one affect the other. Changing the bounds size grows or shrinks the view relative to its center point. The coordinates of the bounds rectangle are always specified in points.

* **var** **frame**: **[Rect](Rect.md)**
The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

* **var** **userInteractionEnabled**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether user events are ignored by the view and by its subviews.

* **var** **shadowColor**: **[Color](Color.md)**
The color of the view's shadow.

* **var** **shadowOffset**: **[Size](Size.md)**
The offset (in points) of the view's shadow.

* **var** **shadowOpacity**: **[Float](../gravity/float.md)**
The opacity of the view's shadow.

* **var** **shadowRadius**: **[Float](../gravity/float.md)**
The blur radius (in points) used to render the view's shadow

* **var** **subviews**: **[List](../gravity/list.md)**
The array of subviews. \(read-only\)

* **var** **autoresizingMask**: **Autoresizing**
An integer bit mask that determines how the receiver resizes itself when its superview’s bounds change.

* **var** **flex**: **[Flex](Flex.md)**
FlexBox layout. \(read-only\)

* **var** **clipsToBounds**: **[Bool](../gravity/bool.md)**
Clip content to bounds.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **refresh**()
Notify the system that your view’s contents need to be redrawn. This method makes a note of the request and returns immediately. The view is not actually redrawn until the next drawing cycle, at which point all invalidated views are updated.

* **func** **addGestureRecognizer**(**gestureRecognizer**: **[UIGestureRecognizer](UIGestureRecognizer.md)**)
Attaches a gesture recognizer to the view.

* **func** **removeGestureRecognizer**(**gestureRecognizer**: **[UIGestureRecognizer](UIGestureRecognizer.md)**)
Detaches a gesture recognizer from the view.

* **func** **addSubview**(**view**: **[UIView](UIView.md)**)
Adds a view to the end of the list of subviews.

* **func** **removeFromSuperview**()
Unlinks the view from its superview and its window, and removes it from the responder chain.

* **func** **insertSubview**(**view**: **[UIView](UIView.md)**, **index**: **[Int](../gravity/int.md)**)
Inserts a subview at the specified index.

* **func** **convertRectTo**(**rect**: **[Rect](Rect.md)**, **view**: **[UIView](UIView.md)**): <strong>[Rect](Rect.md)</strong> 
Converts a rectangle from the view's coordinate system to that of another view.

* **func** **convertRectFrom**(**rect**: **[Rect](Rect.md)**, **view**: **[UIView](UIView.md)**): <strong>[Rect](Rect.md)</strong> 
Converts a rectangle from the coordinate system of another view to that of the view.

* **func** **convertPointTo**(**point**: **[Point](Point.md)**, **view**: **[UIView](UIView.md)**): <strong>[Point](Point.md)</strong> 
Converts a point from the view's coordinate system to that of another view.

* **func** **convertPointFrom**(**point**: **[Point](Point.md)**, **view**: **[UIView](UIView.md)**): <strong>[Point](Point.md)</strong> 
Converts a point from the coordinate system of another view to that of the view.

* **func** **hitTest**(**point**: **[Point](Point.md)**): <strong>[UIView](UIView.md)</strong> 
.



* None

### Enumeration

<div name="_enum_Autoresizing"></div>

#### Autoresizing
 * .FlexibleBottomMargin
 * .FlexibleHeight
 * .FlexibleLeftMargin
 * .FlexibleRightMargin
 * .FlexibleTopMargin
 * .FlexibleWidth
 * .None



