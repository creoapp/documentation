**super**: **[Object](Object.md)**

Use a Device object to get information about the device such as assigned name, device model, operating-system name and version, battery state and device orientation.

### Events

* None

### Properties

* **var** **version**: **DeviceVersion**
Returns a value from the DeviceVersion enum identifying the type of device (for example iPhone7, iPhone7Plus, iPadPro12Dot9Inch2Gen, etc.). \(read-only\)

* **var** **versionName**: **[String](../gravity/types.md)**
Returns a string representation of the deviceVersion property. \(read-only\)

* **var** **size**: **DeviceSize**
Returns a value from the DeviceSize enum identifying the screen size of the device (for example Screen4inch, Screen4Dot7inch, etc.). To get a human readable string representation or the numeric diagonal size in inches you can use the conversion methods <i>sizeName</i> or <i>sizeInches</i>. \(read-only\)

* **var** **systemName**: **[String](../gravity/types.md)**
The name of the operating system running on the device. \(read-only\)

* **var** **systemVersion**: **[String](../gravity/types.md)**
The current version of the operating system. \(read-only\)

* **var** **systemMajorVersion**: **[Int](../gravity/types.md)**
The current major version of the operating system. For example in iOS 11.4.1 this value is 11. \(read-only\)

* **var** **systemMinorVersion**: **[Int](../gravity/types.md)**
The current minor version of the operating system. For example in iOS 11.4.1 this value is 4. \(read-only\)

* **var** **systemPatchVersion**: **[Int](../gravity/types.md)**
The current patch version of the operating system. For example in iOS 11.4.1 this value is 1. \(read-only\)

* **var** **name**: **[String](../gravity/types.md)**
The name identifying the device. \(read-only\)

* **var** **model**: **[String](../gravity/types.md)**
The model of the device. \(read-only\)

* **var** **orientation**: **DeviceOrientation**
The physical orientation of the device. \(read-only\)

* **var** **batteryLevel**: **[Float](../gravity/types.md)**
The battery charge level for the device.Battery level ranges from 0.0 (fully discharged) to 1.0 (100% charged). Before accessing this property, ensure that battery monitoring is enabled. If battery monitoring is not enabled, battery state is unknown and the value of this property is –1.0. \(read-only\)

* **var** **batteryMonitoringEnabled**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether battery monitoring is enabled (true) or not (false).

* **var** **batteryState**: **DeviceBatteryState**
The battery state for the device. If battery monitoring is not enabled, the value of this property is unknown

* **var** **language**: **[String](../gravity/types.md)**
Users choose a primary language when configuring a device. Use this property to obtain the current user's primary device language. \(read-only\)

* **var** **isPhone**: **[Bool](../gravity/types.md)**
Check if current device is an iPhone. \(read-only\)

* **var** **isPad**: **[Bool](../gravity/types.md)**
Check if current device is an iPad. \(read-only\)



### Methods

* **func** **sizeInches**(**size**: **<a href="#_enum_DeviceSize">DeviceSize</a>**): <strong>[Float](../gravity/types.md)</strong> 
Convert a value from the DeviceSize enum to the numeric value of the screen size (diagonal).

* **func** **sizeName**(**size**: **<a href="#_enum_DeviceSize">DeviceSize</a>**): <strong>[String](../gravity/types.md)</strong> 
Convert a value from the DeviceSize enum to its string representation.





### Enumeration

#### DeviceVersion
 * .Simulator
 * .Unknown
 * .iPad1
 * .iPad2
 * .iPad3
 * .iPad4
 * .iPad5
 * .iPadAir
 * .iPadAir2
 * .iPadMini
 * .iPadMini2
 * .iPadMini3
 * .iPadMini4
 * .iPadPro10Dot5Inch
 * .iPadPro12Dot9Inch
 * .iPadPro12Dot9Inch2Gen
 * .iPadPro9Dot7Inch
 * .iPhone4
 * .iPhone4S
 * .iPhone5
 * .iPhone5C
 * .iPhone5S
 * .iPhone6
 * .iPhone6Plus
 * .iPhone6S
 * .iPhone6SPlus
 * .iPhone7
 * .iPhone7Plus
 * .iPhone8
 * .iPhone8Plus
 * .iPhoneSE
 * .iPhoneX

#### DeviceSize
 * .Screen10Dot5inch
 * .Screen12Dot9inch
 * .Screen3Dot5inch
 * .Screen4Dot7inch
 * .Screen4inch
 * .Screen5Dot5inch
 * .Screen5Dot8inch
 * .Screen7Dot9inch
 * .Screen9Dot7inch
 * .Unknown

#### DeviceOrientation
 * .FaceDown
 * .FaceUp
 * .LandscapeLeft
 * .LandscapeRight
 * .Portrait
 * .PortraitUpsideDown
 * .Unknown

#### DeviceBatteryState
 * .Charging
 * .Full
 * .Unknown
 * .Unplugged



