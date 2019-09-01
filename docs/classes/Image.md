**super**: **[Object](../gravity/object.md)**

A Image object manages image data in your app. You use image objects to represent image data of all kinds, and the Image class is capable of managing data for all image formats supported by the underlying platform. Image objects are immutable, so you always create them from existing image data, such as an image file on disk or programmatically created image data. An image object may contain a single image or a sequence of images you intend to use in an animation. Although image objects support all platform-native image formats, it is recommended that you use PNG or JPEG files for most images in your app. Image objects are optimized for reading and displaying both formats, and those formats offer better performance than most other image formats. Because the PNG format is lossless, it is especially recommended for the images you use in your app’s interface.



### Properties

* **var** **size**: **[Size](Size.md)**
The logical dimensions of the image, measured in points. Multiply the size values by the value in the scale property to get the pixel dimensions of the image. \(read-only\)

* **var** **scale**: **[Float](../gravity/float.md)**
The scale factor of the image. If you multiply the logical size of the image (stored in the size property) by the value in this property, you get the dimensions of the image in pixels. \(read-only\)

* **var** **capInsets**: **[EdgeInsets](EdgeInsets.md)**
The end-cap insets. End caps specify the portion of an image that should not be resized when an image is stretched. This technique is used to implement buttons and other resizable image-based interface elements. When a button with end caps is resized, the resizing occurs only in the middle of the button, in the region between the end caps. The end caps themselves keep their original size and appearance.

This property specifies the sizes of all four end caps. The middle (stretchable) portion consists of all the pixels that are not included in the end caps. These pixels are tiled, left-to-right, top-to-bottom to fill the remaining space. \(read-only\)

* **var** **resizingMode**: **<a href="#_enum_ImageResizingMode">ImageResizingMode</a>**
The resizing mode of the image. \(read-only\)

* **var** **renderingMode**: **<a href="#_enum_ImageRenderingMode">ImageRenderingMode</a>**
Determines how an image is rendered. \(read-only\)

* **var** **RGBBuffer**: **[RGBBuffer](RGBBuffer.md)**
Creates a RGBBuffer for direct pixel inspection and manipulation. This is a costly operation that should not be performed in a loop. \(read-only\)

* **var** **imageOrientation**: **<a href="#_enum_ImageOrientation">ImageOrientation</a>**
Image orientation affects the way the image data is displayed when drawn. By default, images are displayed in the “up” orientation. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **open**(**srcfile**: **[Object](../gravity/object.md)**)<strong>: [Object](../gravity/object.md)</strong> 
Initializes and returns the image object with the content of the source file. The source file can be an URL or a <a href="File.html">File</a> object.



### Constructors

* **func** **Image**(**name**: **[String](../gravity/string.md)**)
Initializes and returns the image object with the specified name.

* **func** **Image**(**data**: **[Data](Data.md)**, **scale**: **[Float](../gravity/float.md)**)
Initializes and returns the image object with the specified data and scale factor. 



### Methods

* **func** **resizableImageWithCapInsets**(**capInsets**: **[EdgeInsets](EdgeInsets.md)**, **resizingMode**: **<a href="#_enum_ImageResizingMode">ImageResizingMode</a>**)<strong>: [Image](Image.md)</strong> 
Creates and returns a new image object with the specified cap insets and options.

* **func** **PNGRepresentation**()<strong>: [Data](Data.md)</strong> 
Returns the data for the specified image in PNG format.

* **func** **JPEGRepresentation**(**compressionQuality**: **[Float](../gravity/float.md)**)<strong>: [Data](Data.md)</strong> 
Returns the data for the specified image in JPEG format using the specified compression quality.

* **func** **scaleImageToFillSize**(**size**: **[Size](Size.md)**)<strong>: [Image](Image.md)</strong> 
Returns a scaled version of the image that fill the specified size, preserving the aspect ratio of the original image (as "aspect fill")

* **func** **scaleImageToFitSize**(**size**: **[Size](Size.md)**)<strong>: [Image](Image.md)</strong> 
Returns a scaled version of the image that fit into the specified size, preserving the aspect ratio of the original image (as "aspect fit")

* **func** **imageWithRenderingMode**(**renderingMode**: **<a href="#_enum_ImageRenderingMode">ImageRenderingMode</a>**)<strong>: [Image](Image.md)</strong> 
Creates and returns a new image object with the specified rendering mode.

* **func** **imageWithFilters**(**filters**: **[List](../gravity/list.md)**, **completionClosure**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completionClosure (image: Image)" data-content="The completionClosure closure, if set, is executed in a background thread so the UI stays responsive and, when the image is ready, it is passed as the only parameter of the closure.">Closure</a> = null**, **rectToRender**: **[Rect](Rect.md) = null**)<strong>: [Image](Image.md)</strong> 
Applies the list of filters to the source image. You don't need to set the inputImage value for the filters, it is automatically configured. If the completion closure parameter is set the execution is performed in a background thread so the UI stays responsive, the methods immediatly returns with null value and, when the image is ready, it is passed as the only parameter of the closure; otherwise, the execution is performed in the main thread and the methods returns the resulting image. The optional rectToRender parameter defines the region of the image to render. If not set, the extent of the filtered image is used instead and the image is completely rendered (if the extent of the image is infinite, the rect is too big to be rendered so the resulting image is NULL).





### Enums

<div id="_enum_ImageResizingMode"></div>

#### ImageResizingMode
 * .Stretch
 * .Tile

<div id="_enum_ImageRenderingMode"></div>

#### ImageRenderingMode
 * .AlwaysOriginal
 * .AlwaysTemplate
 * .Automatic

<div id="_enum_ImageOrientation"></div>

#### ImageOrientation
 * .Down
 * .DownMirrored
 * .Left
 * .LeftMirrored
 * .Right
 * .RightMirrored
 * .Up
 * .UpMirrored



