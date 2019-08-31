**super**: **[Object](../gravity/object.md)**

A Color object represents color and sometimes opacity (alpha value). You can use Color objects to store color data, and during drawing you can use them to set the current fill and stroke colors.
Many methods require you to specify color data using a Color object, and for general color needs it should be your main way of specifying colors.



### Class Properties

* **var** **black**: **[Color](Color.md)**
Returns a color object whose grayscale value is 0.0 and whose alpha value is 1.0. \(read-only\)

* **var** **darkGray**: **[Color](Color.md)**
Returns a color object whose grayscale value is 1/3 and whose alpha value is 1.0. \(read-only\)

* **var** **lightGray**: **[Color](Color.md)**
Returns a color object whose grayscale value is 2/3 and whose alpha value is 1.0. \(read-only\)

* **var** **white**: **[Color](Color.md)**
Returns a color object whose grayscale value is 1.0 and whose alpha value is 1.0. \(read-only\)

* **var** **gray**: **[Color](Color.md)**
Returns a color object whose grayscale value is 0.5 and whose alpha value is 1.0. \(read-only\)

* **var** **red**: **[Color](Color.md)**
Returns a color object whose RGB values are 1.0, 0.0, and 0.0 and whose alpha value is 1.0. \(read-only\)

* **var** **green**: **[Color](Color.md)**
Returns a color object whose RGB values are 0.0, 1.0, and 0.0 and whose alpha value is 1.0. \(read-only\)

* **var** **blue**: **[Color](Color.md)**
Returns a color object whose RGB values are 0.0, 0.0, and 1.0 and whose alpha value is 1.0. \(read-only\)

* **var** **cyan**: **[Color](Color.md)**
Returns a color object whose RGB values are 0.0, 1.0, and 1.0 and whose alpha value is 1.0. \(read-only\)

* **var** **yellow**: **[Color](Color.md)**
Returns a color object whose RGB values are 1.0, 1.0, and 0.0 and whose alpha value is 1.0. \(read-only\)

* **var** **magenta**: **[Color](Color.md)**
Returns a color object whose RGB values are 1.0, 0.0, and 1.0 and whose alpha value is 1.0. \(read-only\)

* **var** **orange**: **[Color](Color.md)**
Returns a color object whose RGB values are 1.0, 0.5, and 0.0 and whose alpha value is 1.0. \(read-only\)

* **var** **purple**: **[Color](Color.md)**
Returns a color object whose RGB values are 0.5, 0.0, and 0.5 and whose alpha value is 1.0. \(read-only\)

* **var** **brown**: **[Color](Color.md)**
Returns a color object whose RGB values are 0.6, 0.4, and 0.2 and whose alpha value is 1.0. \(read-only\)

* **var** **clear**: **[Color](Color.md)**
Returns a color object whose grayscale and alpha values are both 0.0. \(read-only\)



### Properties

* **var** **spaceModel**: **ColorSpaceModel**
Returns the model on which the color space of the receiver is based. \(read-only\)

* **var** **isRGB**: **[Bool](../gravity/bool.md)**
Returns true if can be decomposed by its RGB components. \(read-only\)

* **var** **red**: **[Float](../gravity/float.md)**
Returns red component (only valid if isRGB is true). \(read-only\)

* **var** **green**: **[Float](../gravity/float.md)**
Returns green component (only valid if isRGB is true). \(read-only\)

* **var** **blue**: **[Float](../gravity/float.md)**
Returns blue component (only valid if isRGB is true). \(read-only\)

* **var** **white**: **[Float](../gravity/float.md)**
Returns white component (only valid if spaceModel is ColorSpaceModel.Monocrome). \(read-only\)

* **var** **hue**: **[Float](../gravity/float.md)**
Returns hue component (only valid if isRGB is true). \(read-only\)

* **var** **saturation**: **[Float](../gravity/float.md)**
Returns saturation component (only valid if isRGB is true). \(read-only\)

* **var** **brightness**: **[Float](../gravity/float.md)**
Returns brightness component (only valid if isRGB is true). \(read-only\)

* **var** **alpha**: **[Float](../gravity/float.md)**
Returns alpha component. \(read-only\)

* **var** **luminance**: **[Float](../gravity/float.md)**
Returns luminance component (only valid if isRGB is true). \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **colorWithPatternImage**(**image**: **[Image](Image.md)**): <strong>[Color](Color.md)</strong> 
Creates and returns a color object using the specified image. You can use pattern colors to set the fill or stroke color just as you would a solid color. During drawing, the image in the pattern color is tiled as necessary to cover the given area.

* **func** **hsba**(**hue**: **[Float](../gravity/float.md)**, **saturation**: **[Float](../gravity/float.md)**, **brightness**: **[Float](../gravity/float.md)**, **alpha**: **[Float](../gravity/float.md)**): <strong>[Color](Color.md)</strong> 
Creates and returns a color object using the specified opacity and HSB color space component values.

* **func** **rgba**(**red**: **[Float](../gravity/float.md)**, **green**: **[Float](../gravity/float.md)**, **blue**: **[Float](../gravity/float.md)**, **alpha**: **[Float](../gravity/float.md)**): <strong>[Color](Color.md)</strong> 
Creates and returns a color object using the specified opacity and RGB component values.

* **func** **whiteWithAlpha**(**white**: **[Float](../gravity/float.md)**, **alpha**: **[Float](../gravity/float.md)**): <strong>[Color](Color.md)</strong> 
Initializes and returns a color object using the specified opacity and grayscale values.



### Initializers

* **func** **Color**(**red**: **[Float](../gravity/float.md)**, **green**: **[Float](../gravity/float.md)**, **blue**: **[Float](../gravity/float.md)**, **alpha**: **[Float](../gravity/float.md)**)
Creates a color object using the specified opacity and RGB component values.

* **func** **Color**(**red**: **[Float](../gravity/float.md)**, **green**: **[Float](../gravity/float.md)**, **blue**: **[Float](../gravity/float.md)**)
Creates a color object using the specified RGB component values (alphs set to 1.0).

* **func** **Color**(**string**: **[String](../gravity/string.md)**)
Creates a color using the specified HEX string.



### Methods

* **func** **hex**(**withAlpha**: **[Bool](../gravity/bool.md)**): <strong>[String](../gravity/string.md)</strong> 
Returns hex string representing the color (with an optional alpha value speciafied in the parameter, this method is valid only if isRGB is true).

* **func** **darkerColor**(**amount**: **[Float](../gravity/float.md)**): <strong>[Color](Color.md)</strong> 
Returns a darker color with the amount specified in the parameter (only valid if isRGB is true).





### Enums

<div id="_enum_ColorSpaceModel"></div>

#### ColorSpaceModel
 * .CMYK
 * .DeviceN
 * .Lab
 * .Monochrome
 * .Pattern
 * .RGB
 * .Unknown



