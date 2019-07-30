List of the available ImageFilter.

#### CIEdges:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Edges |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIEdges |
| CIAttributeReferenceDocumentation | [CIEdges Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEdges) |
| inputIntensity | CIAttributeDefault = 1;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the edges. The larger the value, the higher the intensity.;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIOpTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Op Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of a tile.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIOpTile |
| CIAttributeReferenceDocumentation | [CIOpTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIOpTile) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scale determines the number of tiles in the effect.;<br/>CIAttributeDefault = 2.8;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.1 |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 65;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 65;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAffineTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Affine Tile |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAffineTile |
| CIAttributeReferenceDocumentation | [CIAffineTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAffineTile) |
| inputTransform | CIAttributeDisplayName = Transform;<br/>CIAttributeDescription = The transform to apply to the image.;<br/>CIAttributeIdentity = <NSAffineTransform: 0x6000017802c0>;<br/>CIAttributeDefault = <NSAffineTransform: 0x600001780280>;<br/>CIAttributeClass = NSAffineTransform |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Perspective Transform |
| inputTopRight | CIAttributeDisplayName = Top Right;<br/>CIAttributeDescription = The top right coordinate to map the image to.;<br/>CIAttributeDefault = [646 507];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIPerspectiveTransform |
| CIAttributeReferenceDocumentation | [CIPerspectiveTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveTransform) |
| inputBottomLeft | CIAttributeDisplayName = Bottom Left;<br/>CIAttributeDescription = The bottom left coordinate to map the image to.;<br/>CIAttributeDefault = [155 153];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputTopLeft | CIAttributeDisplayName = Top Left;<br/>CIAttributeDescription = The top left coordinate to map the image to.;<br/>CIAttributeDefault = [118 484];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputBottomRight | CIAttributeDisplayName = Bottom Right;<br/>CIAttributeDescription = The bottom right coordinate to map the image to.;<br/>CIAttributeDefault = [548 140];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAffineClamp:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Affine Clamp |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAffineClamp |
| CIAttributeReferenceDocumentation | [CIAffineClamp Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAffineClamp) |
| inputTransform | CIAttributeDisplayName = Transform;<br/>CIAttributeDescription = The transform to apply to the image.;<br/>CIAttributeIdentity = <NSAffineTransform: 0x600001780040>;<br/>CIAttributeDefault = <NSAffineTransform: 0x600001780000>;<br/>CIAttributeClass = NSAffineTransform |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CINoiseReduction:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Noise Reduction |
| inputNoiseLevel | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of noise reduction. The larger the value, the more noise reduction.;<br/>CIAttributeSliderMax = 0.1;<br/>CIAttributeDisplayName = Noise Level;<br/>CIAttributeDefault = 0.02;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CINoiseReduction |
| CIAttributeReferenceDocumentation | [CINoiseReduction Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CINoiseReduction) |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The sharpness of the final image. The larger the value, the sharper the result.;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeDefault = 0.4;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHueBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Hue Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHueBlendMode |
| CIAttributeReferenceDocumentation | [CIHueBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHueBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorPosterize:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Color Posterize |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorPosterize |
| CIAttributeReferenceDocumentation | [CIColorPosterize Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorPosterize) |
| inputLevels | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The number of brightness levels to use for each color component. Lower values result in a more extreme poster effect.;<br/>CIAttributeDefault = 6;<br/>CIAttributeDisplayName = Levels;<br/>CIAttributeSliderMax = 30;<br/>CIAttributeMin = 1;<br/>CIAttributeIdentity = 300;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 2 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorMonochrome:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Monochrome |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorMonochrome |
| CIAttributeReferenceDocumentation | [CIColorMonochrome Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorMonochrome) |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The monochrome color to apply to the image.;<br/>CIAttributeDefault = (0.6 0.45 0.3 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeOpaqueColor |
| inputIntensity | CIAttributeDefault = 1;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the monochrome effect. A value of 1.0 creates a monochrome image using the supplied color. A value of 0.0 has no effect on the image.;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMaximumComponent:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Maximum Component |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMaximumComponent |
| CIAttributeReferenceDocumentation | [CIMaximumComponent Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaximumComponent) |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIPhotoEffectMono:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Mono |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectMono |
| CIAttributeReferenceDocumentation | [CIPhotoEffectMono Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectMono) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CITriangleKaleidoscope:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Triangle Kaleidoscope |
| inputPoint | CIAttributeDisplayName = Point;<br/>CIAttributeDescription = The x and y position to use as the center of the triangular area in the input image.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = Input image to generate kaleidoscope effect from.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CITriangleKaleidoscope |
| CIAttributeReferenceDocumentation | [CITriangleKaleidoscope Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITriangleKaleidoscope) |
| inputSize | CIAttributeDefault = 700;<br/>CIAttributeDescription = The size in pixels of the triangle.;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Size;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputRotation | CIAttributeDefault = 5.924285296593801;<br/>CIAttributeDescription = Rotation angle of the triangle.;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Rotation;<br/>CIAttributeSliderMax = 6.283185307179586;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = 0 |
| inputDecay | CIAttributeDefault = 0.85;<br/>CIAttributeDescription = The decay determines how fast the color fades from the center triangle.;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Decay;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIConvolution9Horizontal:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Horizontal 9 Convolution |
| inputWeights | CIAttributeDisplayName = Weights;<br/>CIAttributeIdentity = [0 0 0 0 1 0 0 0 0];<br/>CIAttributeDefault = [0 0 0 0 1 0 0 0 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution9Horizontal |
| CIAttributeReferenceDocumentation | [CIConvolution9Horizontal Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution9Horizontal) |
| inputBias | CIAttributeDisplayName = Bias;<br/>CIAttributeIdentity = 0;<br/>CIAttributeDefault = 0;<br/>CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIPointillize:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Pointillize |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIPointillize |
| CIAttributeReferenceDocumentation | [CIPointillize Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPointillize) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the circles in the resulting pattern.;<br/>CIAttributeDefault = 20;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 1;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorCurves:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Color Curves |
| inputColorSpace | CIAttributeDisplayName = Color Space;<br/>CIAttributeClass = NSObject |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCurves |
| CIAttributeReferenceDocumentation | [CIColorCurves Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCurves) |
| inputCurvesDomain | CIAttributeDefault = [0 1];<br/>CIAttributeDisplayName = Curves Domain;<br/>CIAttributeClass = Vector |
| inputCurvesData | CIAttributeDefault = <00000000 00000000 00000000 0000003f 0000003f 0000003f 0000803f 0000803f 0000803f>;<br/>CIAttributeDisplayName = Curves Data;<br/>CIAttributeClass = NSData |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIParallelogramTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Parallelogram Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIParallelogramTile |
| CIAttributeReferenceDocumentation | [CIParallelogramTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIParallelogramTile) |
| inputAcuteAngle | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The primary angle for the repeating parallelogram tile. Small values create thin diamond tiles, and higher values create fatter parallelogram tiles.;<br/>CIAttributeDefault = 1.570796326794897;<br/>CIAttributeDisplayName = Acute Angle;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeIdentity = 1.570796326794897;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBloom:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Bloom |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBloom |
| CIAttributeReferenceDocumentation | [CIBloom Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBloom) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the effect. The larger the radius, the greater the effect.;<br/>CIAttributeDefault = 10;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputIntensity | CIAttributeDefault = 0.5;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the effect. A value of 0.0 is no effect. A value of 1.0 is the maximum effect.;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIQRCodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | QR Code Generator |
| inputMessage | CIAttributeDescription = The message to encode in the QR Code;<br/>CIAttributeDisplayName = Message;<br/>CIAttributeClass = NSData |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIQRCodeGenerator |
| inputCorrectionLevel | CIAttributeDisplayName = Correction Level;<br/>CIAttributeDescription = QR Code correction level L, M, Q, or H.;<br/>CIAttributeDefault = M;<br/>CIAttributeClass = NSString |
| CIAttributeReferenceDocumentation | [CIQRCodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIQRCodeGenerator) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIFalseColor:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | False Color |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIFalseColor |
| CIAttributeReferenceDocumentation | [CIFalseColor Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFalseColor) |
| inputColor0 | CIAttributeDisplayName = Color 1;<br/>CIAttributeDescription = The first color to use for the color ramp.;<br/>CIAttributeDefault = (0.3 0 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| inputColor1 | CIAttributeDisplayName = Color 2;<br/>CIAttributeDescription = The second color to use for the color ramp.;<br/>CIAttributeDefault = (1 0.9 0.8 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAreaMaximumAlpha:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Maximum Alpha |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMaximumAlpha |
| CIAttributeReferenceDocumentation | [CIAreaMaximumAlpha Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMaximumAlpha) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIMeshGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Mesh Generator |
| inputMesh | CIAttributeDescription = An array of line segments stored as an array of CIVectors each containing a start point and end point.;<br/>CIAttributeDisplayName = Mesh;<br/>CIAttributeClass = NSArray |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMeshGenerator |
| CIAttributeReferenceDocumentation | [CIMeshGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMeshGenerator) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of the effect.;<br/>CIAttributeDefault = 1.5;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = A color.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIAttributedTextImageGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Attributed Text Image Generator |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputText | CIAttributeDisplayName = Text;<br/>CIAttributeClass = NSAttributedString |
| CIAttributeFilterName | CIAttributedTextImageGenerator |
| CIAttributeReferenceDocumentation | [CIAttributedTextImageGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAttributedTextImageGenerator) |
| inputScaleFactor | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 4;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Scale Factor;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIDotScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Dot Screen |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryHalftoneEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDotScreen |
| CIAttributeReferenceDocumentation | [CIDotScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDotScreen) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance between dots in the pattern.;<br/>CIAttributeDefault = 6;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 2 |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The sharpness of the pattern. The larger the value, the sharper the pattern.;<br/>CIAttributeDefault = 0.7;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the dot screen pattern;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIOverlayBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Overlay Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIOverlayBlendMode |
| CIAttributeReferenceDocumentation | [CIOverlayBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIOverlayBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIRadialGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Radial Gradient |
| inputRadius0 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the starting circle to use in the gradient.;<br/>CIAttributeDefault = 5;<br/>CIAttributeDisplayName = Radius 1;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterCategories | CICategoryGradient;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIRadialGradient |
| inputRadius1 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the ending circle to use in the gradient.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Radius 2;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CIRadialGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRadialGradient) |
| inputColor0 | CIAttributeDisplayName = Color 1;<br/>CIAttributeDescription = The first color to use in the gradient.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| inputColor1 | CIAttributeDisplayName = Color 2;<br/>CIAttributeDescription = The second color to use in the gradient.;<br/>CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPinchDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Pinch Distortion |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIPinchDistortion |
| CIAttributeReferenceDocumentation | [CIPinchDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPinchDistortion) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of pinching. A value of 0.0 has no effect. A value of 1.0 is the maximum pinch.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIComicEffect:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Comic Effect |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIComicEffect |
| CIAttributeReferenceDocumentation | [CIComicEffect Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIComicEffect) |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CISubtractBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Subtract Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISubtractBlendMode |
| CIAttributeReferenceDocumentation | [CISubtractBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISubtractBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMix:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Mix |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as a foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMix |
| CIAttributeReferenceDocumentation | [CIMix Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMix) |
| inputAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of the effect.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Amount;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIBumpDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Bump Distortion |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBumpDistortion |
| CIAttributeReferenceDocumentation | [CIBumpDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBumpDistortion) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scale of the effect determines the curvature of the bump. A value of 0.0 has no effect. Positive values create an outward bump; negative values create an inward bump.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -1 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 600;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDisparityToDepth:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Disparity To Depth |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The input disparity data image to convert to depth data.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDisparityToDepth |
| CIAttributeReferenceDocumentation | [CIDisparityToDepth Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDisparityToDepth) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIHatchedScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Hatched Screen |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryHalftoneEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHatchedScreen |
| CIAttributeReferenceDocumentation | [CIHatchedScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHatchedScreen) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance between lines in the pattern.;<br/>CIAttributeDefault = 6;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 2 |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of sharpening to apply.;<br/>CIAttributeDefault = 0.7;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the hatched screen pattern;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIRowAverage:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Row Average |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIRowAverage |
| CIAttributeReferenceDocumentation | [CIRowAverage Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRowAverage) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIBlendWithRedMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Blend With Red Mask |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithRedMask |
| CIAttributeReferenceDocumentation | [CIBlendWithRedMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithRedMask) |
| inputMaskImage | CIAttributeDisplayName = Mask Image;<br/>CIAttributeDescription = A masking image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILenticularHaloGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = A color.;<br/>CIAttributeDefault = (1 0.9 0.8 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The duration of the effect.;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0 |
| inputStriationStrength | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The intensity of the halo colors. Larger values are more intense.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Striation Strength;<br/>CIAttributeSliderMax = 3;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CILenticularHaloGenerator |
| CIAttributeFilterDisplayName | Lenticular Halo |
| inputHaloOverlap | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDefault = 0.77;<br/>CIAttributeDisplayName = Halo Overlap;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the halo.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeReferenceDocumentation | [CILenticularHaloGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILenticularHaloGenerator) |
| inputStriationContrast | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The contrast of the halo colors. Larger values are higher contrast.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Striation Contrast;<br/>CIAttributeSliderMax = 5;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputHaloRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the halo.;<br/>CIAttributeDefault = 70;<br/>CIAttributeDisplayName = Halo Radius;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputHaloWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of the halo, from its inner radius to its outer radius.;<br/>CIAttributeDefault = 87;<br/>CIAttributeDisplayName = Halo Width;<br/>CIAttributeSliderMax = 300;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |


#### CICircleSplashDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Circle Splash Distortion |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICircleSplashDistortion |
| CIAttributeReferenceDocumentation | [CICircleSplashDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICircleSplashDistortion) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 150;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CICircularWrap:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Circular Wrap Distortion |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the effect.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICircularWrap |
| CIAttributeReferenceDocumentation | [CICircularWrap Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICircularWrap) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 150;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 600;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIStraightenFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Straighten |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = An angle in radians.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIStraightenFilter |
| CIAttributeReferenceDocumentation | [CIStraightenFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStraightenFilter) |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIHighlightShadowAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Highlight and Shadow Adjust |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHighlightShadowAdjust |
| CIAttributeReferenceDocumentation | [CIHighlightShadowAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHighlightShadowAdjust) |
| inputHighlightAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of adjustment to the highlights of the image.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Highlight Amount;<br/>CIAttributeSliderMin = 0.3;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 1 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Shadow Highlight Radius;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputShadowAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of adjustment to the shadows of the image.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Shadow Amount;<br/>CIAttributeSliderMin = -1;<br/>CIAttributeMin = -1;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIColorCrossPolynomial:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Cross Polynomial |
| inputRedCoefficients | CIAttributeDisplayName = Red Coefficients;<br/>CIAttributeDescription = Polynomial coefficients for red channel;<br/>CIAttributeIdentity = [1 0 0 0 0 0 0 0 0 0];<br/>CIAttributeDefault = [1 0 0 0 0 0 0 0 0 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCrossPolynomial |
| CIAttributeReferenceDocumentation | [CIColorCrossPolynomial Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCrossPolynomial) |
| inputGreenCoefficients | CIAttributeDisplayName = Green Coefficients;<br/>CIAttributeDescription = Polynomial coefficients for green channel;<br/>CIAttributeIdentity = [0 1 0 0 0 0 0 0 0 0];<br/>CIAttributeDefault = [0 1 0 0 0 0 0 0 0 0];<br/>CIAttributeClass = Vector |
| inputBlueCoefficients | CIAttributeDisplayName = Blue Coefficients;<br/>CIAttributeDescription = Polynomial coefficients for blue channel;<br/>CIAttributeIdentity = [0 0 1 0 0 0 0 0 0 0];<br/>CIAttributeDefault = [0 0 1 0 0 0 0 0 0 0];<br/>CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIUnsharpMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Unsharp Mask |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategorySharpen;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIUnsharpMask |
| CIAttributeReferenceDocumentation | [CIUnsharpMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIUnsharpMask) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius around a given pixel to apply the unsharp mask. The larger the radius, the more of the image is affected.;<br/>CIAttributeDefault = 2.5;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputIntensity | CIAttributeDefault = 0.5;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the effect. The larger the value, the more contrast in the affected area.;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISourceOutCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source Out |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISourceOutCompositing |
| CIAttributeReferenceDocumentation | [CISourceOutCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceOutCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAdditionCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Addition |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAdditionCompositing |
| CIAttributeReferenceDocumentation | [CIAdditionCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAdditionCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHistogramDisplayFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Histogram Display |
| inputHeight | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The height of the displayable histogram image.;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeDisplayName = Height;<br/>CIAttributeSliderMin = 1;<br/>CIAttributeMin = 1;<br/>CIAttributeMax = 200;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 100 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHistogramDisplayFilter |
| CIAttributeReferenceDocumentation | [CIHistogramDisplayFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHistogramDisplayFilter) |
| inputLowLimit | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The fraction of the left portion of the histogram image to make darker;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Low Limit;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0 |
| inputHighLimit | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The fraction of the right portion of the histogram image to make lighter.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = High Limit;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 1 |
| CIAttributeFilterAvailable_Mac | 10.? |


#### CILineScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Line Screen |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryHalftoneEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILineScreen |
| CIAttributeReferenceDocumentation | [CILineScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILineScreen) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance between lines in the pattern.;<br/>CIAttributeDefault = 6;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 2 |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The sharpness of the pattern. The larger the value, the sharper the pattern.;<br/>CIAttributeDefault = 0.7;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the line screen pattern;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveCorrection:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.10 |
| CIAttributeFilterName | CIPerspectiveCorrection |
| CIAttributeFilterDisplayName | Perspective Correction |
| inputTopRight | CIAttributeDisplayName = Top Right;<br/>CIAttributeDescription = The top right coordinate to be perspective corrected.;<br/>CIAttributeDefault = [646 507];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputCrop | CIAttributeDisplayName = Crop;<br/>CIAttributeDefault = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeType = CIAttributeTypeBoolean |
| inputBottomRight | CIAttributeDisplayName = Bottom Right;<br/>CIAttributeDescription = The bottom right coordinate to be perspective corrected.;<br/>CIAttributeDefault = [548 140];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeReferenceDocumentation | [CIPerspectiveCorrection Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveCorrection) |
| inputTopLeft | CIAttributeDisplayName = Top Left;<br/>CIAttributeDescription = The top left coordinate to be perspective corrected.;<br/>CIAttributeDefault = [118 484];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryBuiltIn |
| inputBottomLeft | CIAttributeDisplayName = Bottom Left;<br/>CIAttributeDescription = The bottom left coordinate to be perspective corrected.;<br/>CIAttributeDefault = [155 153];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIAreaMaximum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Maximum |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMaximum |
| CIAttributeReferenceDocumentation | [CIAreaMaximum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMaximum) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CISmoothLinearGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Smooth Linear Gradient |
| inputColor1 | CIAttributeDisplayName = Color 2;<br/>CIAttributeDescription = The second color to use in the gradient.;<br/>CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterCategories | CICategoryGradient;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISmoothLinearGradient |
| inputColor0 | CIAttributeDisplayName = Color 1;<br/>CIAttributeDescription = The first color to use in the gradient.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeReferenceDocumentation | [CISmoothLinearGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISmoothLinearGradient) |
| inputPoint1 | CIAttributeDisplayName = Point 1;<br/>CIAttributeDescription = The ending position of the gradient -- where the second color begins.;<br/>CIAttributeDefault = [200 200];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputPoint0 | CIAttributeDisplayName = Point 0;<br/>CIAttributeDescription = The starting position of the gradient -- where the first color begins.;<br/>CIAttributeDefault = [0 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CISixfoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Sixfold Reflected Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISixfoldReflectedTile |
| CIAttributeReferenceDocumentation | [CISixfoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISixfoldReflectedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CISpotLight:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputLightPointsAt | CIAttributeDisplayName = Light Points At;<br/>CIAttributeDescription = The x and y position that the spotlight points at.;<br/>CIAttributeDefault = [200 200 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition3 |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The color of the spotlight.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeOpaqueColor |
| inputConcentration | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The spotlight size. The smaller the value, the more tightly focused the light beam.;<br/>CIAttributeDefault = 0.1;<br/>CIAttributeDisplayName = Concentration;<br/>CIAttributeSliderMax = 1.5;<br/>CIAttributeMin = 0.001;<br/>CIAttributeIdentity = 20;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.001 |
| CIAttributeFilterName | CISpotLight |
| CIAttributeFilterDisplayName | Spot Light |
| CIAttributeFilterAvailable_iOS | 9 |
| inputBrightness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The brightness of the spotlight.;<br/>CIAttributeDefault = 3;<br/>CIAttributeDisplayName = Brightness;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CISpotLight Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISpotLight) |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputLightPosition | CIAttributeDisplayName = Light Position;<br/>CIAttributeDescription = The x and y position of the spotlight.;<br/>CIAttributeDefault = [400 600 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition3 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIThermal:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Thermal |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIThermal |
| CIAttributeReferenceDocumentation | [CIThermal Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIThermal) |
| CIAttributeFilterAvailable_Mac | 10.11 |


#### CICheckerboardGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Checkerboard |
| inputColor1 | CIAttributeDisplayName = Color 2;<br/>CIAttributeDescription = A color to use for the second set of squares.;<br/>CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICheckerboardGenerator |
| inputColor0 | CIAttributeDisplayName = Color 1;<br/>CIAttributeDescription = A color to use for the first set of squares.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| CIAttributeReferenceDocumentation | [CICheckerboardGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICheckerboardGenerator) |
| inputWidth | CIAttributeDefault = 80;<br/>CIAttributeDescription = The width of the squares in the pattern.;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The sharpness of the edges in pattern. The smaller the value, the more blurry the pattern. Values range from 0.0 to 1.0.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISRGBToneCurveToLinear:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | sRGB Tone Curve to Linear |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISRGBToneCurveToLinear |
| CIAttributeReferenceDocumentation | [CISRGBToneCurveToLinear Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISRGBToneCurveToLinear) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIBlendWithMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Blend With Mask |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as a foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithMask |
| CIAttributeReferenceDocumentation | [CIBlendWithMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithMask) |
| inputMaskImage | CIAttributeDisplayName = Mask Image;<br/>CIAttributeDescription = A grayscale mask. When a mask value is 0.0, the result is the background. When the mask value is 1.0, the result is the image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectChrome:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Chrome |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectChrome |
| CIAttributeReferenceDocumentation | [CIPhotoEffectChrome Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectChrome) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CINinePartTiled:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Nine Part Tiled |
| inputGrowAmount | CIAttributeDisplayName = Grow Amount;<br/>CIAttributeDefault = [100 100];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CINinePartTiled |
| CIAttributeReferenceDocumentation | [CINinePartTiled Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CINinePartTiled) |
| inputBreakpoint0 | CIAttributeDisplayName = Breakpoint0;<br/>CIAttributeDescription = Lower left corner of image to retain before tiling begins.;<br/>CIAttributeDefault = [50 50];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputFlipYTiles | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Indicates that Y-Axis flip should occur.;<br/>CIAttributeDisplayName = Flip Y Tiles;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeBoolean;<br/>CIAttributeDefault = 1 |
| inputBreakpoint1 | CIAttributeDisplayName = Breakpoint1;<br/>CIAttributeDescription = Upper right corner of image to retain after tiling ends.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIHexagonalPixellate:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Hexagonal Pixelate |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHexagonalPixellate |
| CIAttributeReferenceDocumentation | [CIHexagonalPixellate Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHexagonalPixellate) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scale determines the size of the hexagons. Larger values result in larger hexagons.;<br/>CIAttributeDefault = 8;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 1;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIBicubicScaleTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Bicubic Scale Transform |
| inputB | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Specifies the value of B to use for the cubic resampling function.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = B;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBicubicScaleTransform |
| CIAttributeReferenceDocumentation | [CIBicubicScaleTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBicubicScaleTransform) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scaling factor to use on the image. Values less than 1.0 scale down the images. Values greater than 1.0 scale up the image.;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMin = 0.05;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 1 |
| inputC | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Specifies the value of C to use for the cubic resampling function.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = C;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0.75 |
| inputAspectRatio | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The additional horizontal scaling factor to use on the image.;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeDisplayName = Aspect Ratio;<br/>CIAttributeSliderMin = 0.5;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 1 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIColorClamp:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Clamp |
| inputMaxComponents | CIAttributeDisplayName = Max Components;<br/>CIAttributeDescription = Higher clamping values;<br/>CIAttributeDefault = [1 1 1 1];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorClamp |
| CIAttributeReferenceDocumentation | [CIColorClamp Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorClamp) |
| inputMinComponents | CIAttributeDisplayName = Min Components;<br/>CIAttributeDescription = Lower clamping values;<br/>CIAttributeDefault = [0 0 0 0];<br/>CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIPhotoEffectProcess:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Process |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectProcess |
| CIAttributeReferenceDocumentation | [CIPhotoEffectProcess Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectProcess) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CISourceInCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source In |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISourceInCompositing |
| CIAttributeReferenceDocumentation | [CISourceInCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceInCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectNoir:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Noir |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectNoir |
| CIAttributeReferenceDocumentation | [CIPhotoEffectNoir Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectNoir) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CICameraCalibrationLensCorrection:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Lens Correction for AVC |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICameraCalibrationLensCorrection |
| CIAttributeReferenceDocumentation | [CICameraCalibrationLensCorrection Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICameraCalibrationLensCorrection) |
| inputAVCameraCalibrationData | CIAttributeDescription = AVCameraCalibrationData for the correction.  Will be set from the inputImage if available and can be overridden here.;<br/>CIAttributeDisplayName = Calibration Data object of type AVCameraCalibrationData;<br/>CIAttributeClass = AVCameraCalibrationData |
| inputUseInverseLookUpTable | CIAttributeDisplayName = Use Inverse Look Up Table;<br/>CIAttributeDescription = Boolean value used to select the Look Up Table from the AVCameraCalibrationData;<br/>CIAttributeDefault = 0;<br/>CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIXRay:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | X-Ray |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIXRay |
| CIAttributeReferenceDocumentation | [CIXRay Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIXRay) |
| CIAttributeFilterAvailable_Mac | 10.11 |


#### CIConvolution7X7:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | 7 by 7 convolution |
| inputWeights | CIAttributeDisplayName = Weights;<br/>CIAttributeIdentity = [0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0];<br/>CIAttributeDefault = [0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution7X7 |
| CIAttributeReferenceDocumentation | [CIConvolution7X7 Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution7X7) |
| inputBias | CIAttributeDisplayName = Bias;<br/>CIAttributeIdentity = 0;<br/>CIAttributeDefault = 0;<br/>CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIToneCurve:
| Attribute | Value |
| ---------- | --------- |
| inputPoint0 | CIAttributeIdentity = [0 0];<br/>CIAttributeDisplayName = Point 0;<br/>CIAttributeDefault = [0 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterAvailable_Mac | 10.7 |
| inputPoint1 | CIAttributeIdentity = [0.25 0.25];<br/>CIAttributeDisplayName = Point 1;<br/>CIAttributeDefault = [0.25 0.25];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| inputPoint2 | CIAttributeIdentity = [0.5 0.5];<br/>CIAttributeDisplayName = Point 2;<br/>CIAttributeDefault = [0.5 0.5];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| inputPoint3 | CIAttributeIdentity = [0.75 0.75];<br/>CIAttributeDisplayName = Point 3;<br/>CIAttributeDefault = [0.75 0.75];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterName | CIToneCurve |
| CIAttributeFilterDisplayName | Tone Curve |
| inputPoint4 | CIAttributeIdentity = [1 1];<br/>CIAttributeDisplayName = Point 4;<br/>CIAttributeDefault = [1 1];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeReferenceDocumentation | [CIToneCurve Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIToneCurve) |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIColorBurnBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Burn Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorBurnBlendMode |
| CIAttributeReferenceDocumentation | [CIColorBurnBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorBurnBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectFade:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Fade |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectFade |
| CIAttributeReferenceDocumentation | [CIPhotoEffectFade Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectFade) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CICrop:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Crop |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICrop |
| CIAttributeReferenceDocumentation | [CICrop Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICrop) |
| inputRectangle | CIAttributeDisplayName = Rectangle;<br/>CIAttributeDescription = The rectangle that specifies the crop to apply to the image.;<br/>CIAttributeIdentity = [-8.98847e+307 -8.98847e+307 1.79769e+308 1.79769e+308];<br/>CIAttributeDefault = [-8.98847e+307 -8.98847e+307 1.79769e+308 1.79769e+308];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveTransformWithExtent:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| CIAttributeFilterName | CIPerspectiveTransformWithExtent |
| CIAttributeFilterDisplayName | Perspective Transform with Extent |
| inputTopRight | CIAttributeDisplayName = Top Right;<br/>CIAttributeDefault = [646 507];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that defines the extent of the effect.;<br/>CIAttributeDefault = [0 0 300 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| inputBottomRight | CIAttributeDisplayName = Bottom Right;<br/>CIAttributeDefault = [548 140];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIPerspectiveTransformWithExtent Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveTransformWithExtent) |
| inputTopLeft | CIAttributeDisplayName = Top Left;<br/>CIAttributeDefault = [118 484];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputBottomLeft | CIAttributeDisplayName = Bottom Left;<br/>CIAttributeDefault = [155 153];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIConvolution5X5:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | 5 by 5 convolution |
| inputWeights | CIAttributeDisplayName = Weights;<br/>CIAttributeIdentity = [0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0];<br/>CIAttributeDefault = [0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution5X5 |
| CIAttributeReferenceDocumentation | [CIConvolution5X5 Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution5X5) |
| inputBias | CIAttributeDisplayName = Bias;<br/>CIAttributeIdentity = 0;<br/>CIAttributeDefault = 0;<br/>CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CITwirlDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Twirl Distortion |
| inputAngle | CIAttributeDefault = 3.141592653589793;<br/>CIAttributeSliderMax = 12.56637061435917;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the twirl. Values can be positive or negative.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -12.56637061435917 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CITwirlDistortion |
| CIAttributeReferenceDocumentation | [CITwirlDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITwirlDistortion) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 500;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 300;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDisplacementDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Displacement Distortion |
| inputDisplacementImage | CIAttributeDescription = An image whose grayscale values will be applied to the source image.;<br/>CIAttributeDisplayName = Displacement Image;<br/>CIAttributeClass = Image |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDisplacementDistortion |
| CIAttributeReferenceDocumentation | [CIDisplacementDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDisplacementDistortion) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of texturing of the resulting image. The larger the value, the greater the texturing.;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeDefault = 50;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISepiaTone:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Sepia Tone |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CISepiaTone |
| CIAttributeReferenceDocumentation | [CISepiaTone Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISepiaTone) |
| inputIntensity | CIAttributeDefault = 1;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the sepia effect. A value of 1.0 creates a monochrome sepia image. A value of 0.0 has no effect on the image.;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISourceOverCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source Over |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISourceOverCompositing |
| CIAttributeReferenceDocumentation | [CISourceOverCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceOverCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIGlideReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Glide Reflected Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIGlideReflectedTile |
| CIAttributeReferenceDocumentation | [CIGlideReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGlideReflectedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIModTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputAngle | CIAttributeDefault = 2;<br/>CIAttributeSliderMax = 6.283185307179586;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the mod hole pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -6.283185307179586 |
| inputCompression | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of stretching applied to the mod hole pattern. Holes in the center are not distorted as much as those at the edge of the image.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Compression;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 100 |
| CIAttributeFilterName | CIModTransition |
| CIAttributeFilterDisplayName | Mod |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIModTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIModTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the undistorted holes in the pattern.;<br/>CIAttributeDefault = 150;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIConvolution3X3:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | 3 by 3 convolution |
| inputWeights | CIAttributeDisplayName = Weights;<br/>CIAttributeIdentity = [0 0 0 0 1 0 0 0 0];<br/>CIAttributeDefault = [0 0 0 0 1 0 0 0 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution3X3 |
| CIAttributeReferenceDocumentation | [CIConvolution3X3 Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution3X3) |
| inputBias | CIAttributeDisplayName = Bias;<br/>CIAttributeIdentity = 0;<br/>CIAttributeDefault = 0;<br/>CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIDepthToDisparity:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Depth To Disparity |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The input depth data image to convert to disparity data.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDepthToDisparity |
| CIAttributeReferenceDocumentation | [CIDepthToDisparity Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDepthToDisparity) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILanczosScaleTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Lanczos Scale Transform |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILanczosScaleTransform |
| CIAttributeReferenceDocumentation | [CILanczosScaleTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILanczosScaleTransform) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scaling factor to use on the image. Values less than 1.0 scale down the images. Values greater than 1.0 scale up the image.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 1.5;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.05 |
| inputAspectRatio | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The additional horizontal scaling factor to use on the image.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Aspect Ratio;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.5 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHeightFieldFromMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Height Field From Mask |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The white values of the mask define those pixels that are inside the height field while the black values define those pixels that are outside. The field varies smoothly and continuously inside the mask, reaching the value 0 at the edge of the mask.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHeightFieldFromMask |
| CIAttributeReferenceDocumentation | [CIHeightFieldFromMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHeightFieldFromMask) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance from the edge of the mask for the smooth transition is proportional to the input radius. Larger values make the transition smoother and more pronounced. Smaller values make the transition approximate a fillet radius.;<br/>CIAttributeDefault = 10;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 300;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 10;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDivideBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Divide Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDivideBlendMode |
| CIAttributeReferenceDocumentation | [CIDivideBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDivideBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIDifferenceBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Difference Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDifferenceBlendMode |
| CIAttributeReferenceDocumentation | [CIDifferenceBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDifferenceBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMorphologyGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Morphology Gradient |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMorphologyGradient |
| CIAttributeReferenceDocumentation | [CIMorphologyGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMorphologyGradient) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The desired radius of the circular morphological operation to the image.;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeDefault = 5;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIMinimumComponent:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Minimum Component |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMinimumComponent |
| CIAttributeReferenceDocumentation | [CIMinimumComponent Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMinimumComponent) |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIDiscBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Disc Blur |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDiscBlur |
| CIAttributeReferenceDocumentation | [CIDiscBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDiscBlur) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;<br/>CIAttributeDefault = 8;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CITorusLensDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Torus Lens Distortion |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CITorusLensDistortion |
| CIAttributeReferenceDocumentation | [CITorusLensDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITorusLensDistortion) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of the ring.;<br/>CIAttributeDefault = 80;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The outer radius of the torus.;<br/>CIAttributeDefault = 160;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 500;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputRefraction | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The refraction of the glass.;<br/>CIAttributeSliderMax = 5;<br/>CIAttributeDisplayName = Refraction;<br/>CIAttributeDefault = 1.7;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the torus.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIFlashTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The color of the light rays emanating from the flash.;<br/>CIAttributeDefault = (1 0.8 0.6 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputStriationStrength | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The strength of the light rays emanating from the flash.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Striation Strength;<br/>CIAttributeSliderMax = 3;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CIFlashTransition |
| CIAttributeFilterDisplayName | Flash |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = The extent of the flash.;<br/>CIAttributeDefault = [0 0 300 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| inputFadeThreshold | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of fade between the flash and the target image. The higher the value, the more flash time and the less fade time.;<br/>CIAttributeDefault = 0.85;<br/>CIAttributeDisplayName = Fade Threshold;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| inputStriationContrast | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The contrast of the light rays emanating from the flash.;<br/>CIAttributeDefault = 1.375;<br/>CIAttributeDisplayName = Striation Contrast;<br/>CIAttributeSliderMax = 5;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CIFlashTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFlashTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputMaxStriationRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the light rays emanating from the flash.;<br/>CIAttributeDefault = 2.58;<br/>CIAttributeDisplayName = Maximum Striation Radius;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIFourfoldRotatedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Fourfold Rotated Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIFourfoldRotatedTile |
| CIAttributeReferenceDocumentation | [CIFourfoldRotatedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFourfoldRotatedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIColorCubesMixedWithMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.13 |
| inputCubeDimension | CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Cube Dimension;<br/>CIAttributeMin = 2;<br/>CIAttributeMax = 128;<br/>CIAttributeIdentity = 2;<br/>CIAttributeType = CIAttributeTypeCount;<br/>CIAttributeDefault = 2 |
| inputMaskImage | CIAttributeDisplayName = Mask Image;<br/>CIAttributeDescription = A masking image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputCube0Data | CIAttributeDisplayName = Cube 0 Data;<br/>CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;<br/>CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeClass = NSData |
| CIAttributeFilterName | CIColorCubesMixedWithMask |
| CIAttributeFilterDisplayName | Color Cubes Mixed With Mask |
| inputCube1Data | CIAttributeDisplayName = Cube 1 Data;<br/>CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;<br/>CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeClass = NSData |
| CIAttributeFilterAvailable_iOS | 11 |
| inputColorSpace | CIAttributeDisplayName = Color Space;<br/>CIAttributeClass = NSObject |
| CIAttributeReferenceDocumentation | [CIColorCubesMixedWithMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCubesMixedWithMask) |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIKaleidoscope:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Kaleidoscope |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of reflection.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIKaleidoscope |
| CIAttributeReferenceDocumentation | [CIKaleidoscope Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIKaleidoscope) |
| inputCount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The number of reflections in the pattern.;<br/>CIAttributeDefault = 6;<br/>CIAttributeDisplayName = Count;<br/>CIAttributeSliderMax = 64;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBarcodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Barcode Generator |
| inputBarcodeDescriptor | CIAttributeDescription = The CIBarcodeDescription object to generate an image for.;<br/>CIAttributeDisplayName = Barcode Descriptor;<br/>CIAttributeClass = CIBarcodeDescriptor |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBarcodeGenerator |
| CIAttributeReferenceDocumentation | [CIBarcodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBarcodeGenerator) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIAreaHistogram:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Area Histogram |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image whose histogram you want to calculate.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaHistogram |
| CIAttributeReferenceDocumentation | [CIAreaHistogram Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaHistogram) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scale value to use for the histogram values. If the scale is 1.0, then the bins in the resulting image will add up to 1.0.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The number of bins for the histogram. This value will determine the width of the output image.;<br/>CIAttributeDefault = 64;<br/>CIAttributeDisplayName = Count;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeMin = 1;<br/>CIAttributeMax = 2048;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 10 |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that, after intersection with the image extent, specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIEdgePreserveUpsampleFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Edge Preserve Upsample Filter |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIEdgePreserveUpsampleFilter |
| CIAttributeReferenceDocumentation | [CIEdgePreserveUpsampleFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEdgePreserveUpsampleFilter) |
| inputLumaSigma | CIAttributeMax = 1;<br/>CIAttributeDisplayName = Luma Sigma;<br/>CIAttributeDefault = 0.15;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar |
| inputSmallImage | CIAttributeDisplayName = Small Image;<br/>CIAttributeClass = Image |
| inputSpatialSigma | CIAttributeMax = 5;<br/>CIAttributeDisplayName = Spatial Sigma;<br/>CIAttributeDefault = 3;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIColorMatrix:
| Attribute | Value |
| ---------- | --------- |
| inputGVector | CIAttributeDisplayName = Green Vector;<br/>CIAttributeDescription = The amount of green to multiply the source color values by.;<br/>CIAttributeIdentity = [0 1 0 0];<br/>CIAttributeDefault = [0 1 0 0];<br/>CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputBiasVector | CIAttributeDisplayName = Bias Vector;<br/>CIAttributeDescription = A vector that’s added to each color component.;<br/>CIAttributeIdentity = [0 0 0 0];<br/>CIAttributeDefault = [0 0 0 0];<br/>CIAttributeClass = Vector |
| inputRVector | CIAttributeDisplayName = Red Vector;<br/>CIAttributeDescription = The amount of red to multiply the source color values by.;<br/>CIAttributeIdentity = [1 0 0 0];<br/>CIAttributeDefault = [1 0 0 0];<br/>CIAttributeClass = Vector |
| CIAttributeFilterDisplayName | Color Matrix |
| CIAttributeFilterName | CIColorMatrix |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeReferenceDocumentation | [CIColorMatrix Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorMatrix) |
| inputAVector | CIAttributeDisplayName = Alpha Vector;<br/>CIAttributeDescription = The amount of alpha to multiply the source color values by.;<br/>CIAttributeIdentity = [0 0 0 1];<br/>CIAttributeDefault = [0 0 0 1];<br/>CIAttributeClass = Vector |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| inputBVector | CIAttributeDisplayName = Blue Vector;<br/>CIAttributeDescription = The amount of blue to multiply the source color values by.;<br/>CIAttributeIdentity = [0 0 1 0];<br/>CIAttributeDefault = [0 0 1 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CISampleNearest:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Sample Nearest |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISampleNearest |
| CIAttributeReferenceDocumentation | [CISampleNearest Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISampleNearest) |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIHoleDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Hole Distortion |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHoleDistortion |
| CIAttributeReferenceDocumentation | [CIHoleDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHoleDistortion) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 150;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeMin = 0.01;<br/>CIAttributeIdentity = 0.1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.01 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIExclusionBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Exclusion Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIExclusionBlendMode |
| CIAttributeReferenceDocumentation | [CIExclusionBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIExclusionBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIGlassDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Glass Distortion |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIGlassDistortion |
| CIAttributeReferenceDocumentation | [CIGlassDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGlassDistortion) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of texturing of the resulting image. The larger the value, the greater the texturing.;<br/>CIAttributeDefault = 200;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 500;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.01 |
| inputTexture | CIAttributeDisplayName = Texture;<br/>CIAttributeDescription = A texture to apply to the source image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDepthBlurEffect:
| Attribute | Value |
| ---------- | --------- |
| inputNosePositions | CIAttributeDisplayName = Nose Positions;<br/>CIAttributeDefault = [-1 -1];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputCalibrationData | CIAttributeDisplayName = Calibration Data;<br/>CIAttributeClass = AVCameraCalibrationData |
| CIAttributeFilterName | CIDepthBlurEffect |
| inputChinPositions | CIAttributeDisplayName = Chin Positions;<br/>CIAttributeDefault = [-1 -1];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.13 |
| CIAttributeFilterAvailable_iOS | 11 |
| inputLumaNoiseScale | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 0.1;<br/>CIAttributeDisplayName = Luma Noise Scale;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 0.1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputDisparityImage | CIAttributeDisplayName = Disparity Image;<br/>CIAttributeClass = Image |
| inputScaleFactor | CIAttributeDisplayName = Scale Factor;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeDefault = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 1 |
| inputMatteImage | CIAttributeDescription = A matting image.;<br/>CIAttributeDisplayName = Matte Image;<br/>CIAttributeClass = Image |
| inputLeftEyePositions | CIAttributeDisplayName = Left Eye Positions;<br/>CIAttributeDefault = [-1 -1];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeReferenceDocumentation | [CIDepthBlurEffect Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDepthBlurEffect) |
| inputShape | CIAttributeDisplayName = Shape;<br/>CIAttributeClass = NSString |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputRightEyePositions | CIAttributeDisplayName = Right Eye Positions;<br/>CIAttributeDefault = [-1 -1];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputAuxDataMetadata | CIAttributeDisplayName = Aux Data Metadata;<br/>CIAttributeClass = CGImageMetadataRef |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterDisplayName | Depth Blur Effect |
| inputFocusRect | CIAttributeDisplayName = Focus Rectangle;<br/>CIAttributeIdentity = [-8.98847e+307 -8.98847e+307 1.79769e+308 1.79769e+308];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| inputAperture | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 22;<br/>CIAttributeDisplayName = Aperture;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 22;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |


#### CIDither:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Dither |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDither |
| CIAttributeReferenceDocumentation | [CIDither Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDither) |
| inputIntensity | CIAttributeDefault = 0.1;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the effect.;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 5;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIAreaMinimumAlpha:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Minimum Alpha |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinimumAlpha |
| CIAttributeReferenceDocumentation | [CIAreaMinimumAlpha Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinimumAlpha) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIDroste:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.6 |
| inputZoom | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 1;<br/>CIAttributeSliderMax = 5;<br/>CIAttributeDisplayName = Zoom;<br/>CIAttributeMin = 0.01;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.01 |
| inputInsetPoint1 | CIAttributeDisplayName = Inset Point 1;<br/>CIAttributeDefault = [400 400];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterName | CIDroste |
| CIAttributeFilterDisplayName | Droste |
| inputRotation | CIAttributeDisplayName = Rotation;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeDefault = 0;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 6.283185307179586 |
| CIAttributeFilterAvailable_iOS | 9 |
| inputStrands | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 1;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeDisplayName = Strands;<br/>CIAttributeMin = -10;<br/>CIAttributeMax = 10;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -2 |
| CIAttributeReferenceDocumentation | [CIDroste Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDroste) |
| inputPeriodicity | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 1;<br/>CIAttributeSliderMax = 5;<br/>CIAttributeDisplayName = Periodicity;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |
| inputInsetPoint0 | CIAttributeDisplayName = Inset Point 0;<br/>CIAttributeDefault = [200 200];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIFourfoldTranslatedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Fourfold Translated Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIFourfoldTranslatedTile |
| CIAttributeReferenceDocumentation | [CIFourfoldTranslatedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFourfoldTranslatedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputAcuteAngle | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The primary angle for the repeating translated tile. Small values create thin diamond tiles, and higher values create fatter translated tiles.;<br/>CIAttributeDefault = 1.570796326794897;<br/>CIAttributeDisplayName = Acute Angle;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeIdentity = 1.570796326794897;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIDepthOfField:
| Attribute | Value |
| ---------- | --------- |
| inputPoint0 | CIAttributeDisplayName = Point 0;<br/>CIAttributeDefault = [0 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.6 |
| inputPoint1 | CIAttributeDisplayName = Point 1;<br/>CIAttributeDefault = [300 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterName | CIDepthOfField |
| CIAttributeFilterDisplayName | Depth of Field |
| inputUnsharpMaskRadius | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeDefault = 2.5;<br/>CIAttributeDisplayName = Unsharp Mask Radius;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputSaturation | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount to adjust the saturation.;<br/>CIAttributeDefault = 1.5;<br/>CIAttributeDisplayName = Saturation;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIDepthOfField Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDepthOfField) |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputUnsharpMaskIntensity | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Unsharp Mask Intensity;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance from the center of the effect.;<br/>CIAttributeDefault = 6;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 30;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CITriangleTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Triangle Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CITriangleTile |
| CIAttributeReferenceDocumentation | [CITriangleTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITriangleTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISaliencyMapFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Saliency Map Filter |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryStylize |
| CIAttributeFilterName | CISaliencyMapFilter |
| CIAttributeReferenceDocumentation | [CISaliencyMapFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISaliencyMapFilter) |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CISaturationBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Saturation Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISaturationBlendMode |
| CIAttributeReferenceDocumentation | [CISaturationBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISaturationBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISourceAtopCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source Atop |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISourceAtopCompositing |
| CIAttributeReferenceDocumentation | [CISourceAtopCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceAtopCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColumnAverage:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Column Average |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColumnAverage |
| CIAttributeReferenceDocumentation | [CIColumnAverage Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColumnAverage) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIFourfoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Fourfold Reflected Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIFourfoldReflectedTile |
| CIAttributeReferenceDocumentation | [CIFourfoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFourfoldReflectedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputAcuteAngle | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The primary angle for the repeating reflected tile. Small values create thin diamond tiles, and higher values create fatter reflected tiles.;<br/>CIAttributeDefault = 1.570796326794897;<br/>CIAttributeDisplayName = Acute Angle;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeIdentity = 1.570796326794897;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIShadedMaterial:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Shaded Material |
| inputShadingImage | CIAttributeDisplayName = Shading Image;<br/>CIAttributeDescription = The image to use as the height field. The resulting image has greater heights with lighter shades, and lesser heights (lower areas) with darker shades.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIShadedMaterial |
| CIAttributeReferenceDocumentation | [CIShadedMaterial Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIShadedMaterial) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scale of the effect. The higher the value, the more dramatic the effect.;<br/>CIAttributeDefault = 10;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.5 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CITwelvefoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Twelvefold Reflected Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CITwelvefoldReflectedTile |
| CIAttributeReferenceDocumentation | [CITwelvefoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITwelvefoldReflectedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIMaximumCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Maximum |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMaximumCompositing |
| CIAttributeReferenceDocumentation | [CIMaximumCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaximumCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBoxBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Box Blur |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBoxBlur |
| CIAttributeReferenceDocumentation | [CIBoxBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBoxBlur) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;<br/>CIAttributeDefault = 10;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIBumpDistortionLinear:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Bump Distortion Linear |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 6.283185307179586;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the line around which the distortion occurs.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBumpDistortionLinear |
| CIAttributeReferenceDocumentation | [CIBumpDistortionLinear Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBumpDistortionLinear) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scale of the effect.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = -1;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 600;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIGaussianBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Gaussian Blur |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIGaussianBlur |
| CIAttributeReferenceDocumentation | [CIGaussianBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGaussianBlur) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;<br/>CIAttributeDefault = 10;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVibrance:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Vibrance |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIVibrance |
| CIAttributeReferenceDocumentation | [CIVibrance Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVibrance) |
| inputAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount to adjust the saturation.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Amount;<br/>CIAttributeSliderMin = -1;<br/>CIAttributeMin = -1;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIMorphologyMaximum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Morphology Maximum |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMorphologyMaximum |
| CIAttributeReferenceDocumentation | [CIMorphologyMaximum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMorphologyMaximum) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The desired radius of the circular morphological operation to the image.;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIPhotoEffectInstant:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Instant |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectInstant |
| CIAttributeReferenceDocumentation | [CIPhotoEffectInstant Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectInstant) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIColorMap:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Color Map |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorMap |
| CIAttributeReferenceDocumentation | [CIColorMap Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorMap) |
| inputGradientImage | CIAttributeDisplayName = Gradient Image;<br/>CIAttributeDescription = The image data from this image transforms the source image values.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeGradient |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPageCurlTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the curling page.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| CIAttributeFilterName | CIPageCurlTransition |
| CIAttributeFilterDisplayName | Page Curl |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = The extent of the effect.;<br/>CIAttributeDefault = [0 0 300 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| inputShadingImage | CIAttributeDisplayName = Shading Image;<br/>CIAttributeDescription = An image that looks like a shaded sphere enclosed in a square image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIPageCurlTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPageCurlTransition) |
| inputBacksideImage | CIAttributeDescription = The image that appears on the back of the source image, as the page curls to reveal the target image.;<br/>CIAttributeDisplayName = Backside Image;<br/>CIAttributeClass = Image |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the curl.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 400;<br/>CIAttributeMin = 0.01;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.01 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIStripesGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Stripes |
| inputColor1 | CIAttributeDisplayName = Color 2;<br/>CIAttributeDescription = A color to use for the even stripes.;<br/>CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIStripesGenerator |
| inputColor0 | CIAttributeDisplayName = Color 1;<br/>CIAttributeDescription = A color to use for the odd stripes.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| CIAttributeReferenceDocumentation | [CIStripesGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStripesGenerator) |
| inputWidth | CIAttributeDefault = 80;<br/>CIAttributeDescription = The width of a stripe.;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The sharpness of the stripe pattern. The smaller the value, the more blurry the pattern. Values range from 0.0 to 1.0.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the stripe pattern.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAreaMinMaxRed:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Area Min and Max Red |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinMaxRed |
| CIAttributeReferenceDocumentation | [CIAreaMinMaxRed Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinMaxRed) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CICircularScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Circular Screen |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryHalftoneEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICircularScreen |
| CIAttributeReferenceDocumentation | [CICircularScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICircularScreen) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance between each circle in the pattern.;<br/>CIAttributeDefault = 6;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 2 |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The sharpness of the circles. The larger the value, the sharper the circles.;<br/>CIAttributeDefault = 0.7;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the circular screen pattern;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILightTunnel:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Light Tunnel Distortion |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILightTunnel |
| CIAttributeReferenceDocumentation | [CILightTunnel Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILightTunnel) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Center radius of the light tunnel.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 500;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputRotation | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Rotation angle of the light tunnel.;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = Rotation;<br/>CIAttributeSliderMax = 1.570796326794897;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = Center of the light tunnel.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMultiplyBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Multiply Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMultiplyBlendMode |
| CIAttributeReferenceDocumentation | [CIMultiplyBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMultiplyBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorControls:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Controls |
| inputSaturation | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of saturation to apply. The larger the value, the more saturated the result.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Saturation;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorControls |
| CIAttributeReferenceDocumentation | [CIColorControls Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorControls) |
| inputBrightness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of brightness to apply. The larger the value, the brighter the result.;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = Brightness;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = -1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -1 |
| inputContrast | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of contrast to apply. The larger the value, the more contrast in the resulting image.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Contrast;<br/>CIAttributeSliderMax = 4;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.25 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CITextImageGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Text Image Generator |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputText | CIAttributeDisplayName = Text;<br/>CIAttributeClass = NSString |
| CIAttributeFilterName | CITextImageGenerator |
| CIAttributeReferenceDocumentation | [CITextImageGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITextImageGenerator) |
| inputFontName | CIAttributeDefault = HelveticaNeue;<br/>CIAttributeDisplayName = Font Name;<br/>CIAttributeClass = NSString |
| inputScaleFactor | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 4;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Scale Factor;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |
| inputFontSize | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 128;<br/>CIAttributeDefault = 12;<br/>CIAttributeDisplayName = Font Size;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 9 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILinearToSRGBToneCurve:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Linear to sRGB Tone Curve |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILinearToSRGBToneCurve |
| CIAttributeReferenceDocumentation | [CILinearToSRGBToneCurve Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearToSRGBToneCurve) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIColorPolynomial:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Polynomial |
| inputRedCoefficients | CIAttributeDisplayName = Red Coefficients;<br/>CIAttributeDescription = Polynomial coefficients for red channel;<br/>CIAttributeIdentity = [0 1 0 0];<br/>CIAttributeDefault = [0 1 0 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorPolynomial |
| CIAttributeReferenceDocumentation | [CIColorPolynomial Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorPolynomial) |
| inputGreenCoefficients | CIAttributeDisplayName = Green Coefficients;<br/>CIAttributeDescription = Polynomial coefficients for green channel;<br/>CIAttributeIdentity = [0 1 0 0];<br/>CIAttributeDefault = [0 1 0 0];<br/>CIAttributeClass = Vector |
| inputAlphaCoefficients | CIAttributeDisplayName = Alpha Coefficients;<br/>CIAttributeDescription = Polynomial coefficients for alpha channel;<br/>CIAttributeIdentity = [0 1 0 0];<br/>CIAttributeDefault = [0 1 0 0];<br/>CIAttributeClass = Vector |
| inputBlueCoefficients | CIAttributeDisplayName = Blue Coefficients;<br/>CIAttributeDescription = Polynomial coefficients for blue channel;<br/>CIAttributeIdentity = [0 1 0 0];<br/>CIAttributeDefault = [0 1 0 0];<br/>CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIConstantColorGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Constant Color |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIConstantColorGenerator |
| CIAttributeReferenceDocumentation | [CIConstantColorGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConstantColorGenerator) |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The color to generate.;<br/>CIAttributeDefault = (1 0 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIGlassLozenge:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Glass Lozenge |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIGlassLozenge |
| CIAttributeReferenceDocumentation | [CIGlassLozenge Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGlassLozenge) |
| inputPoint1 | CIAttributeDisplayName = Point 1;<br/>CIAttributeDescription = The x and y position that defines the center of the circle at the other end of the lozenge.;<br/>CIAttributeDefault = [350 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the lozenge. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeSliderMax = 1000;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeDefault = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputRefraction | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The refraction of the glass.;<br/>CIAttributeSliderMax = 5;<br/>CIAttributeDisplayName = Refraction;<br/>CIAttributeDefault = 1.7;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputPoint0 | CIAttributeDisplayName = Point 0;<br/>CIAttributeDescription = The x and y position that defines the center of the circle at one end of the lozenge.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISixfoldRotatedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Sixfold Rotated Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISixfoldRotatedTile |
| CIAttributeReferenceDocumentation | [CISixfoldRotatedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISixfoldRotatedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CICopyMachineTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The color of the copier light.;<br/>CIAttributeDefault = (0.6 1 0.8 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeOpaqueColor |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 6.283185307179586;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the copier light.;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of the copier light. ;<br/>CIAttributeDefault = 200;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 500;<br/>CIAttributeMin = 0.1;<br/>CIAttributeIdentity = 200;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.1 |
| CIAttributeFilterName | CICopyMachineTransition |
| CIAttributeFilterDisplayName | Copy Machine |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that defines the extent of the effect.;<br/>CIAttributeDefault = [0 0 300 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CICopyMachineTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICopyMachineTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputOpacity | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The opacity of the copier light. A value of 0.0 is transparent. A value of 1.0 is opaque.;<br/>CIAttributeDefault = 1.3;<br/>CIAttributeDisplayName = Opacity;<br/>CIAttributeSliderMax = 3;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1.3;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIGloom:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Gloom |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIGloom |
| CIAttributeReferenceDocumentation | [CIGloom Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGloom) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the effect. The larger the radius, the greater the effect.;<br/>CIAttributeDefault = 10;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputIntensity | CIAttributeDefault = 0.5;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the effect. A value of 0.0 is no effect. A value of 1.0 is the maximum effect.;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISpotColor:
| Attribute | Value |
| ---------- | --------- |
| inputCenterColor2 | CIAttributeDisplayName = Center Color 2;<br/>CIAttributeDescription = The center value of the second color range to replace.;<br/>CIAttributeDefault = (0.5255 0.3059 0.3451 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| CIAttributeFilterAvailable_Mac | 10.5 |
| inputCloseness2 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = A value that indicates how close the second color must match before it is replaced.;<br/>CIAttributeDefault = 0.15;<br/>CIAttributeDisplayName = Closeness 2;<br/>CIAttributeSliderMax = 0.5;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputContrast1 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The contrast of the first replacement color.;<br/>CIAttributeDefault = 0.98;<br/>CIAttributeDisplayName = Contrast 1;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenterColor1 | CIAttributeDisplayName = Center Color 1;<br/>CIAttributeDescription = The center value of the first color range to replace.;<br/>CIAttributeDefault = (0.0784 0.0627 0.0706 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| inputCloseness3 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = A value that indicates how close the third color must match before it is replaced.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Closeness 3;<br/>CIAttributeSliderMax = 0.5;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputContrast3 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The contrast of the third replacement color.;<br/>CIAttributeDefault = 0.99;<br/>CIAttributeDisplayName = Contrast 3;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CISpotColor |
| CIAttributeFilterDisplayName | Spot Color |
| inputCloseness1 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = A value that indicates how close the first color must match before it is replaced.;<br/>CIAttributeDefault = 0.22;<br/>CIAttributeDisplayName = Closeness 1;<br/>CIAttributeSliderMax = 0.5;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputContrast2 | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The contrast of the second replacement color.;<br/>CIAttributeDefault = 0.98;<br/>CIAttributeDisplayName = Contrast 2;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CISpotColor Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISpotColor) |
| inputReplacementColor1 | CIAttributeDisplayName = Replacement Color 1;<br/>CIAttributeDescription = A replacement color for the first color range.;<br/>CIAttributeDefault = (0.4392 0.1922 0.1961 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| CIAttributeFilterCategories | CICategoryBuiltIn;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryStylize |
| inputReplacementColor2 | CIAttributeDisplayName = Replacement Color 2;<br/>CIAttributeDescription = A replacement color for the second color range.;<br/>CIAttributeDefault = (0.9137 0.5608 0.5059 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| inputCenterColor3 | CIAttributeDisplayName = Center Color 3;<br/>CIAttributeDescription = The center value of the third color range to replace.;<br/>CIAttributeDefault = (0.9216 0.4549 0.3333 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| inputReplacementColor3 | CIAttributeDisplayName = Replacement Color 3;<br/>CIAttributeDescription = A replacement color for the third color range.;<br/>CIAttributeDefault = (0.9098 0.7529 0.6078 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIAreaMinimum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Minimum |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinimum |
| CIAttributeReferenceDocumentation | [CIAreaMinimum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinimum) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CICrystallize:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Crystallize |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICrystallize |
| CIAttributeReferenceDocumentation | [CICrystallize Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICrystallize) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the effect. The larger the radius, the larger the resulting crystals.;<br/>CIAttributeDefault = 20;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 1;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorDodgeBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Dodge Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorDodgeBlendMode |
| CIAttributeReferenceDocumentation | [CIColorDodgeBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorDodgeBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIWhitePointAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | White Point Adjust |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIWhitePointAdjust |
| CIAttributeReferenceDocumentation | [CIWhitePointAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIWhitePointAdjust) |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = A color to use as the white point.;<br/>CIAttributeIdentity = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILinearDodgeBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Linear Dodge Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILinearDodgeBlendMode |
| CIAttributeReferenceDocumentation | [CILinearDodgeBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearDodgeBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CILinearBurnBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Linear Burn Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILinearBurnBlendMode |
| CIAttributeReferenceDocumentation | [CILinearBurnBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearBurnBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIClamp:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Clamp |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIClamp |
| CIAttributeReferenceDocumentation | [CIClamp Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIClamp) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that defines the extent of the effect.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIPhotoEffectTonal:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Tonal |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectTonal |
| CIAttributeReferenceDocumentation | [CIPhotoEffectTonal Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectTonal) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIDissolveTransition:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Dissolve |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDissolveTransition |
| CIAttributeReferenceDocumentation | [CIDissolveTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDissolveTransition) |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHardLightBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Hard Light Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHardLightBlendMode |
| CIAttributeReferenceDocumentation | [CIHardLightBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHardLightBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPageCurlWithShadowTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.9 |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the curling page.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputShadowSize | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The maximum size in pixels of the shadow.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Shadow Size;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputShadowAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The strength of the shadow.;<br/>CIAttributeDefault = 0.7;<br/>CIAttributeDisplayName = Shadow Amount;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputShadowExtent | CIAttributeDisplayName = Shadow Extent;<br/>CIAttributeDescription = The rectagular portion of input image that will cast a shadow.;<br/>CIAttributeDefault = [0 0 0 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterName | CIPageCurlWithShadowTransition |
| CIAttributeFilterDisplayName | Page Curl With Shadow |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = The extent of the effect.;<br/>CIAttributeDefault = [0 0 0 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIPageCurlWithShadowTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPageCurlWithShadowTransition) |
| inputBacksideImage | CIAttributeDescription = The image that appears on the back of the source image, as the page curls to reveal the target image.;<br/>CIAttributeDisplayName = Backside Image;<br/>CIAttributeClass = Image |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the curl.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 400;<br/>CIAttributeMin = 0.01;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.01 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIGaussianGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Gaussian Gradient |
| inputColor1 | CIAttributeDisplayName = Color 2;<br/>CIAttributeDescription = The second color to use in the gradient.;<br/>CIAttributeDefault = (0 0 0 0) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterCategories | CICategoryGradient;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIGaussianGradient |
| inputColor0 | CIAttributeDisplayName = Color 1;<br/>CIAttributeDescription = The first color to use in the gradient.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeReferenceDocumentation | [CIGaussianGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGaussianGradient) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the Gaussian distribution.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBlendWithBlueMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Blend With Blue Mask |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithBlueMask |
| CIAttributeReferenceDocumentation | [CIBlendWithBlueMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithBlueMask) |
| inputMaskImage | CIAttributeDisplayName = Mask Image;<br/>CIAttributeDescription = A masking image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIHueAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Hue Adjust |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = An angle (in radians) to use to correct the hue of an image.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHueAdjust |
| CIAttributeReferenceDocumentation | [CIHueAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHueAdjust) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMorphologyMinimum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Morphology Minimum |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMorphologyMinimum |
| CIAttributeReferenceDocumentation | [CIMorphologyMinimum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMorphologyMinimum) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The desired radius of the circular morphological operation to the image.;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIStretchCrop:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Stretch Crop |
| inputCenterStretchAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Determine how much the center of the image is stretched if stretching is used. If value is 0 then the center of the image maintains the original aspect ratio. If 1 then the image is stretched uniformly.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Center Stretch Amount;<br/>CIAttributeDefault = 0.25;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIStretchCrop |
| CIAttributeReferenceDocumentation | [CIStretchCrop Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStretchCrop) |
| inputCropAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Determines if and how much cropping should be used to achieve the target size. If value is 0 then only stretching is used. If 1 then only cropping is used.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Crop Amount;<br/>CIAttributeDefault = 0.25;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputSize | CIAttributeDisplayName = Size;<br/>CIAttributeDescription = The size in pixels of the output image.;<br/>CIAttributeDefault = [1280 720];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.6 |


#### CIBarsSwipeTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.5 |
| inputAngle | CIAttributeDefault = 3.141592653589793;<br/>CIAttributeSliderMax = 6.283185307179586;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the bars.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = 0 |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of each bar.;<br/>CIAttributeDefault = 30;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 300;<br/>CIAttributeMin = 2;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 2 |
| CIAttributeFilterName | CIBarsSwipeTransition |
| CIAttributeFilterDisplayName | Bars Swipe Transition |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIBarsSwipeTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBarsSwipeTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputBarOffset | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The offset of one bar with respect to another;<br/>CIAttributeDefault = 10;<br/>CIAttributeDisplayName = Bar Offset;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIEightfoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Eightfold Reflected Tile |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the tiled pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIEightfoldReflectedTile |
| CIAttributeReferenceDocumentation | [CIEightfoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEightfoldReflectedTile) |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of a tile.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 100;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CITemperatureAndTint:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Temperature and Tint |
| inputTargetNeutral | CIAttributeIdentity = [6500 0];<br/>CIAttributeDisplayName = Target Neutral;<br/>CIAttributeDefault = [6500 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CITemperatureAndTint |
| CIAttributeReferenceDocumentation | [CITemperatureAndTint Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITemperatureAndTint) |
| inputNeutral | CIAttributeIdentity = [6500 0];<br/>CIAttributeDisplayName = Neutral;<br/>CIAttributeDefault = [6500 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIConvolution9Vertical:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Vertical 9 Convolution |
| inputWeights | CIAttributeDisplayName = Weights;<br/>CIAttributeIdentity = [0 0 0 0 1 0 0 0 0];<br/>CIAttributeDefault = [0 0 0 0 1 0 0 0 0];<br/>CIAttributeClass = Vector |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution9Vertical |
| CIAttributeReferenceDocumentation | [CIConvolution9Vertical Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution9Vertical) |
| inputBias | CIAttributeDisplayName = Bias;<br/>CIAttributeIdentity = 0;<br/>CIAttributeDefault = 0;<br/>CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIGammaAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Gamma Adjust |
| inputPower | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = A gamma value to use to correct image brightness. The larger the value, the darker the result.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Power;<br/>CIAttributeSliderMax = 4;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.25 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIGammaAdjust |
| CIAttributeReferenceDocumentation | [CIGammaAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGammaAdjust) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIZoomBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8.3 |
| CIAttributeFilterDisplayName | Zoom Blur |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIZoomBlur |
| CIAttributeReferenceDocumentation | [CIZoomBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIZoomBlur) |
| inputAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The zoom-in amount. Larger values result in more zooming in.;<br/>CIAttributeDefault = 20;<br/>CIAttributeDisplayName = Amount;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = -200 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVignette:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Vignette |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIVignette |
| CIAttributeReferenceDocumentation | [CIVignette Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVignette) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance from the center of the effect.;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 2;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputIntensity | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the effect.;<br/>CIAttributeMin = -1;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -1 |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIAccordionFoldTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputNumberOfFolds | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 3;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeDisplayName = Number of Folds;<br/>CIAttributeMin = 1;<br/>CIAttributeMax = 50;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The duration of the effect.;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |
| CIAttributeFilterName | CIAccordionFoldTransition |
| CIAttributeFilterDisplayName | Accordion Fold Transition |
| inputBottomHeight | CIAttributeDisplayName = Bottom Height;<br/>CIAttributeMin = 0;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 0;<br/>CIAttributeType = CIAttributeTypeDistance |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeReferenceDocumentation | [CIAccordionFoldTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAccordionFoldTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputFoldShadowAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 0.1;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Fold Shadow Amount;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CISunbeamsGenerator:
| Attribute | Value |
| ---------- | --------- |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The duration of the effect.;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0 |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The color of the sun.;<br/>CIAttributeDefault = (1 0.5 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| inputStriationStrength | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The intensity of the sunbeams. Higher values result in more intensity.;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeDisplayName = Striation Strength;<br/>CIAttributeSliderMax = 3;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0.5;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CISunbeamsGenerator |
| CIAttributeFilterDisplayName | Sunbeams |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the sunbeam pattern;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 9 |
| inputStriationContrast | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The contrast of the sunbeams. Higher values result in more contrast.;<br/>CIAttributeDefault = 1.375;<br/>CIAttributeDisplayName = Striation Contrast;<br/>CIAttributeSliderMax = 5;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1.375;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CISunbeamsGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISunbeamsGenerator) |
| inputSunRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the sun.;<br/>CIAttributeDefault = 40;<br/>CIAttributeDisplayName = Sun Radius;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 40;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputMaxStriationRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the sunbeams.;<br/>CIAttributeDefault = 2.58;<br/>CIAttributeDisplayName = Maximum Striation Radius;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 2.58;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMaskedVariableBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Masked Variable Blur |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMaskedVariableBlur |
| CIAttributeReferenceDocumentation | [CIMaskedVariableBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaskedVariableBlur) |
| inputMask | CIAttributeDisplayName = Mask;<br/>CIAttributeClass = Image |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance from the center of the effect.;<br/>CIAttributeDefault = 5;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIPinLightBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Pin Light Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIPinLightBlendMode |
| CIAttributeReferenceDocumentation | [CIPinLightBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPinLightBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMaskToAlpha:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Mask to Alpha |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMaskToAlpha |
| CIAttributeReferenceDocumentation | [CIMaskToAlpha Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaskToAlpha) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CINinePartStretched:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Nine Part Stretched |
| inputGrowAmount | CIAttributeDisplayName = Grow Amount;<br/>CIAttributeDefault = [100 100];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CINinePartStretched |
| CIAttributeReferenceDocumentation | [CINinePartStretched Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CINinePartStretched) |
| inputBreakpoint0 | CIAttributeDisplayName = Breakpoint0;<br/>CIAttributeDescription = Lower left corner of image to retain before stretching begins.;<br/>CIAttributeDefault = [50 50];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputBreakpoint1 | CIAttributeDisplayName = Breakpoint1;<br/>CIAttributeDescription = Upper right corner of image to retain after stretching ends.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIScreenBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Screen Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIScreenBlendMode |
| CIAttributeReferenceDocumentation | [CIScreenBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIScreenBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVignetteEffect:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Vignette Effect |
| inputIntensity | CIAttributeDefault = 1;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Intensity;<br/>CIAttributeDescription = The intensity of the effect.;<br/>CIAttributeMin = -1;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -1 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIVignetteEffect |
| CIAttributeReferenceDocumentation | [CIVignetteEffect Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVignetteEffect) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance from the center of the effect.;<br/>CIAttributeDefault = 150;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 2000;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputFalloff | CIAttributeClass = NSNumber;<br/>CIAttributeDefault = 0.5;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Falloff;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIRandomGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterDisplayName | Random Generator |
| CIAttributeFilterAvailable_Mac | 10.4 |
| CIAttributeReferenceDocumentation | [CIRandomGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRandomGenerator) |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIRandomGenerator |


#### CIDisintegrateWithMaskTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputMaskImage | CIAttributeDisplayName = Mask Image;<br/>CIAttributeDescription = An image that defines the shape to use when disintegrating from the source to the target image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterName | CIDisintegrateWithMaskTransition |
| CIAttributeFilterDisplayName | Disintegrate With Mask |
| inputShadowOffset | CIAttributeDisplayName = Shadow Offset;<br/>CIAttributeDescription = The offset of the shadow created by the mask.;<br/>CIAttributeIdentity = [0 0];<br/>CIAttributeDefault = [0 -10];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeOffset |
| inputShadowDensity | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The density of the shadow created by the mask.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Shadow Density;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0.65 |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIDisintegrateWithMaskTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDisintegrateWithMaskTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputShadowRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the shadow created by the mask.;<br/>CIAttributeDefault = 8;<br/>CIAttributeDisplayName = Shadow Radius;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIMultiplyCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Multiply |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMultiplyCompositing |
| CIAttributeReferenceDocumentation | [CIMultiplyCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMultiplyCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Perspective Tile |
| inputTopRight | CIAttributeDisplayName = Top Right;<br/>CIAttributeDescription = The top right coordinate of a tile.;<br/>CIAttributeDefault = [646 507];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryTileEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIPerspectiveTile |
| CIAttributeReferenceDocumentation | [CIPerspectiveTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveTile) |
| inputBottomLeft | CIAttributeDisplayName = Bottom Left;<br/>CIAttributeDescription = The bottom left coordinate of a tile.;<br/>CIAttributeDefault = [155 153];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputTopLeft | CIAttributeDisplayName = Top Left;<br/>CIAttributeDescription = The top left coordinate of a tile.;<br/>CIAttributeDefault = [118 484];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputBottomRight | CIAttributeDisplayName = Bottom Right;<br/>CIAttributeDescription = The bottom right coordinate of a tile.;<br/>CIAttributeDefault = [548 140];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILineOverlay:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.5 |
| inputNRNoiseLevel | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The noise level of the image (used with camera data) that gets removed before tracing the edges of the image. Increasing the noise level helps to clean up the traced edges of the image.;<br/>CIAttributeSliderMax = 0.1;<br/>CIAttributeDisplayName = NR Noise Level;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0.07000000000000001 |
| inputContrast | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of anti-aliasing to use on the edges produced by this filter. Higher values produce higher contrast edges (they are less anti-aliased).;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeDisplayName = Contrast;<br/>CIAttributeSliderMin = 0.25;<br/>CIAttributeMin = 0.25;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 50 |
| inputThreshold | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = This value determines edge visibility. Larger values thin out the edges.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Threshold;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0.1 |
| CIAttributeFilterName | CILineOverlay |
| CIAttributeFilterDisplayName | Line Overlay |
| inputEdgeIntensity | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The accentuation factor of the Sobel gradient information when tracing the edges of the image. Higher values find more edges, although typically a low value (such as 1.0) is used.;<br/>CIAttributeSliderMax = 200;<br/>CIAttributeDisplayName = Edge Intensity;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 1 |
| CIAttributeFilterAvailable_iOS | 9 |
| inputNRSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of sharpening done when removing noise in the image before tracing the edges of the image. This improves the edge acquisition.;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeDisplayName = NR Sharpness;<br/>CIAttributeSliderMin = 0;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0.71 |
| CIAttributeReferenceDocumentation | [CILineOverlay Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILineOverlay) |
| CIAttributeFilterCategories | CICategoryBuiltIn;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryStylize |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIColorCube:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Cube |
| inputCubeDimension | CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Cube Dimension;<br/>CIAttributeMin = 2;<br/>CIAttributeMax = 128;<br/>CIAttributeIdentity = 2;<br/>CIAttributeType = CIAttributeTypeCount;<br/>CIAttributeDefault = 2 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCube |
| CIAttributeReferenceDocumentation | [CIColorCube Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCube) |
| inputCubeData | CIAttributeDisplayName = Cube Data;<br/>CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;<br/>CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeClass = NSData |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILuminosityBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Luminosity Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILuminosityBlendMode |
| CIAttributeReferenceDocumentation | [CILuminosityBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILuminosityBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISwipeTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The color of the swipe.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeOpaqueColor |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the swipe.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of the swipe;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 0.1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.1 |
| CIAttributeFilterName | CISwipeTransition |
| CIAttributeFilterDisplayName | Swipe |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = The extent of the effect.;<br/>CIAttributeDefault = [0 0 300 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CISwipeTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISwipeTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputOpacity | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The opacity of the swipe.;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = Opacity;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIPixellate:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Pixelate |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIPixellate |
| CIAttributeReferenceDocumentation | [CIPixellate Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPixellate) |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The scale determines the size of the squares. Larger values result in larger squares.;<br/>CIAttributeDefault = 8;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIExposureAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Exposure Adjust |
| inputEV | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount to adjust the exposure of the image by. The larger the value, the brighter the exposure.;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = EV;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -10 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIExposureAdjust |
| CIAttributeReferenceDocumentation | [CIExposureAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIExposureAdjust) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILinearGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Linear Gradient |
| inputColor1 | CIAttributeDisplayName = Color 2;<br/>CIAttributeDescription = The second color to use in the gradient.;<br/>CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterCategories | CICategoryGradient;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILinearGradient |
| inputColor0 | CIAttributeDisplayName = Color 1;<br/>CIAttributeDescription = The first color to use in the gradient.;<br/>CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color;<br/>CIAttributeType = CIAttributeTypeColor |
| CIAttributeReferenceDocumentation | [CILinearGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearGradient) |
| inputPoint1 | CIAttributeDisplayName = Point 1;<br/>CIAttributeDescription = The ending position of the gradient -- where the second color begins.;<br/>CIAttributeDefault = [200 200];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| inputPoint0 | CIAttributeDisplayName = Point 0;<br/>CIAttributeDescription = The starting position of the gradient -- where the first color begins.;<br/>CIAttributeDefault = [0 0];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CICMYKHalftone:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the pattern.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The sharpness of the pattern. The larger the value, the sharper the pattern.;<br/>CIAttributeDefault = 0.7;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 1;<br/>CIUIParameterSet = CIUISetBasic;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance between dots in the pattern.;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMin = 2;<br/>CIUIParameterSet = CIUISetBasic;<br/>CIAttributeMin = -2;<br/>CIAttributeIdentity = 6;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeDefault = 6 |
| inputUCR | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The under color removal value. The value can vary from 0.0 to 1.0. ;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Under Color Removal;<br/>CIAttributeSliderMin = 0;<br/>CIUIParameterSet = CIUISetIntermediate;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0.5;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 0.5 |
| CIAttributeFilterName | CICMYKHalftone |
| CIAttributeFilterDisplayName | CMYK Halftone |
| inputGCR | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The gray component replacement value. The value can vary from 0.0 (none) to 1.0.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Gray Component Replacement;<br/>CIAttributeSliderMin = 0;<br/>CIUIParameterSet = CIUISetIntermediate;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeDefault = 1 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the halftone pattern;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CICMYKHalftone Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICMYKHalftone) |
| CIAttributeFilterCategories | CICategoryHalftoneEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CISoftLightBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Soft Light Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISoftLightBlendMode |
| CIAttributeReferenceDocumentation | [CISoftLightBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISoftLightBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIStarShineGenerator:
| Attribute | Value |
| ---------- | --------- |
| inputColor | CIAttributeDisplayName = Color;<br/>CIAttributeDescription = The color to use for the outer shell of the circular star.;<br/>CIAttributeDefault = (1 0.8 0.6 1) <CGColorSpace 0x600002601920> (kCGColorSpaceDeviceRGB);<br/>CIAttributeClass = Color |
| inputCrossScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The size of the cross pattern.;<br/>CIAttributeDefault = 15;<br/>CIAttributeDisplayName = Cross Scale;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 15;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CIStarShineGenerator |
| CIAttributeFilterDisplayName | Star Shine |
| inputCrossWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of the cross pattern.;<br/>CIAttributeDefault = 2.5;<br/>CIAttributeDisplayName = Cross Width;<br/>CIAttributeSliderMax = 10;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0.5 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the star.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| inputCrossOpacity | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The opacity of the cross pattern.;<br/>CIAttributeDefault = -2;<br/>CIAttributeDisplayName = Cross Opacity;<br/>CIAttributeSliderMax = 0;<br/>CIAttributeMin = -8;<br/>CIAttributeIdentity = -2;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -8 |
| CIAttributeReferenceDocumentation | [CIStarShineGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStarShineGenerator) |
| inputCrossAngle | CIAttributeDefault = 0.6;<br/>CIAttributeDescription = The angle of the cross pattern.;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Cross Angle;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius of the star.;<br/>CIAttributeDefault = 50;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 300;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputEpsilon | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The length of the cross spikes.;<br/>CIAttributeDefault = -2;<br/>CIAttributeDisplayName = Epsilon;<br/>CIAttributeSliderMax = 0;<br/>CIAttributeMin = -8;<br/>CIAttributeIdentity = -2;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -8 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CICoreMLModelFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | CoreML Model Filter |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryStylize |
| CIAttributeFilterName | CICoreMLModelFilter |
| CIAttributeReferenceDocumentation | [CICoreMLModelFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICoreMLModelFilter) |
| inputModel | CIAttributeDescription = The CoreML model to be used for applying effect on the image.;<br/>CIAttributeDisplayName = Model;<br/>CIAttributeClass = MLModel |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIBlendWithAlphaMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Blend With Alpha Mask |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithAlphaMask |
| CIAttributeReferenceDocumentation | [CIBlendWithAlphaMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithAlphaMask) |
| inputMaskImage | CIAttributeDisplayName = Mask Image;<br/>CIAttributeDescription = A masking image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIHueSaturationValueGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Hue/Saturation/Value Gradient |
| inputColorSpace | CIAttributeDisplayName = Color Space;<br/>CIAttributeDescription = The CGColorSpaceRef that the color wheel should be generated in.;<br/>CIAttributeDefault = <CGColorSpace 0x6000026019e0> (kCGColorSpaceICCBased; kCGColorSpaceModelRGB; sRGB IEC61966-2.1);<br/>CIAttributeClass = NSObject |
| CIAttributeFilterCategories | CICategoryGradient;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIHueSaturationValueGradient |
| CIAttributeReferenceDocumentation | [CIHueSaturationValueGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHueSaturationValueGradient) |
| inputDither | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 3;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Dither;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputValue | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Value;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance from the center of the effect.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputSoftness | CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDefault = 1;<br/>CIAttributeDisplayName = Softness;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIColorInvert:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Invert |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorInvert |
| CIAttributeReferenceDocumentation | [CIColorInvert Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorInvert) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIRippleTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage | CIAttributeDisplayName = Target Image;<br/>CIAttributeDescription = The target image for a transition.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputTime | CIAttributeSliderMin = 0;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Time;<br/>CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeTime;<br/>CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The width of the ripple.;<br/>CIAttributeDefault = 100;<br/>CIAttributeDisplayName = Width;<br/>CIAttributeSliderMax = 300;<br/>CIAttributeMin = 1;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 10 |
| CIAttributeFilterName | CIRippleTransition |
| CIAttributeFilterDisplayName | Ripple |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that defines the extent of the effect.;<br/>CIAttributeDefault = [0 0 300 300];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| inputShadingImage | CIAttributeDisplayName = Shading Image;<br/>CIAttributeDescription = An image that looks like a shaded sphere enclosed in a square image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The x and y position to use as the center of the effect;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 9 |
| inputScale | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = A value that determines whether the ripple starts as a bulge (higher value) or a dimple (lower value).;<br/>CIAttributeDefault = 50;<br/>CIAttributeDisplayName = Scale;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeMin = -50;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = -50 |
| CIAttributeReferenceDocumentation | [CIRippleTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRippleTransition) |
| CIAttributeFilterCategories | CICategoryTransition;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |


#### CIAztecCodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Aztec Code Generator |
| inputMessage | CIAttributeDescription = The message to encode in the Aztec Barcode;<br/>CIAttributeDisplayName = Message;<br/>CIAttributeClass = NSData |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAztecCodeGenerator |
| inputCorrectionLevel | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Aztec error correction value between 5 and 95;<br/>CIAttributeDefault = 23;<br/>CIAttributeDisplayName = Correction Level;<br/>CIAttributeSliderMax = 95;<br/>CIAttributeMin = 5;<br/>CIAttributeMax = 95;<br/>CIAttributeSliderMin = 5 |
| CIAttributeReferenceDocumentation | [CIAztecCodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAztecCodeGenerator) |
| inputLayers | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Aztec layers value between 1 and 32. Set to nil for automatic.;<br/>CIAttributeSliderMax = 32;<br/>CIAttributeDisplayName = Layers;<br/>CIAttributeMin = 1;<br/>CIAttributeMax = 32;<br/>CIAttributeSliderMin = 1 |
| inputCompactStyle | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Force a compact style Aztec code to @YES or @NO. Set to nil for automatic.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Compact Style;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMotionBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8.3 |
| CIAttributeFilterDisplayName | Motion Blur |
| inputAngle | CIAttributeDefault = 0;<br/>CIAttributeSliderMax = 3.141592653589793;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle of the motion determines which direction the blur smears.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -3.141592653589793 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMotionBlur |
| CIAttributeReferenceDocumentation | [CIMotionBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMotionBlur) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;<br/>CIAttributeDefault = 20;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMedianFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Median |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryStillImage;<br/>CICategoryVideo;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMedianFilter |
| CIAttributeReferenceDocumentation | [CIMedianFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMedianFilter) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorCubeWithColorSpace:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Cube with ColorSpace |
| inputCubeDimension | CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Cube Dimension;<br/>CIAttributeMin = 2;<br/>CIAttributeMax = 128;<br/>CIAttributeIdentity = 2;<br/>CIAttributeType = CIAttributeTypeCount;<br/>CIAttributeDefault = 2 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCubeWithColorSpace |
| CIAttributeReferenceDocumentation | [CIColorCubeWithColorSpace Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCubeWithColorSpace) |
| inputCubeData | CIAttributeDisplayName = Cube Data;<br/>CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;<br/>CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;<br/>CIAttributeClass = NSData |
| inputColorSpace | CIAttributeDisplayName = Color Space;<br/>CIAttributeClass = NSObject |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIAffineTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Affine Transform |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryGeometryAdjustment;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAffineTransform |
| CIAttributeReferenceDocumentation | [CIAffineTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAffineTransform) |
| inputTransform | CIAttributeDisplayName = Transform;<br/>CIAttributeDescription = A transform to apply to the image.;<br/>CIAttributeIdentity = <NSAffineTransform: 0x600001739640>;<br/>CIAttributeDefault = <NSAffineTransform: 0x600001739640>;<br/>CIAttributeClass = NSAffineTransform;<br/>CIAttributeType = CIAttributeTypeTransform |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPDF417BarcodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| inputDataColumns | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The number of data columns in the generated barcode;<br/>CIAttributeSliderMax = 30;<br/>CIAttributeDisplayName = Data Columns;<br/>CIAttributeMin = 1;<br/>CIAttributeMax = 30;<br/>CIAttributeSliderMin = 1 |
| inputMinHeight | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The minimum height of the generated barcode in pixels.;<br/>CIAttributeSliderMax = 283;<br/>CIAttributeDisplayName = Min Height;<br/>CIAttributeMin = 13;<br/>CIAttributeMax = 283;<br/>CIAttributeSliderMin = 13 |
| inputAlwaysSpecifyCompaction | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Force compaction style to @YES or @NO. Set to nil for automatic.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Always Specify Compaction;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeSliderMin = 0 |
| inputMinWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The minimum width of the generated barcode in pixels.;<br/>CIAttributeSliderMax = 583;<br/>CIAttributeDisplayName = Min Width;<br/>CIAttributeMin = 56;<br/>CIAttributeMax = 583;<br/>CIAttributeSliderMin = 56 |
| inputMaxWidth | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The maximum width of the generated barcode in pixels.;<br/>CIAttributeSliderMax = 583;<br/>CIAttributeDisplayName = Max Width;<br/>CIAttributeMin = 56;<br/>CIAttributeMax = 583;<br/>CIAttributeSliderMin = 56 |
| CIAttributeFilterName | CIPDF417BarcodeGenerator |
| CIAttributeFilterDisplayName | PDF417 Barcode Generator |
| inputMessage | CIAttributeDescription = The message to encode in the PDF417 Barcode;<br/>CIAttributeDisplayName = Message;<br/>CIAttributeClass = NSData |
| inputCorrectionLevel | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The correction level ratio of the generated barcode;<br/>CIAttributeSliderMax = 8;<br/>CIAttributeDisplayName = Correction Level;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 8;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIPDF417BarcodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPDF417BarcodeGenerator) |
| inputRows | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The number of rows in the generated barcode;<br/>CIAttributeSliderMax = 90;<br/>CIAttributeDisplayName = Rows;<br/>CIAttributeMin = 3;<br/>CIAttributeMax = 90;<br/>CIAttributeSliderMin = 3 |
| inputMaxHeight | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The maximum height of the generated barcode in pixels.;<br/>CIAttributeSliderMax = 283;<br/>CIAttributeDisplayName = Max Height;<br/>CIAttributeMin = 13;<br/>CIAttributeMax = 283;<br/>CIAttributeSliderMin = 13 |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| inputPreferredAspectRatio | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The preferred aspect ratio of the generated barcode;<br/>CIAttributeSliderMax = 9223372036854775807;<br/>CIAttributeDisplayName = Preferred Aspect Ratio;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 9223372036854775807;<br/>CIAttributeSliderMin = 0 |
| inputCompactionMode | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The compaction mode of the generated barcode.;<br/>CIAttributeSliderMax = 3;<br/>CIAttributeDisplayName = Compaction Mode;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 3;<br/>CIAttributeSliderMin = 0 |
| inputCompactStyle | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = Force a compact style Aztec code to @YES or @NO. Set to nil for automatic.;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeDisplayName = Compact Style;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.11 |


#### CICode128BarcodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Code 128 Barcode Generator |
| inputMessage | CIAttributeDescription = The message to encode in the Code 128 Barcode;<br/>CIAttributeDisplayName = Message;<br/>CIAttributeClass = NSData |
| CIAttributeFilterCategories | CICategoryGenerator;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CICode128BarcodeGenerator |
| inputQuietSpace | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The number of empty white pixels that should surround the barcode.;<br/>CIAttributeDefault = 7;<br/>CIAttributeDisplayName = Quiet Space;<br/>CIAttributeSliderMax = 20;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 100;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CICode128BarcodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICode128BarcodeGenerator) |
| inputBarcodeHeight | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The height of the generated barcode in pixels.;<br/>CIAttributeDefault = 32;<br/>CIAttributeDisplayName = Barcode Height;<br/>CIAttributeSliderMax = 50;<br/>CIAttributeMin = 1;<br/>CIAttributeMax = 500;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 1 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CISharpenLuminance:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Sharpen Luminance |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategorySharpen;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CISharpenLuminance |
| CIAttributeReferenceDocumentation | [CISharpenLuminance Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISharpenLuminance) |
| inputSharpness | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of sharpening to apply. Larger values are sharper.;<br/>CIAttributeDefault = 0.4;<br/>CIAttributeDisplayName = Sharpness;<br/>CIAttributeSliderMax = 2;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The distance from the center of the effect.;<br/>CIAttributeDefault = 1.69;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 20;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectTransfer:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Transfer |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn;<br/>CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectTransfer |
| CIAttributeReferenceDocumentation | [CIPhotoEffectTransfer Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectTransfer) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIAreaMinMax:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Area Min and Max |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinMax |
| CIAttributeReferenceDocumentation | [CIAreaMinMax Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinMax) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CILabDeltaE:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Lab ∆E |
| inputImage2 | CIAttributeDescription = The second input image for comparison.;<br/>CIAttributeDisplayName = Image2;<br/>CIAttributeClass = Image |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The first input image for comparison.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryColorEffect;<br/>CICategoryVideo;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILabDeltaE |
| CIAttributeReferenceDocumentation | [CILabDeltaE Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILabDeltaE) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILightenBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Lighten Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CILightenBlendMode |
| CIAttributeReferenceDocumentation | [CILightenBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILightenBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMinimumCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Minimum |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryHighDynamicRange;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIMinimumCompositing |
| CIAttributeReferenceDocumentation | [CIMinimumCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMinimumCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVortexDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Vortex Distortion |
| inputAngle | CIAttributeDefault = 56.54866776461628;<br/>CIAttributeSliderMax = 94.24777960769379;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeDisplayName = Angle;<br/>CIAttributeDescription = The angle (in radians) of the vortex.;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeAngle;<br/>CIAttributeSliderMin = -94.24777960769379 |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryDistortionEffect;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIVortexDistortion |
| CIAttributeReferenceDocumentation | [CIVortexDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVortexDistortion) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;<br/>CIAttributeDefault = 300;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 800;<br/>CIAttributeMin = 0;<br/>CIAttributeIdentity = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputCenter | CIAttributeDisplayName = Center;<br/>CIAttributeDescription = The center of the effect as x and y coordinates.;<br/>CIAttributeDefault = [150 150];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAreaAverage:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Average |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to process.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryReduction;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaAverage |
| CIAttributeReferenceDocumentation | [CIAreaAverage Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaAverage) |
| inputExtent | CIAttributeDisplayName = Extent;<br/>CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;<br/>CIAttributeDefault = [0 0 640 80];<br/>CIAttributeClass = Vector;<br/>CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIEdgeWork:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Edge Work |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryStylize;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIEdgeWork |
| CIAttributeReferenceDocumentation | [CIEdgeWork Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEdgeWork) |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The thickness of the edges. The larger the value, the thicker the edges.;<br/>CIAttributeDefault = 3;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 20;<br/>CIAttributeMin = 0;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIColorBlendMode |
| CIAttributeReferenceDocumentation | [CIColorBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBokehBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Bokeh Blur |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryBlur;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIBokehBlur |
| CIAttributeReferenceDocumentation | [CIBokehBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBokehBlur) |
| inputSoftness | CIAttributeDefault = 1;<br/>CIAttributeClass = NSNumber;<br/>CIAttributeSliderMax = 0.4;<br/>CIAttributeDisplayName = Softness;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 10;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0.25 |
| inputRadius | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;<br/>CIAttributeDefault = 20;<br/>CIAttributeDisplayName = Radius;<br/>CIAttributeSliderMax = 100;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 500;<br/>CIAttributeType = CIAttributeTypeDistance;<br/>CIAttributeSliderMin = 0 |
| inputRingSize | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The size of extra emphasis at the ring of the bokeh;<br/>CIAttributeDefault = 0.1;<br/>CIAttributeDisplayName = Ring Size;<br/>CIAttributeSliderMax = 0.2;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 0.2;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| inputRingAmount | CIAttributeClass = NSNumber;<br/>CIAttributeDescription = The amount of extra emphasis at the ring of the bokeh.;<br/>CIAttributeDefault = 0;<br/>CIAttributeDisplayName = Ring Amount;<br/>CIAttributeSliderMax = 1;<br/>CIAttributeMin = 0;<br/>CIAttributeMax = 1;<br/>CIAttributeType = CIAttributeTypeScalar;<br/>CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIDarkenBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Darken Blend Mode |
| inputBackgroundImage | CIAttributeDisplayName = Background Image;<br/>CIAttributeDescription = The image to use as a background image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| inputImage | CIAttributeDisplayName = Image;<br/>CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;<br/>CIAttributeClass = Image;<br/>CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories | CICategoryCompositeOperation;<br/>CICategoryVideo;<br/>CICategoryStillImage;<br/>CICategoryInterlaced;<br/>CICategoryNonSquarePixels;<br/>CICategoryBuiltIn |
| CIAttributeFilterName | CIDarkenBlendMode |
| CIAttributeReferenceDocumentation | [CIDarkenBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDarkenBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |
