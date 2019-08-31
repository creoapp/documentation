**super**: **[UIView](UIView.md)** (on iOS)

Display map or satellite imagery from the windows and views of your custom apps.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **WillStart**()
Tells that the map view will start tracking the user's position.

* **DidFail**()
Tells that an attempt to locate the user’s position failed.

* **DidStop**()
Tells that map view stopped tracking the user’s location.

* **LocationDidChange**(**value**: **[Map](../gravity/map.md)**)
The location of the user was updated.

* **DidSelectAnnotation**(**annotationPoint**: **[MapPointAnnotation](MapPointAnnotation.md)**)
Raised when one of its annotation views was selected.

* **DidDeselectAnnotation**(**annotationPoint**: **[MapPointAnnotation](MapPointAnnotation.md)**)
Raised when one of its annotation views was deselected.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **address**: **[String](../gravity/string.md)**
A string describing the location you want to center the map to.

* **var** **latitude**: **[Float](../gravity/float.md)**
The latitude of the center point of the visible area.

* **var** **longitude**: **[Float](../gravity/float.md)**
The longitude of the center point of the map.

* **var** **mapType**: **MapType**
The type of data displayed by the map view.

* **var** **zoomValue**: **[Float](../gravity/float.md)**
The zoom value used to display the map.

* **var** **zoomEnabled**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether the user may use pinch gestures to zoom in and out of the map.

* **var** **scrollEnabled**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether the user may scroll around the map.

* **var** **pitchEnabled**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the map camera’s pitch information is used.

* **var** **rotateEnabled**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the map camera’s heading information is used.

* **var** **visibleMapRect**: **[Rect](Rect.md)**
The area currently displayed by the map view.

* **var** **showsPointsOfInterest**: **[Bool](../gravity/bool.md)**
A Boolean indicating whether the map displays point-of-interest information.

* **var** **showsBuildings**: **[Bool](../gravity/bool.md)**
A Boolean indicating whether the map displays extruded building information.

* **var** **showsUserLocation**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the map should try to display the user’s location.

* **var** **userLocationVisible**: **[Bool](../gravity/bool.md)**
A Boolean value indicating whether the device’s current location is visible in the map view. \(read-only\)

* **var** **userTrackingMode**: **MapUserTrackingMode**
Sets the mode used to track the user location.

* **var** **annotationVisibleRect**: **[Rect](Rect.md)**
The visible rectangle where annotation views are currently being displayed. \(read-only\)

* **var** **annotations**: **[List](../gravity/list.md)**
The complete list of annotations associated with the map. \(read-only\)

* **var** **selectedAnnotations**: **[List](../gravity/list.md)**
The annotations that are currently selected. Assigning a new array to this property selects only the first annotation in the array.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **addAnnotation**(**annotationPoint**: **[MapPointAnnotation](MapPointAnnotation.md)**)
Adds the specified annotation to the map view.

* **func** **removeAnnotation**(**annotationPoint**: **[MapPointAnnotation](MapPointAnnotation.md)**)
Removes the specified annotation object from the map view.

* **func** **annotationsInRect**(**regionRect**: **[Rect](Rect.md)**): <strong>[List](../gravity/list.md)</strong> 
Returns the annotation objects located in the specified map rectangle.

* **func** **addAnnotations**(**annotations**: **[List](../gravity/list.md)**)
Adds an array of annotation objects to the map view.

* **func** **showAnnotations**(**annotations**: **[List](../gravity/list.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Sets the visible region so that the map displays the specified annotations.

* **func** **removeAnnotations**(**annotations**: **[List](../gravity/list.md)**)
Removes an array of annotation objects from the map view.

* **func** **selectAnnotation**(**annotationPoint**: **[MapPointAnnotation](MapPointAnnotation.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Selects the specified annotation and displays a callout view for it.

* **func** **deselectAnnotation**(**annotationPoint**: **[MapPointAnnotation](MapPointAnnotation.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Deselects the specified annotation and hides its callout view.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control



* None

### Enumeration

<div name="_enum_MapType"></div>

#### MapType
 * .Hybrid
 * .HybridFlyover
 * .Satellite
 * .SatelliteFlyover
 * .Standard

<div name="_enum_MapUserTrackingMode"></div>

#### MapUserTrackingMode
 * .Follow
 * .FollowWithHeading
 * .None

<div name="_enum_AnimationOption"></div>

#### AnimationOption
 * .AllowAnimatedContent
 * .AllowUserInteraction
 * .Autoreverse
 * .BeginFromCurrentState
 * .CurveEaseIn
 * .CurveEaseInOut
 * .CurveEaseOut
 * .CurveLinear
 * .LayoutSubviews
 * .OverrideInheritedCurve
 * .OverrideInheritedDuration
 * .OverrideInheritedOptions
 * .Repeat
 * .ShowHideTransitionViews
 * .TransitionCrossDissolve
 * .TransitionCurlDown
 * .TransitionCurlUp
 * .TransitionFlipFromBottom
 * .TransitionFlipFromLeft
 * .TransitionFlipFromRight
 * .TransitionFlipFromTop
 * .TransitionNone



