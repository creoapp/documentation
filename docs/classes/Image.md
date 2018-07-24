**super**: [Object](Object.md)

A Image object manages image data in your app. You use image objects to represent image data of all kinds, and the Image class is capable of managing data for all image formats supported by the underlying platform. Image objects are immutable, so you always create them from existing image data, such as an image file on disk or programmatically created image data. An image object may contain a single image or a sequence of images you intend to use in an animation. Although image objects support all platform-native image formats, it is recommended that you use PNG or JPEG files for most images in your app. Image objects are optimized for reading and displaying both formats, and those formats offer better performance than most other image formats. Because the PNG format is lossless, it is especially recommended for the images you use in your app’s interface.

### Events

* None

### Properties

* **var** **size**: **[Size](size.md)**
The logical dimensions of the image, measured in points. Multiply the size values by the value in the scale property to get the pixel dimensions of the image. \(read-only\)

* **var** **scale**: **[Float](../gravity/types.md)**
The scale factor of the image. If you multiply the logical size of the image (stored in the size property) by the value in this property, you get the dimensions of the image in pixels. \(read-only\)

* **var** **capInsets**: **[EdgeInsets](edgeinsets.md)**
The end-cap insets. End caps specify the portion of an image that should not be resized when an image is stretched. This technique is used to implement buttons and other resizable image-based interface elements. When a button with end caps is resized, the resizing occurs only in the middle of the button, in the region between the end caps. The end caps themselves keep their original size and appearance.

This property specifies the sizes of all four end caps. The middle (stretchable) portion consists of all the pixels that are not included in the end caps. These pixels are tiled, left-to-right, top-to-bottom to fill the remaining space. \(read-only\)

* **var** **resizingMode**: **ImageResizingMode**
The resizing mode of the image. \(read-only\)

* **var** **renderingMode**: **ImageRenderingMode**
Determines how an image is rendered. \(read-only\)



### Class Methods

* **func** **open**(**srcfile**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Object](../gravity/types.md)</strong> 
Initializes and returns the image object with the content of the source file. The source file can be an URL or a <a href="File.html">File</a> object.



### Initializers

* **func** **Image**(**name**: <strong>[String](../gravity/types.md)</strong>)
Initializes and returns the image object with the specified name.

* **func** **Image**(**data**: <strong>[Data](data.md)</strong>, **scale**: <strong>[Float](../gravity/types.md)</strong>)
Initializes and returns the image object with the specified data and scale factor. 



### Methods

* **func** **resizableImageWithCapInsets**(**capInsets**: <strong>[EdgeInsets](edgeinsets.md)</strong>, **resizingMode**: <strong><a href="#_enum_ImageResizingMode">ImageResizingMode</a></strong>): <strong>[Image](image.md)</strong> 
Creates and returns a new image object with the specified cap insets and options.

* **func** **PNGRepresentation**(): <strong>[Data](data.md)</strong> 
Returns the data for the specified image in PNG format.

* **func** **JPEGRepresentation**(**compressionQuality**: <strong>[Float](../gravity/types.md)</strong>): <strong>[Data](data.md)</strong> 
Returns the data for the specified image in JPEG format using the specified compression quality.

* **func** **scaleImageToFillSize**(**size**: <strong>[Size](size.md)</strong>): <strong>[Image](image.md)</strong> 
Returns a scaled version of the image that fill the specified size, preserving the aspect ratio of the original image (as "aspect fill")

* **func** **scaleImageToFitSize**(**size**: <strong>[Size](size.md)</strong>): <strong>[Image](image.md)</strong> 
Returns a scaled version of the image that fit into the specified size, preserving the aspect ratio of the original image (as "aspect fit")

* **func** **imageWithRenderingMode**(**renderingMode**: <strong><a href="#_enum_ImageRenderingMode">ImageRenderingMode</a></strong>): <strong>[Image](image.md)</strong> 
Creates and returns a new image object with the specified rendering mode.





### Enumeration

#### ImageResizingMode
 * .Stretch
 * .Tile

#### ImageRenderingMode
 * .AlwaysOriginal
 * .AlwaysTemplate
 * .Automatic



