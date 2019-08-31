**super**: **[UIImageView](UIImageView.md)** (on iOS)

An ImageView object displays a single image or a sequence of animated images in your interface. Image views let you efficiently draw any image that can be specified using a UIImage object. For example, you can use this class to display the contents of many standard image files, such as JPEG and PNG files. You can configure image views programmatically or in your storyboard file and change the images they display at runtime. For animated images, you can also use the methods of this class to start and stop the animation and specify other animation parameters.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **TouchesBegan**(**touches**: **[Object](../gravity/object.md)**)-> <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when one or more new touches occurred in this view and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesMoved**(**touches**: **[Object](../gravity/object.md)**, **touchInside**: **[Bool](../gravity/bool.md)**)-> <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when the location or force of a touch changes and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesEnded**(**touches**: **[Object](../gravity/object.md)**, **touchInside**: **[Bool](../gravity/bool.md)**)-> <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when one or more fingers are raised and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **TouchesCancelled**(**touches**: **[Object](../gravity/object.md)**)-> <strong>[Bool](../gravity/bool.md)</strong> 
This event is called when the sysyem receives a system interruption (such as a system alert) requiring cancellation of the touch sequence and the userInteractionEnabled property is enabled. Return "true" if you want to consume the event and not forward it to the next responder, return "no" to forward any events that you do not handle yourself.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **image**: **[Image](Image.md)**
The image displayed in the image view.

* **var** **renderedImage**: **[Image](Image.md)**
The rendered image as it appears in the ImageView, resized according to its settings. \(read-only\)

* **var** **highlightedImage**: **[Image](Image.md)**
The highlighted image displayed in the image view.

* **var** **animationImages**: **[List](../gravity/list.md)**
An array of Image objects to use for an animation.

* **var** **highlightedAnimationImages**: **[List](../gravity/list.md)**
An array of Image objects to use for an animation when the view is highlighted.

* **var** **animationDuration**: **[Float](../gravity/float.md)**
The amount of time it takes to go through one cycle of the images. The time duration is measured in seconds. The default value of this property is 0.0, which causes the image view to use a duration equal to the number of images multiplied by 1/30th of a second. Thus, if you had 30 images, the duration would be 1 second.

* **var** **animationRepeatCount**: **[Int](../gravity/int.md)**
Specifies the number of times to repeat the animation. The default value is 0, which specifies to repeat the animation indefinitely.

* **var** **highlighted**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether the image is highlighted.

* **var** **url**: **[String](../gravity/string.md)**
Asynchronously downloads an image from the specified URL (both local and remote urls work), and sets it once the request is finished. Any previous image request for the receiver will be cancelled. If the image is cached locally, the image is set immediately, otherwise the specified placeholder image will be set immediately, and then the remote image will be set once the request is finished. By default, URL requests have a `Accept` header field value of "image / *".

* **var** **contentMode**: **ContentMode**
Options to specify how a view adjusts its content when its size changes.

* **var** **imagesRenderingMode**: **ImageRenderingMode**
Options to specify how a view adjusts its content when its size changes.

* **var** **filters**: **[List](../gravity/list.md)**
A list a ImageFilters to apply to the image or highlighted image of the ImageView.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **startAnimating**()
Starts animating the images in the receiver.

* **func** **stopAnimating**()
Stops animating the images in the receiver.

* **func** **isAnimating**()-> <strong>[Bool](../gravity/bool.md)</strong> 
Returns a Boolean value indicating whether the animation is running.

* **func** **applyFilters**()
Call this method to commit changes in properties of a the configured filters.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_ContentMode"></div>

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

<div id="_enum_ImageRenderingMode"></div>

#### ImageRenderingMode
 * .AlwaysOriginal
 * .AlwaysTemplate
 * .Automatic

<div id="_enum_AnimationOption"></div>

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



