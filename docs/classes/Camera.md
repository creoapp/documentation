**super**: [UIView](UIView.md) on iOS

A Camera object represents a physical capture device and the properties associated with that device. You use a capture device to configure the properties of the underlying hardware. A capture device also provides input data, such as audio or video.

#### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **NewImage**(**image**: <strong>[Image](image.md)</strong>)
This event is triggered when a new still picture is available.

* **NewVideo**(**videoPath**: <strong>[String](../gravity/types.md)</strong>)
This event is triggered when a new recordered movie is available.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



#### Properties

* **var** **position**: **CameraPosition**
Current position of a capture device. \(read-only\)

* **var** **whiteBalance**: **[Int](../gravity/types.md)**
White balance mode.

* **var** **mirror**: **[Int](../gravity/types.md)**
Camera mirror mode.

* **var** **flash**: **[Int](../gravity/types.md)**
Current flash mode of a capture device. \(read-only\)

* **var** **recording**: **[Bool](../gravity/types.md)**
Boolean value to indicate if the camera is recording a video at the current moment. \(read-only\)

* **var** **videoEnabled**: **[Bool](../gravity/types.md)**
Check if video mode is enabled in the capture device.

* **var** **cropImageAsSeen**: **[Bool](../gravity/types.md)**
If set to true then captured Image is cropped usign the exact View size.

* **var** **zoomingEnabled**: **[Bool](../gravity/types.md)**
Boolean value to indicate if zooming is enabled.

* **var** **fixOrientationAfterCapture**: **[Bool](../gravity/types.md)**
Boolean value to indicate if the image must be rasterized according to device orientation.

* **var** **useDeviceOrientation**: **[Bool](../gravity/types.md)**
Boolean value to indicate if device orientation should be taken into account.

* **var** **isFlashAvailable**: **[Bool](../gravity/types.md)**
Checks if flash is available.

* **var** **isTorchAvailable**: **[Bool](../gravity/types.md)**
Checks if torch is available.

* **var** **isFrontCameraAvailable**: **[Bool](../gravity/types.md)**
Checks if the front camera is available.

* **var** **isRearCameraAvailable**: **[Bool](../gravity/types.md)**
Checks if the rear camera is available.

* **var** **autoFocusOnTap**: **[Bool](../gravity/types.md)**
Boolean value to indicate if zooming is enabled.

* **var** **autoExposureOnTap**: **[Bool](../gravity/types.md)**
Boolean value to indicate if zooming is enabled.

* **var** **maxScale**: **[Float](../gravity/types.md)**
Maximum scaling factor.



#### Methods

* **func** **capture**()
Initiates a still image capture action.

* **func** **togglePosition**()
Toggle the position of a capture device.

* **func** **toggleFlashMode**(): <strong><a href="#_enum_CameraFlashMode">CameraFlashMode</a></strong> 
Toggle the flash mode of the capture device. Returns the new flash mode.

* **func** **startRecording**()
Start recording a video.

* **func** **stopRecording**()
Stop recording a video.

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





#### Enumeration

#### CameraPosition
 * .Front
 * .Rear
<br><br>#### CameraFlashMode
 * .Auto
 * .Off
 * .On
<br><br>#### AnimationOption
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
<br><br>

