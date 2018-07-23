# Location

**super**: [Object](Object.md)

(null)

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).

</ul>

### Properties

* **var** **latitude**: **[Float](../gravity/types.md)**
The latitude in degrees. \(read-only\)

* **var** **longitude**: **[Float](../gravity/types.md)**
The longitude in degrees. \(read-only\)

* **var** **altitude**: **[Float](../gravity/types.md)**
The altitude measured in meters. \(read-only\)

* **var** **horizontalAccuracy**: **[Float](../gravity/types.md)**
The radius of uncertainty for the location, measured in meters. The location’s latitude and longitude identify the center of the circle, and this value indicates the radius of that circle. A negative value indicates that the location’s latitude and longitude are invalid. \(read-only\)

* **var** **verticalAccuracy**: **[Float](../gravity/types.md)**
The accuracy of the altitude value in meters. The value in the altitude property could be plus or minus the value indicated by this property. A negative value indicates that the altitude value is invalid. \(read-only\)

* **var** **course**: **[Float](../gravity/types.md)**
The direction in which the device is traveling. Course values are measured in degrees starting at due north and continuing clockwise around the compass. Thus, north is 0 degrees, east is 90 degrees, south is 180 degrees, and so on. Course values may not be available on all devices. A negative value indicates that the direction is invalid. \(read-only\)

* **var** **timestamp**: **[Date](date.md)**
The time at which this location was determined. \(read-only\)

* **var** **floor**: **[Int](../gravity/types.md)**
The logical floor of the building in which the user is located. \(read-only\)

</ul>

### Initializers

* **func** **Location**(**latitude**: <strong>[Float](../gravity/types.md)</strong>, **longitude**: <strong>[Float](../gravity/types.md)</strong>)
Description not yet ready.

* **func** **Location**(**latitude**: <strong>[Float](../gravity/types.md)</strong>, **longitude**: <strong>[Float](../gravity/types.md)</strong>, **altitude**: <strong>[Float](../gravity/types.md)</strong>, **horizontalAccuracy**: <strong>[Float](../gravity/types.md)</strong>, **verticalAccuracy**: <strong>[Float](../gravity/types.md)</strong>, **timestamp**: <strong>[Date](date.md)</strong>)
Description not yet ready.

</ul>

### Methods

* **func** **distanceFromLocation**(**location**: <strong>[Location](Location.md)</strong>): <strong>[Float](../gravity/types.md)</strong> 
Returns the distance (in meters) from the receiver’s location to the specified location. This method measures the distance between the two locations by tracing a line between them that follows the curvature of the Earth. The resulting arc is a smooth curve and does not take into account specific altitude changes between the two locations.

</ul>

</ul>

