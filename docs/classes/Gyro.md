**super**: **[BaseDataSet](BaseDataSet.md)**

The Gyro object is the gateway to the motion services provided by OS. These services provide an app with accelerometer data, rotation rate data, magnetometer data, altitude related data, pedestrian related data, activity type data and other device motion data such as attitude. These types of data originate with a device’s accelerometers and (on some models) its magnetometer, gyroscope and barometer.

Important: An app should create only a single instance of the Gyro class. Multiple instances of this class can affect the rate at which data is received from the accelerometer and gyroscope.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: **[Object](../gravity/types.md)**)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **deviceMotionActive**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether the app is receiving updates from the device-motion service. \(read-only\)

* **var** **deviceMotionAvailable**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether the device-motion service is available on the device. \(read-only\)

* **var** **accelerometerActive**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether accelerometer updates are currently happening. \(read-only\)

* **var** **accelerometerAvailable**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether an accelerometer is available on the device. \(read-only\)

* **var** **gyroActive**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether gyroscope updates are currently happening. \(read-only\)

* **var** **gyroAvailable**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether a gyroscope is available on the device. \(read-only\)

* **var** **magnetometerActive**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether magnetometer updates are currently happening. \(read-only\)

* **var** **magnetometerAvailable**: **[Bool](../gravity/types.md)**
A Boolean value that indicates whether a magnetometer is available on the device. \(read-only\)

* **var** **isRelativeAltitudeAvailable**: **[Bool](../gravity/types.md)**
Returns a Boolean value indicating whether the current device supports generating data for relative altitude changes. \(read-only\)

* **var** **isDistanceAvailable**: **[Bool](../gravity/types.md)**
Returns a Boolean value indicating whether distance estimation is available on the current device. Distance estimation indicates the ability to use step information to supply the approximate distance traveled by the user. This capability is not supported on all devices. \(read-only\)

* **var** **isFloorCountingAvailable**: **[Bool](../gravity/types.md)**
Returns a Boolean value indicating whether floor counting is available on the current device. Floor counting indicates the ability to count the number of floors the user walks up or down using stairs. This capability is not supported on all devices. \(read-only\)

* **var** **isStepCountingAvailable**: **[Bool](../gravity/types.md)**
Returns a Boolean value indicating whether step counting is available on the current device. \(read-only\)

* **var** **isActivityAvailable**: **[Bool](../gravity/types.md)**
Returns a Boolean indicating whether motion data is available on the current device. \(read-only\)

* **var** **showsDeviceMovementDisplay**: **[Bool](../gravity/types.md)**
Returns a Boolean indicating whether motion data is available on the current device. Motion data is not available on all iOS devices. Use this method to determine if support is available on the current device.

* **var** **objectName**: **[String](../gravity/types.md)**
The name of the object.





