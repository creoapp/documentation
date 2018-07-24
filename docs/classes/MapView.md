**super**: **[UIView](UIView.md)** (on iOS)

Display map or satellite imagery from the windows and views of your custom apps.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillStart**()
Tells that the map view will start tracking the user's position.

* **DidFail**()
Tells that an attempt to locate the user’s position failed.

* **DidStop**()
Tells that map view stopped tracking the user’s location.

* **LocationDidChange**(**value**: **[Map](../gravity/maps.md)**)
The location of the user was updated.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **address**: **[String](../gravity/types.md)**
A string describing the location you want to center the map to.

* **var** **latitude**: **[Float](../gravity/types.md)**
The latitude of the center point of the visible area.

* **var** **longitude**: **[Float](../gravity/types.md)**
The longitude of the center point of the map.

* **var** **mapType**: **MapType**
The type of data displayed by the map view.

* **var** **zoomEnabled**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether the user may use pinch gestures to zoom in and out of the map.

* **var** **scrollEnabled**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether the user may scroll around the map.

* **var** **pitchEnabled**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the map camera’s pitch information is used.

* **var** **rotateEnabled**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the map camera’s heading information is used.

* **var** **visibleMapRect**: **[Rect](rect.md)**
The area currently displayed by the map view.

* **var** **showsPointsOfInterest**: **[Bool](../gravity/types.md)**
A Boolean indicating whether the map displays point-of-interest information.

* **var** **showsBuildings**: **[Bool](../gravity/types.md)**
A Boolean indicating whether the map displays extruded building information.

* **var** **showsUserLocation**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the map should try to display the user’s location.

* **var** **userLocationVisible**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the device’s current location is visible in the map view. \(read-only\)

* **var** **userTrackingMode**: **MapUserTrackingMode**
Sets the mode used to track the user location.



### Methods

* **func** **addAnnotation**(**annotationPoint**: **[MapPointAnnotation](MapPointAnnotation.md)**)
Adds the specified annotation to the map view.

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closures.md)**, **completion**: **[Closure](../gravity/closures.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### MapType
 * .Hybrid
 * .HybridFlyover
 * .Satellite
 * .SatelliteFlyover
 * .Standard

#### MapUserTrackingMode
 * .Follow
 * .FollowWithHeading
 * .None

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



