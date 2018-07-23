**super**: [UIImageView](UIImageView.md) on iOS

An ImageView object displays a single image or a sequence of animated images in your interface. Image views let you efficiently draw any image that can be specified using a UIImage object. For example, you can use this class to display the contents of many standard image files, such as JPEG and PNG files. You can configure image views programmatically or in your storyboard file and change the images they display at runtime. For animated images, you can also use the methods of this class to start and stop the animation and specify other animation parameters.

#### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **TouchesBegan**(**touches**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when one or more new touches occurred in this view and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesMoved**(**touches**: <strong>[Object](../gravity/types.md)</strong>, **touchInside**: <strong>[Bool](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the location or force of a touch changes and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesEnded**(**touches**: <strong>[Object](../gravity/types.md)</strong>, **touchInside**: <strong>[Bool](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when one or more fingers are raised and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesCancelled**(**touches**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when the sysyem receives a system interruption (such as a system alert) requiring cancellation of the touch sequence and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



#### Properties

* **var** **image**: **[Image](image.md)**
The image displayed in the image view.

* **var** **highlightedImage**: **[Image](image.md)**
The highlighted image displayed in the image view.

* **var** **animationImages**: **[List](../gravity/lists.md)**
An array of Image objects to use for an animation.

* **var** **highlightedAnimationImages**: **[List](../gravity/lists.md)**
An array of Image objects to use for an animation when the view is highlighted.

* **var** **animationDuration**: **[Float](../gravity/types.md)**
The amount of time it takes to go through one cycle of the images. The time duration is measured in seconds. The default value of this property is 0.0, which causes the image view to use a duration equal to the number of images multiplied by 1/30th of a second. Thus, if you had 30 images, the duration would be 1 second.

* **var** **animationRepeatCount**: **[Int](../gravity/types.md)**
Specifies the number of times to repeat the animation. The default value is 0, which specifies to repeat the animation indefinitely.

* **var** **highlighted**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether the image is highlighted.

* **var** **url**: **[String](../gravity/types.md)**
Asynchronously downloads an image from the specified URL (both local and remote urls work), and sets it once the request is finished. Any previous image request for the receiver will be cancelled. If the image is cached locally, the image is set immediately, otherwise the specified placeholder image will be set immediately, and then the remote image will be set once the request is finished. By default, URL requests have a `Accept` header field value of "image / *".

* **var** **contentMode**: **ContentMode**
Options to specify how a view adjusts its content when its size changes.

* **var** **imagesRenderingMode**: **[Int](../gravity/types.md)**
Options to specify how a view adjusts its content when its size changes.



#### Methods

* **func** **startAnimating**()
Starts animating the images in the receiver.

* **func** **stopAnimating**()
Stops animating the images in the receiver.

* **func** **isAnimating**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether the animation is running.

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





#### Enumeration

#### ContentMode
 * .Bottom
 * .BottomLeft
 * .BottomRight
 * .Center
 * .Left
 * .Redraw
 * .Right
 * .ScaleAspectFill
 * .ScaleAspectFit
 * .ScaleToFill
 * .Top
 * .TopLeft
 * .TopRight
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

