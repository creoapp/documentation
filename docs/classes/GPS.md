**super**: **[DataSet](DataSet.md)**

The GPS class is the central point for configuring the delivery of location and heading related events to your app. You use an instance of this class to establish the parameters that determine when location and heading events should be delivered and to start and stop the actual delivery of those events. You can also use a GPS object to retrieve the most recent location and heading data.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **NewValue**(**value**: **[Map](../gravity/maps.md)**)
Event raised when a new value becomes available. The value parameter is map.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **distanceFilter**: **[Float](../gravity/types.md)**
The minimum distance (measured in meters) a device must move horizontally before an update event is generated. This distance is measured relative to the previously delivered location. Use the value kCLDistanceFilterNone to be notified of all movements. The default value of this property is -1.0. This property is used only in conjunction with the standard location services and is not used when monitoring significant location changes.

* **var** **desiredAccuracy**: **[Float](../gravity/types.md)**
The desired location accuracy. The location service will try its best to achieve your desired accuracy. However, it is not guaranteed. To optimize power performance, be sure to specify an appropriate accuracy for your usage scenario (eg, use a large accuracy value when only a coarse location is needed). Use AccuracyBest to achieve the best possible accuracy. Use AccuracyBestForNavigation for navigation. The default value varies by platform.

* **var** **activityType**: **ActivityType**
The type of user activity associated with the location updates. The location manager uses the information in this property as a cue to determine when location updates may be automatically paused. Pausing updates gives the system the opportunity to save power in situations where the user's location is not likely to be changing. For example, if the activity type is AutomotiveNavigation and no location changes have occurred recently, the radios might be powered down until movement is detected again.



### Methods

* **func** **locationServicesEnabled**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether location services are enabled on the device.

* **func** **headingAvailable**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether the location manager is able to generate heading-related events. Heading data may not be available on all iOS-based devices.

* **func** **deferredLocationUpdatesAvailable**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether the device supports deferred location updates. Deferred location updates are a way for the location manager to avoid frequently waking up a background app to deliver location changes. Normally, when an app wants location updates in the background, the app must be woken up whenever a new event arrives. Waking up the app consumes power, which in some situations might be wasted if the app cannot do anything with the location information other than log it and go back to sleep anyway. Deferring location updates gives you the ability to wait until a time when your app can do something useful with the data and then process the updates all at once. Deferred location updates require the presence of GPS hardware and may not be supported on all iOS devices.

* **func** **significantLocationChangeMonitoringAvailable**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether significant location change tracking is available. This method indicates whether the device is able to report updates based on significant location changes only. This capability provides tremendous power savings for apps that want to track a user’s approximate location and do not need highly accurate position information.

* **func** **authorizationStatus**(): <strong><a href="#_enum_AuthorizationStatus">AuthorizationStatus</a></strong> 
Returns the app’s authorization status for using location services. The authorization status of a given app is managed by the system and determined by several factors. Apps must be explicitly authorized to use location services by the user and location services must themselves currently be enabled for the system. A request for user authorization is displayed automatically when your app first attempts to use location services.





### Enumeration

#### ActivityType
 * .AutomotiveNavigation
 * .Fitness
 * .Other
 * .OtherNavigation

#### AuthorizationStatus
 * .AuthorizedAlways
 * .AuthorizedWhenInUse
 * .Denied
 * .NotDetermined
 * .Restricted



