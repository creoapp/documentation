For more information: [Core Image Filter Reference](https://developer.apple.com/library/archive/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html)

#### CIEdges:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Edges |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIEdges |
| CIAttributeReferenceDocumentation | [CIEdges Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEdges) |
| inputIntensity |
	* CIAttributeDefault = 1;
	* CIAttributeSliderMax = 10;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the edges. The larger the value, the higher the intensity.;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIOpTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Op Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of a tile.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIOpTile |
| CIAttributeReferenceDocumentation | [CIOpTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIOpTile) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scale determines the number of tiles in the effect.;
	* CIAttributeDefault = 2.8;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.1 |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 65;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 1000;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 65;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAffineTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Affine Tile |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAffineTile |
| CIAttributeReferenceDocumentation | [CIAffineTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAffineTile) |
| inputTransform |
	* CIAttributeDisplayName = Transform;
	* CIAttributeDescription = The transform to apply to the image.;
	* CIAttributeIdentity = <NSAffineTransform: 0x60000177dac0>;
	* CIAttributeDefault = <NSAffineTransform: 0x60000177da80>;
	* CIAttributeClass = NSAffineTransform |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Perspective Transform |
| inputTopRight |
	* CIAttributeDisplayName = Top Right;
	* CIAttributeDescription = The top right coordinate to map the image to.;
	* CIAttributeDefault = [646 507];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIPerspectiveTransform |
| CIAttributeReferenceDocumentation | [CIPerspectiveTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveTransform) |
| inputBottomLeft |
	* CIAttributeDisplayName = Bottom Left;
	* CIAttributeDescription = The bottom left coordinate to map the image to.;
	* CIAttributeDefault = [155 153];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputTopLeft |
	* CIAttributeDisplayName = Top Left;
	* CIAttributeDescription = The top left coordinate to map the image to.;
	* CIAttributeDefault = [118 484];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputBottomRight |
	* CIAttributeDisplayName = Bottom Right;
	* CIAttributeDescription = The bottom right coordinate to map the image to.;
	* CIAttributeDefault = [548 140];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAffineClamp:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Affine Clamp |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAffineClamp |
| CIAttributeReferenceDocumentation | [CIAffineClamp Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAffineClamp) |
| inputTransform |
	* CIAttributeDisplayName = Transform;
	* CIAttributeDescription = The transform to apply to the image.;
	* CIAttributeIdentity = <NSAffineTransform: 0x60000177d840>;
	* CIAttributeDefault = <NSAffineTransform: 0x60000177d800>;
	* CIAttributeClass = NSAffineTransform |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CINoiseReduction:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Noise Reduction |
| inputNoiseLevel |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of noise reduction. The larger the value, the more noise reduction.;
	* CIAttributeSliderMax = 0.1;
	* CIAttributeDisplayName = Noise Level;
	* CIAttributeDefault = 0.02;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CINoiseReduction |
| CIAttributeReferenceDocumentation | [CINoiseReduction Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CINoiseReduction) |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The sharpness of the final image. The larger the value, the sharper the result.;
	* CIAttributeSliderMax = 2;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeDefault = 0.4;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHueBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Hue Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHueBlendMode |
| CIAttributeReferenceDocumentation | [CIHueBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHueBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorPosterize:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Color Posterize |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorPosterize |
| CIAttributeReferenceDocumentation | [CIColorPosterize Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorPosterize) |
| inputLevels |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The number of brightness levels to use for each color component. Lower values result in a more extreme poster effect.;
	* CIAttributeDefault = 6;
	* CIAttributeDisplayName = Levels;
	* CIAttributeSliderMax = 30;
	* CIAttributeMin = 1;
	* CIAttributeIdentity = 300;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 2 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorMonochrome:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Monochrome |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorMonochrome |
| CIAttributeReferenceDocumentation | [CIColorMonochrome Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorMonochrome) |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The monochrome color to apply to the image.;
	* CIAttributeDefault = (0.6 0.45 0.3 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeOpaqueColor |
| inputIntensity |
	* CIAttributeDefault = 1;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the monochrome effect. A value of 1.0 creates a monochrome image using the supplied color. A value of 0.0 has no effect on the image.;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMaximumComponent:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Maximum Component |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMaximumComponent |
| CIAttributeReferenceDocumentation | [CIMaximumComponent Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaximumComponent) |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIPhotoEffectMono:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Mono |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectMono |
| CIAttributeReferenceDocumentation | [CIPhotoEffectMono Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectMono) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CITriangleKaleidoscope:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Triangle Kaleidoscope |
| inputPoint |
	* CIAttributeDisplayName = Point;
	* CIAttributeDescription = The x and y position to use as the center of the triangular area in the input image.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = Input image to generate kaleidoscope effect from.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CITriangleKaleidoscope |
| CIAttributeReferenceDocumentation | [CITriangleKaleidoscope Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITriangleKaleidoscope) |
| inputSize |
	* CIAttributeDefault = 700;
	* CIAttributeDescription = The size in pixels of the triangle.;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Size;
	* CIAttributeSliderMax = 1000;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputRotation |
	* CIAttributeDefault = 5.924285296593801;
	* CIAttributeDescription = Rotation angle of the triangle.;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Rotation;
	* CIAttributeSliderMax = 6.283185307179586;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = 0 |
| inputDecay |
	* CIAttributeDefault = 0.85;
	* CIAttributeDescription = The decay determines how fast the color fades from the center triangle.;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Decay;
	* CIAttributeSliderMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIConvolution9Horizontal:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Horizontal 9 Convolution |
| inputWeights |
	* CIAttributeDisplayName = Weights;
	* CIAttributeIdentity = [0 0 0 0 1 0 0 0 0];
	* CIAttributeDefault = [0 0 0 0 1 0 0 0 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution9Horizontal |
| CIAttributeReferenceDocumentation | [CIConvolution9Horizontal Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution9Horizontal) |
| inputBias |
	* CIAttributeDisplayName = Bias;
	* CIAttributeIdentity = 0;
	* CIAttributeDefault = 0;
	* CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIPointillize:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Pointillize |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIPointillize |
| CIAttributeReferenceDocumentation | [CIPointillize Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPointillize) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the circles in the resulting pattern.;
	* CIAttributeDefault = 20;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 1;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorCurves:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Color Curves |
| inputColorSpace |
	* CIAttributeDisplayName = Color Space;
	* CIAttributeClass = NSObject |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCurves |
| CIAttributeReferenceDocumentation | [CIColorCurves Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCurves) |
| inputCurvesDomain |
	* CIAttributeDefault = [0 1];
	* CIAttributeDisplayName = Curves Domain;
	* CIAttributeClass = Vector |
| inputCurvesData |
	* CIAttributeDefault = <00000000 00000000 00000000 0000003f 0000003f 0000003f 0000803f 0000803f 0000803f>;
	* CIAttributeDisplayName = Curves Data;
	* CIAttributeClass = NSData |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIParallelogramTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Parallelogram Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIParallelogramTile |
| CIAttributeReferenceDocumentation | [CIParallelogramTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIParallelogramTile) |
| inputAcuteAngle |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The primary angle for the repeating parallelogram tile. Small values create thin diamond tiles, and higher values create fatter parallelogram tiles.;
	* CIAttributeDefault = 1.570796326794897;
	* CIAttributeDisplayName = Acute Angle;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeIdentity = 1.570796326794897;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBloom:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Bloom |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBloom |
| CIAttributeReferenceDocumentation | [CIBloom Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBloom) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the effect. The larger the radius, the greater the effect.;
	* CIAttributeDefault = 10;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputIntensity |
	* CIAttributeDefault = 0.5;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the effect. A value of 0.0 is no effect. A value of 1.0 is the maximum effect.;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIQRCodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | QR Code Generator |
| inputMessage |
	* CIAttributeDescription = The message to encode in the QR Code;
	* CIAttributeDisplayName = Message;
	* CIAttributeClass = NSData |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIQRCodeGenerator |
| inputCorrectionLevel |
	* CIAttributeDisplayName = Correction Level;
	* CIAttributeDescription = QR Code correction level L, M, Q, or H.;
	* CIAttributeDefault = M;
	* CIAttributeClass = NSString |
| CIAttributeReferenceDocumentation | [CIQRCodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIQRCodeGenerator) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIFalseColor:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | False Color |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIFalseColor |
| CIAttributeReferenceDocumentation | [CIFalseColor Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFalseColor) |
| inputColor0 |
	* CIAttributeDisplayName = Color 1;
	* CIAttributeDescription = The first color to use for the color ramp.;
	* CIAttributeDefault = (0.3 0 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| inputColor1 |
	* CIAttributeDisplayName = Color 2;
	* CIAttributeDescription = The second color to use for the color ramp.;
	* CIAttributeDefault = (1 0.9 0.8 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAreaMaximumAlpha:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Maximum Alpha |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMaximumAlpha |
| CIAttributeReferenceDocumentation | [CIAreaMaximumAlpha Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMaximumAlpha) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIMeshGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Mesh Generator |
| inputMesh |
	* CIAttributeDescription = An array of line segments stored as an array of CIVectors each containing a start point and end point.;
	* CIAttributeDisplayName = Mesh;
	* CIAttributeClass = NSArray |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMeshGenerator |
| CIAttributeReferenceDocumentation | [CIMeshGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMeshGenerator) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of the effect.;
	* CIAttributeDefault = 1.5;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = A color.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIAttributedTextImageGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Attributed Text Image Generator |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputText |
	* CIAttributeDisplayName = Text;
	* CIAttributeClass = NSAttributedString |
| CIAttributeFilterName | CIAttributedTextImageGenerator |
| CIAttributeReferenceDocumentation | [CIAttributedTextImageGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAttributedTextImageGenerator) |
| inputScaleFactor |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 4;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Scale Factor;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIDotScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Dot Screen |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryHalftoneEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDotScreen |
| CIAttributeReferenceDocumentation | [CIDotScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDotScreen) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance between dots in the pattern.;
	* CIAttributeDefault = 6;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 50;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 2 |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The sharpness of the pattern. The larger the value, the sharper the pattern.;
	* CIAttributeDefault = 0.7;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the dot screen pattern;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIOverlayBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Overlay Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIOverlayBlendMode |
| CIAttributeReferenceDocumentation | [CIOverlayBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIOverlayBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIRadialGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Radial Gradient |
| inputRadius0 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the starting circle to use in the gradient.;
	* CIAttributeDefault = 5;
	* CIAttributeDisplayName = Radius 1;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterCategories |
	* CICategoryGradient;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIRadialGradient |
| inputRadius1 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the ending circle to use in the gradient.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Radius 2;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CIRadialGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRadialGradient) |
| inputColor0 |
	* CIAttributeDisplayName = Color 1;
	* CIAttributeDescription = The first color to use in the gradient.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| inputColor1 |
	* CIAttributeDisplayName = Color 2;
	* CIAttributeDescription = The second color to use in the gradient.;
	* CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPinchDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Pinch Distortion |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIPinchDistortion |
| CIAttributeReferenceDocumentation | [CIPinchDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPinchDistortion) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of pinching. A value of 0.0 has no effect. A value of 1.0 is the maximum pinch.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 2;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 1000;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIComicEffect:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Comic Effect |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIComicEffect |
| CIAttributeReferenceDocumentation | [CIComicEffect Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIComicEffect) |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CISubtractBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Subtract Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISubtractBlendMode |
| CIAttributeReferenceDocumentation | [CISubtractBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISubtractBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMix:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Mix |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as a foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMix |
| CIAttributeReferenceDocumentation | [CIMix Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMix) |
| inputAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of the effect.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Amount;
	* CIAttributeSliderMax = 1;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIBumpDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Bump Distortion |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBumpDistortion |
| CIAttributeReferenceDocumentation | [CIBumpDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBumpDistortion) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scale of the effect determines the curvature of the bump. A value of 0.0 has no effect. Positive values create an outward bump; negative values create an inward bump.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -1 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 600;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDisparityToDepth:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Disparity To Depth |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The input disparity data image to convert to depth data.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDisparityToDepth |
| CIAttributeReferenceDocumentation | [CIDisparityToDepth Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDisparityToDepth) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIHatchedScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Hatched Screen |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryHalftoneEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHatchedScreen |
| CIAttributeReferenceDocumentation | [CIHatchedScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHatchedScreen) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance between lines in the pattern.;
	* CIAttributeDefault = 6;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 50;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 2 |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of sharpening to apply.;
	* CIAttributeDefault = 0.7;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the hatched screen pattern;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIRowAverage:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Row Average |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIRowAverage |
| CIAttributeReferenceDocumentation | [CIRowAverage Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRowAverage) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIBlendWithRedMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Blend With Red Mask |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithRedMask |
| CIAttributeReferenceDocumentation | [CIBlendWithRedMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithRedMask) |
| inputMaskImage |
	* CIAttributeDisplayName = Mask Image;
	* CIAttributeDescription = A masking image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILenticularHaloGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = A color.;
	* CIAttributeDefault = (1 0.9 0.8 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The duration of the effect.;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0 |
| inputStriationStrength |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The intensity of the halo colors. Larger values are more intense.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Striation Strength;
	* CIAttributeSliderMax = 3;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CILenticularHaloGenerator |
| CIAttributeFilterDisplayName | Lenticular Halo |
| inputHaloOverlap |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 1;
	* CIAttributeDefault = 0.77;
	* CIAttributeDisplayName = Halo Overlap;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the halo.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeReferenceDocumentation | [CILenticularHaloGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILenticularHaloGenerator) |
| inputStriationContrast |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The contrast of the halo colors. Larger values are higher contrast.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Striation Contrast;
	* CIAttributeSliderMax = 5;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputHaloRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the halo.;
	* CIAttributeDefault = 70;
	* CIAttributeDisplayName = Halo Radius;
	* CIAttributeSliderMax = 1000;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputHaloWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of the halo, from its inner radius to its outer radius.;
	* CIAttributeDefault = 87;
	* CIAttributeDisplayName = Halo Width;
	* CIAttributeSliderMax = 300;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |


#### CICircleSplashDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Circle Splash Distortion |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICircleSplashDistortion |
| CIAttributeReferenceDocumentation | [CICircleSplashDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICircleSplashDistortion) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 150;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 1000;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CICircularWrap:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Circular Wrap Distortion |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the effect.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICircularWrap |
| CIAttributeReferenceDocumentation | [CICircularWrap Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICircularWrap) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 150;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 600;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIStraightenFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Straighten |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = An angle in radians.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIStraightenFilter |
| CIAttributeReferenceDocumentation | [CIStraightenFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStraightenFilter) |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIHighlightShadowAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Highlight and Shadow Adjust |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHighlightShadowAdjust |
| CIAttributeReferenceDocumentation | [CIHighlightShadowAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHighlightShadowAdjust) |
| inputHighlightAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of adjustment to the highlights of the image.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Highlight Amount;
	* CIAttributeSliderMin = 0.3;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 1 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Shadow Highlight Radius;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputShadowAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of adjustment to the shadows of the image.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Shadow Amount;
	* CIAttributeSliderMin = -1;
	* CIAttributeMin = -1;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIColorCrossPolynomial:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Cross Polynomial |
| inputRedCoefficients |
	* CIAttributeDisplayName = Red Coefficients;
	* CIAttributeDescription = Polynomial coefficients for red channel;
	* CIAttributeIdentity = [1 0 0 0 0 0 0 0 0 0];
	* CIAttributeDefault = [1 0 0 0 0 0 0 0 0 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCrossPolynomial |
| CIAttributeReferenceDocumentation | [CIColorCrossPolynomial Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCrossPolynomial) |
| inputGreenCoefficients |
	* CIAttributeDisplayName = Green Coefficients;
	* CIAttributeDescription = Polynomial coefficients for green channel;
	* CIAttributeIdentity = [0 1 0 0 0 0 0 0 0 0];
	* CIAttributeDefault = [0 1 0 0 0 0 0 0 0 0];
	* CIAttributeClass = Vector |
| inputBlueCoefficients |
	* CIAttributeDisplayName = Blue Coefficients;
	* CIAttributeDescription = Polynomial coefficients for blue channel;
	* CIAttributeIdentity = [0 0 1 0 0 0 0 0 0 0];
	* CIAttributeDefault = [0 0 1 0 0 0 0 0 0 0];
	* CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIUnsharpMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Unsharp Mask |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategorySharpen;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIUnsharpMask |
| CIAttributeReferenceDocumentation | [CIUnsharpMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIUnsharpMask) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius around a given pixel to apply the unsharp mask. The larger the radius, the more of the image is affected.;
	* CIAttributeDefault = 2.5;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputIntensity |
	* CIAttributeDefault = 0.5;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the effect. The larger the value, the more contrast in the affected area.;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISourceOutCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source Out |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISourceOutCompositing |
| CIAttributeReferenceDocumentation | [CISourceOutCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceOutCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAdditionCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Addition |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAdditionCompositing |
| CIAttributeReferenceDocumentation | [CIAdditionCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAdditionCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHistogramDisplayFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Histogram Display |
| inputHeight |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The height of the displayable histogram image.;
	* CIAttributeSliderMax = 100;
	* CIAttributeDisplayName = Height;
	* CIAttributeSliderMin = 1;
	* CIAttributeMin = 1;
	* CIAttributeMax = 200;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 100 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHistogramDisplayFilter |
| CIAttributeReferenceDocumentation | [CIHistogramDisplayFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHistogramDisplayFilter) |
| inputLowLimit |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The fraction of the left portion of the histogram image to make darker;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Low Limit;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0 |
| inputHighLimit |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The fraction of the right portion of the histogram image to make lighter.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = High Limit;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 1 |
| CIAttributeFilterAvailable_Mac | 10.? |


#### CILineScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Line Screen |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryHalftoneEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILineScreen |
| CIAttributeReferenceDocumentation | [CILineScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILineScreen) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance between lines in the pattern.;
	* CIAttributeDefault = 6;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 50;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 2 |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The sharpness of the pattern. The larger the value, the sharper the pattern.;
	* CIAttributeDefault = 0.7;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the line screen pattern;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveCorrection:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.10 |
| CIAttributeFilterName | CIPerspectiveCorrection |
| CIAttributeFilterDisplayName | Perspective Correction |
| inputTopRight |
	* CIAttributeDisplayName = Top Right;
	* CIAttributeDescription = The top right coordinate to be perspective corrected.;
	* CIAttributeDefault = [646 507];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputCrop |
	* CIAttributeDisplayName = Crop;
	* CIAttributeDefault = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeType = CIAttributeTypeBoolean |
| inputBottomRight |
	* CIAttributeDisplayName = Bottom Right;
	* CIAttributeDescription = The bottom right coordinate to be perspective corrected.;
	* CIAttributeDefault = [548 140];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeReferenceDocumentation | [CIPerspectiveCorrection Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveCorrection) |
| inputTopLeft |
	* CIAttributeDisplayName = Top Left;
	* CIAttributeDescription = The top left coordinate to be perspective corrected.;
	* CIAttributeDefault = [118 484];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryBuiltIn |
| inputBottomLeft |
	* CIAttributeDisplayName = Bottom Left;
	* CIAttributeDescription = The bottom left coordinate to be perspective corrected.;
	* CIAttributeDefault = [155 153];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIAreaMaximum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Maximum |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMaximum |
| CIAttributeReferenceDocumentation | [CIAreaMaximum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMaximum) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CISmoothLinearGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Smooth Linear Gradient |
| inputColor1 |
	* CIAttributeDisplayName = Color 2;
	* CIAttributeDescription = The second color to use in the gradient.;
	* CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterCategories |
	* CICategoryGradient;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISmoothLinearGradient |
| inputColor0 |
	* CIAttributeDisplayName = Color 1;
	* CIAttributeDescription = The first color to use in the gradient.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeReferenceDocumentation | [CISmoothLinearGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISmoothLinearGradient) |
| inputPoint1 |
	* CIAttributeDisplayName = Point 1;
	* CIAttributeDescription = The ending position of the gradient -- where the second color begins.;
	* CIAttributeDefault = [200 200];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputPoint0 |
	* CIAttributeDisplayName = Point 0;
	* CIAttributeDescription = The starting position of the gradient -- where the first color begins.;
	* CIAttributeDefault = [0 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CISixfoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Sixfold Reflected Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISixfoldReflectedTile |
| CIAttributeReferenceDocumentation | [CISixfoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISixfoldReflectedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CISpotLight:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputLightPointsAt |
	* CIAttributeDisplayName = Light Points At;
	* CIAttributeDescription = The x and y position that the spotlight points at.;
	* CIAttributeDefault = [200 200 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition3 |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The color of the spotlight.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeOpaqueColor |
| inputConcentration |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The spotlight size. The smaller the value, the more tightly focused the light beam.;
	* CIAttributeDefault = 0.1;
	* CIAttributeDisplayName = Concentration;
	* CIAttributeSliderMax = 1.5;
	* CIAttributeMin = 0.001;
	* CIAttributeIdentity = 20;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.001 |
| CIAttributeFilterName | CISpotLight |
| CIAttributeFilterDisplayName | Spot Light |
| CIAttributeFilterAvailable_iOS | 9 |
| inputBrightness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The brightness of the spotlight.;
	* CIAttributeDefault = 3;
	* CIAttributeDisplayName = Brightness;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CISpotLight Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISpotLight) |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputLightPosition |
	* CIAttributeDisplayName = Light Position;
	* CIAttributeDescription = The x and y position of the spotlight.;
	* CIAttributeDefault = [400 600 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition3 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIThermal:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Thermal |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIThermal |
| CIAttributeReferenceDocumentation | [CIThermal Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIThermal) |
| CIAttributeFilterAvailable_Mac | 10.11 |


#### CICheckerboardGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Checkerboard |
| inputColor1 |
	* CIAttributeDisplayName = Color 2;
	* CIAttributeDescription = A color to use for the second set of squares.;
	* CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICheckerboardGenerator |
| inputColor0 |
	* CIAttributeDisplayName = Color 1;
	* CIAttributeDescription = A color to use for the first set of squares.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| CIAttributeReferenceDocumentation | [CICheckerboardGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICheckerboardGenerator) |
| inputWidth |
	* CIAttributeDefault = 80;
	* CIAttributeDescription = The width of the squares in the pattern.;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 800;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The sharpness of the edges in pattern. The smaller the value, the more blurry the pattern. Values range from 0.0 to 1.0.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISRGBToneCurveToLinear:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | sRGB Tone Curve to Linear |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISRGBToneCurveToLinear |
| CIAttributeReferenceDocumentation | [CISRGBToneCurveToLinear Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISRGBToneCurveToLinear) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIBlendWithMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Blend With Mask |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as a foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithMask |
| CIAttributeReferenceDocumentation | [CIBlendWithMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithMask) |
| inputMaskImage |
	* CIAttributeDisplayName = Mask Image;
	* CIAttributeDescription = A grayscale mask. When a mask value is 0.0, the result is the background. When the mask value is 1.0, the result is the image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectChrome:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Chrome |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectChrome |
| CIAttributeReferenceDocumentation | [CIPhotoEffectChrome Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectChrome) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CINinePartTiled:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Nine Part Tiled |
| inputGrowAmount |
	* CIAttributeDisplayName = Grow Amount;
	* CIAttributeDefault = [100 100];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CINinePartTiled |
| CIAttributeReferenceDocumentation | [CINinePartTiled Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CINinePartTiled) |
| inputBreakpoint0 |
	* CIAttributeDisplayName = Breakpoint0;
	* CIAttributeDescription = Lower left corner of image to retain before tiling begins.;
	* CIAttributeDefault = [50 50];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputFlipYTiles |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Indicates that Y-Axis flip should occur.;
	* CIAttributeDisplayName = Flip Y Tiles;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeBoolean;
	* CIAttributeDefault = 1 |
| inputBreakpoint1 |
	* CIAttributeDisplayName = Breakpoint1;
	* CIAttributeDescription = Upper right corner of image to retain after tiling ends.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIHexagonalPixellate:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Hexagonal Pixelate |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHexagonalPixellate |
| CIAttributeReferenceDocumentation | [CIHexagonalPixellate Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHexagonalPixellate) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scale determines the size of the hexagons. Larger values result in larger hexagons.;
	* CIAttributeDefault = 8;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 1;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIBicubicScaleTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Bicubic Scale Transform |
| inputB |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Specifies the value of B to use for the cubic resampling function.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = B;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBicubicScaleTransform |
| CIAttributeReferenceDocumentation | [CIBicubicScaleTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBicubicScaleTransform) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scaling factor to use on the image. Values less than 1.0 scale down the images. Values greater than 1.0 scale up the image.;
	* CIAttributeSliderMax = 100;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMin = 0.05;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 1 |
| inputC |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Specifies the value of C to use for the cubic resampling function.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = C;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0.75 |
| inputAspectRatio |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The additional horizontal scaling factor to use on the image.;
	* CIAttributeSliderMax = 2;
	* CIAttributeDisplayName = Aspect Ratio;
	* CIAttributeSliderMin = 0.5;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 1 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIColorClamp:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Clamp |
| inputMaxComponents |
	* CIAttributeDisplayName = Max Components;
	* CIAttributeDescription = Higher clamping values;
	* CIAttributeDefault = [1 1 1 1];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorClamp |
| CIAttributeReferenceDocumentation | [CIColorClamp Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorClamp) |
| inputMinComponents |
	* CIAttributeDisplayName = Min Components;
	* CIAttributeDescription = Lower clamping values;
	* CIAttributeDefault = [0 0 0 0];
	* CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIPhotoEffectProcess:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Process |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectProcess |
| CIAttributeReferenceDocumentation | [CIPhotoEffectProcess Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectProcess) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CISourceInCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source In |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISourceInCompositing |
| CIAttributeReferenceDocumentation | [CISourceInCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceInCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectNoir:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Noir |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectNoir |
| CIAttributeReferenceDocumentation | [CIPhotoEffectNoir Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectNoir) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CICameraCalibrationLensCorrection:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Lens Correction for AVC |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICameraCalibrationLensCorrection |
| CIAttributeReferenceDocumentation | [CICameraCalibrationLensCorrection Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICameraCalibrationLensCorrection) |
| inputAVCameraCalibrationData |
	* CIAttributeDescription = AVCameraCalibrationData for the correction.  Will be set from the inputImage if available and can be overridden here.;
	* CIAttributeDisplayName = Calibration Data object of type AVCameraCalibrationData;
	* CIAttributeClass = AVCameraCalibrationData |
| inputUseInverseLookUpTable |
	* CIAttributeDisplayName = Use Inverse Look Up Table;
	* CIAttributeDescription = Boolean value used to select the Look Up Table from the AVCameraCalibrationData;
	* CIAttributeDefault = 0;
	* CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIXRay:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | X-Ray |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIXRay |
| CIAttributeReferenceDocumentation | [CIXRay Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIXRay) |
| CIAttributeFilterAvailable_Mac | 10.11 |


#### CIConvolution7X7:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | 7 by 7 convolution |
| inputWeights |
	* CIAttributeDisplayName = Weights;
	* CIAttributeIdentity = [0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0];
	* CIAttributeDefault = [0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution7X7 |
| CIAttributeReferenceDocumentation | [CIConvolution7X7 Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution7X7) |
| inputBias |
	* CIAttributeDisplayName = Bias;
	* CIAttributeIdentity = 0;
	* CIAttributeDefault = 0;
	* CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIToneCurve:
| Attribute | Value |
| ---------- | --------- |
| inputPoint0 |
	* CIAttributeIdentity = [0 0];
	* CIAttributeDisplayName = Point 0;
	* CIAttributeDefault = [0 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterAvailable_Mac | 10.7 |
| inputPoint1 |
	* CIAttributeIdentity = [0.25 0.25];
	* CIAttributeDisplayName = Point 1;
	* CIAttributeDefault = [0.25 0.25];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| inputPoint2 |
	* CIAttributeIdentity = [0.5 0.5];
	* CIAttributeDisplayName = Point 2;
	* CIAttributeDefault = [0.5 0.5];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| inputPoint3 |
	* CIAttributeIdentity = [0.75 0.75];
	* CIAttributeDisplayName = Point 3;
	* CIAttributeDefault = [0.75 0.75];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterName | CIToneCurve |
| CIAttributeFilterDisplayName | Tone Curve |
| inputPoint4 |
	* CIAttributeIdentity = [1 1];
	* CIAttributeDisplayName = Point 4;
	* CIAttributeDefault = [1 1];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeReferenceDocumentation | [CIToneCurve Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIToneCurve) |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIColorBurnBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Burn Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorBurnBlendMode |
| CIAttributeReferenceDocumentation | [CIColorBurnBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorBurnBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectFade:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Fade |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectFade |
| CIAttributeReferenceDocumentation | [CIPhotoEffectFade Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectFade) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CICrop:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Crop |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICrop |
| CIAttributeReferenceDocumentation | [CICrop Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICrop) |
| inputRectangle |
	* CIAttributeDisplayName = Rectangle;
	* CIAttributeDescription = The rectangle that specifies the crop to apply to the image.;
	* CIAttributeIdentity = [-8.98847e+307 -8.98847e+307 1.79769e+308 1.79769e+308];
	* CIAttributeDefault = [-8.98847e+307 -8.98847e+307 1.79769e+308 1.79769e+308];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveTransformWithExtent:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| CIAttributeFilterName | CIPerspectiveTransformWithExtent |
| CIAttributeFilterDisplayName | Perspective Transform with Extent |
| inputTopRight |
	* CIAttributeDisplayName = Top Right;
	* CIAttributeDefault = [646 507];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that defines the extent of the effect.;
	* CIAttributeDefault = [0 0 300 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| inputBottomRight |
	* CIAttributeDisplayName = Bottom Right;
	* CIAttributeDefault = [548 140];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIPerspectiveTransformWithExtent Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveTransformWithExtent) |
| inputTopLeft |
	* CIAttributeDisplayName = Top Left;
	* CIAttributeDefault = [118 484];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputBottomLeft |
	* CIAttributeDisplayName = Bottom Left;
	* CIAttributeDefault = [155 153];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIConvolution5X5:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | 5 by 5 convolution |
| inputWeights |
	* CIAttributeDisplayName = Weights;
	* CIAttributeIdentity = [0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0];
	* CIAttributeDefault = [0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution5X5 |
| CIAttributeReferenceDocumentation | [CIConvolution5X5 Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution5X5) |
| inputBias |
	* CIAttributeDisplayName = Bias;
	* CIAttributeIdentity = 0;
	* CIAttributeDefault = 0;
	* CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CITwirlDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Twirl Distortion |
| inputAngle |
	* CIAttributeDefault = 3.141592653589793;
	* CIAttributeSliderMax = 12.56637061435917;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the twirl. Values can be positive or negative.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -12.56637061435917 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CITwirlDistortion |
| CIAttributeReferenceDocumentation | [CITwirlDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITwirlDistortion) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 500;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 300;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDisplacementDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Displacement Distortion |
| inputDisplacementImage |
	* CIAttributeDescription = An image whose grayscale values will be applied to the source image.;
	* CIAttributeDisplayName = Displacement Image;
	* CIAttributeClass = Image |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDisplacementDistortion |
| CIAttributeReferenceDocumentation | [CIDisplacementDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDisplacementDistortion) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of texturing of the resulting image. The larger the value, the greater the texturing.;
	* CIAttributeSliderMax = 200;
	* CIAttributeDisplayName = Scale;
	* CIAttributeDefault = 50;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISepiaTone:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Sepia Tone |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CISepiaTone |
| CIAttributeReferenceDocumentation | [CISepiaTone Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISepiaTone) |
| inputIntensity |
	* CIAttributeDefault = 1;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the sepia effect. A value of 1.0 creates a monochrome sepia image. A value of 0.0 has no effect on the image.;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISourceOverCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source Over |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISourceOverCompositing |
| CIAttributeReferenceDocumentation | [CISourceOverCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceOverCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIGlideReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Glide Reflected Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIGlideReflectedTile |
| CIAttributeReferenceDocumentation | [CIGlideReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGlideReflectedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIModTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputAngle |
	* CIAttributeDefault = 2;
	* CIAttributeSliderMax = 6.283185307179586;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the mod hole pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -6.283185307179586 |
| inputCompression |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of stretching applied to the mod hole pattern. Holes in the center are not distorted as much as those at the edge of the image.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Compression;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 100 |
| CIAttributeFilterName | CIModTransition |
| CIAttributeFilterDisplayName | Mod |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIModTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIModTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the undistorted holes in the pattern.;
	* CIAttributeDefault = 150;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIConvolution3X3:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | 3 by 3 convolution |
| inputWeights |
	* CIAttributeDisplayName = Weights;
	* CIAttributeIdentity = [0 0 0 0 1 0 0 0 0];
	* CIAttributeDefault = [0 0 0 0 1 0 0 0 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution3X3 |
| CIAttributeReferenceDocumentation | [CIConvolution3X3 Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution3X3) |
| inputBias |
	* CIAttributeDisplayName = Bias;
	* CIAttributeIdentity = 0;
	* CIAttributeDefault = 0;
	* CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIDepthToDisparity:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Depth To Disparity |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The input depth data image to convert to disparity data.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDepthToDisparity |
| CIAttributeReferenceDocumentation | [CIDepthToDisparity Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDepthToDisparity) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILanczosScaleTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Lanczos Scale Transform |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILanczosScaleTransform |
| CIAttributeReferenceDocumentation | [CILanczosScaleTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILanczosScaleTransform) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scaling factor to use on the image. Values less than 1.0 scale down the images. Values greater than 1.0 scale up the image.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 1.5;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.05 |
| inputAspectRatio |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The additional horizontal scaling factor to use on the image.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Aspect Ratio;
	* CIAttributeSliderMax = 2;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.5 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHeightFieldFromMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Height Field From Mask |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The white values of the mask define those pixels that are inside the height field while the black values define those pixels that are outside. The field varies smoothly and continuously inside the mask, reaching the value 0 at the edge of the mask.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHeightFieldFromMask |
| CIAttributeReferenceDocumentation | [CIHeightFieldFromMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHeightFieldFromMask) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance from the edge of the mask for the smooth transition is proportional to the input radius. Larger values make the transition smoother and more pronounced. Smaller values make the transition approximate a fillet radius.;
	* CIAttributeDefault = 10;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 300;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 10;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDivideBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Divide Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDivideBlendMode |
| CIAttributeReferenceDocumentation | [CIDivideBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDivideBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIDifferenceBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Difference Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDifferenceBlendMode |
| CIAttributeReferenceDocumentation | [CIDifferenceBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDifferenceBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMorphologyGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Morphology Gradient |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMorphologyGradient |
| CIAttributeReferenceDocumentation | [CIMorphologyGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMorphologyGradient) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The desired radius of the circular morphological operation to the image.;
	* CIAttributeSliderMax = 50;
	* CIAttributeDisplayName = Radius;
	* CIAttributeDefault = 5;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIMinimumComponent:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Minimum Component |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMinimumComponent |
| CIAttributeReferenceDocumentation | [CIMinimumComponent Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMinimumComponent) |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIDiscBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Disc Blur |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDiscBlur |
| CIAttributeReferenceDocumentation | [CIDiscBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDiscBlur) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;
	* CIAttributeDefault = 8;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CITorusLensDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Torus Lens Distortion |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CITorusLensDistortion |
| CIAttributeReferenceDocumentation | [CITorusLensDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITorusLensDistortion) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of the ring.;
	* CIAttributeDefault = 80;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The outer radius of the torus.;
	* CIAttributeDefault = 160;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 500;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputRefraction |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The refraction of the glass.;
	* CIAttributeSliderMax = 5;
	* CIAttributeDisplayName = Refraction;
	* CIAttributeDefault = 1.7;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the torus.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIFlashTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The color of the light rays emanating from the flash.;
	* CIAttributeDefault = (1 0.8 0.6 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputStriationStrength |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The strength of the light rays emanating from the flash.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Striation Strength;
	* CIAttributeSliderMax = 3;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CIFlashTransition |
| CIAttributeFilterDisplayName | Flash |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = The extent of the flash.;
	* CIAttributeDefault = [0 0 300 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| inputFadeThreshold |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of fade between the flash and the target image. The higher the value, the more flash time and the less fade time.;
	* CIAttributeDefault = 0.85;
	* CIAttributeDisplayName = Fade Threshold;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| inputStriationContrast |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The contrast of the light rays emanating from the flash.;
	* CIAttributeDefault = 1.375;
	* CIAttributeDisplayName = Striation Contrast;
	* CIAttributeSliderMax = 5;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CIFlashTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFlashTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputMaxStriationRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the light rays emanating from the flash.;
	* CIAttributeDefault = 2.58;
	* CIAttributeDisplayName = Maximum Striation Radius;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIFourfoldRotatedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Fourfold Rotated Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIFourfoldRotatedTile |
| CIAttributeReferenceDocumentation | [CIFourfoldRotatedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFourfoldRotatedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIColorCubesMixedWithMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.13 |
| inputCubeDimension |
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Cube Dimension;
	* CIAttributeMin = 2;
	* CIAttributeMax = 128;
	* CIAttributeIdentity = 2;
	* CIAttributeType = CIAttributeTypeCount;
	* CIAttributeDefault = 2 |
| inputMaskImage |
	* CIAttributeDisplayName = Mask Image;
	* CIAttributeDescription = A masking image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputCube0Data |
	* CIAttributeDisplayName = Cube 0 Data;
	* CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;
	* CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeClass = NSData |
| CIAttributeFilterName | CIColorCubesMixedWithMask |
| CIAttributeFilterDisplayName | Color Cubes Mixed With Mask |
| inputCube1Data |
	* CIAttributeDisplayName = Cube 1 Data;
	* CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;
	* CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeClass = NSData |
| CIAttributeFilterAvailable_iOS | 11 |
| inputColorSpace |
	* CIAttributeDisplayName = Color Space;
	* CIAttributeClass = NSObject |
| CIAttributeReferenceDocumentation | [CIColorCubesMixedWithMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCubesMixedWithMask) |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIKaleidoscope:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Kaleidoscope |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of reflection.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIKaleidoscope |
| CIAttributeReferenceDocumentation | [CIKaleidoscope Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIKaleidoscope) |
| inputCount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The number of reflections in the pattern.;
	* CIAttributeDefault = 6;
	* CIAttributeDisplayName = Count;
	* CIAttributeSliderMax = 64;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBarcodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Barcode Generator |
| inputBarcodeDescriptor |
	* CIAttributeDescription = The CIBarcodeDescription object to generate an image for.;
	* CIAttributeDisplayName = Barcode Descriptor;
	* CIAttributeClass = CIBarcodeDescriptor |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBarcodeGenerator |
| CIAttributeReferenceDocumentation | [CIBarcodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBarcodeGenerator) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIAreaHistogram:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Area Histogram |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image whose histogram you want to calculate.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaHistogram |
| CIAttributeReferenceDocumentation | [CIAreaHistogram Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaHistogram) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scale value to use for the histogram values. If the scale is 1.0, then the bins in the resulting image will add up to 1.0.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The number of bins for the histogram. This value will determine the width of the output image.;
	* CIAttributeDefault = 64;
	* CIAttributeDisplayName = Count;
	* CIAttributeSliderMax = 1000;
	* CIAttributeMin = 1;
	* CIAttributeMax = 2048;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 10 |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that, after intersection with the image extent, specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIEdgePreserveUpsampleFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Edge Preserve Upsample Filter |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIEdgePreserveUpsampleFilter |
| CIAttributeReferenceDocumentation | [CIEdgePreserveUpsampleFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEdgePreserveUpsampleFilter) |
| inputLumaSigma |
	* CIAttributeMax = 1;
	* CIAttributeDisplayName = Luma Sigma;
	* CIAttributeDefault = 0.15;
	* CIAttributeClass = NSNumber;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar |
| inputSmallImage |
	* CIAttributeDisplayName = Small Image;
	* CIAttributeClass = Image |
| inputSpatialSigma |
	* CIAttributeMax = 5;
	* CIAttributeDisplayName = Spatial Sigma;
	* CIAttributeDefault = 3;
	* CIAttributeClass = NSNumber;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIColorMatrix:
| Attribute | Value |
| ---------- | --------- |
| inputGVector |
	* CIAttributeDisplayName = Green Vector;
	* CIAttributeDescription = The amount of green to multiply the source color values by.;
	* CIAttributeIdentity = [0 1 0 0];
	* CIAttributeDefault = [0 1 0 0];
	* CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputBiasVector |
	* CIAttributeDisplayName = Bias Vector;
	* CIAttributeDescription = A vector that’s added to each color component.;
	* CIAttributeIdentity = [0 0 0 0];
	* CIAttributeDefault = [0 0 0 0];
	* CIAttributeClass = Vector |
| inputRVector |
	* CIAttributeDisplayName = Red Vector;
	* CIAttributeDescription = The amount of red to multiply the source color values by.;
	* CIAttributeIdentity = [1 0 0 0];
	* CIAttributeDefault = [1 0 0 0];
	* CIAttributeClass = Vector |
| CIAttributeFilterDisplayName | Color Matrix |
| CIAttributeFilterName | CIColorMatrix |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeReferenceDocumentation | [CIColorMatrix Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorMatrix) |
| inputAVector |
	* CIAttributeDisplayName = Alpha Vector;
	* CIAttributeDescription = The amount of alpha to multiply the source color values by.;
	* CIAttributeIdentity = [0 0 0 1];
	* CIAttributeDefault = [0 0 0 1];
	* CIAttributeClass = Vector |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| inputBVector |
	* CIAttributeDisplayName = Blue Vector;
	* CIAttributeDescription = The amount of blue to multiply the source color values by.;
	* CIAttributeIdentity = [0 0 1 0];
	* CIAttributeDefault = [0 0 1 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CISampleNearest:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Sample Nearest |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISampleNearest |
| CIAttributeReferenceDocumentation | [CISampleNearest Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISampleNearest) |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIHoleDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Hole Distortion |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHoleDistortion |
| CIAttributeReferenceDocumentation | [CIHoleDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHoleDistortion) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 150;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 1000;
	* CIAttributeMin = 0.01;
	* CIAttributeIdentity = 0.1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.01 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIExclusionBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Exclusion Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIExclusionBlendMode |
| CIAttributeReferenceDocumentation | [CIExclusionBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIExclusionBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIGlassDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Glass Distortion |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIGlassDistortion |
| CIAttributeReferenceDocumentation | [CIGlassDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGlassDistortion) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of texturing of the resulting image. The larger the value, the greater the texturing.;
	* CIAttributeDefault = 200;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 500;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.01 |
| inputTexture |
	* CIAttributeDisplayName = Texture;
	* CIAttributeDescription = A texture to apply to the source image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIDepthBlurEffect:
| Attribute | Value |
| ---------- | --------- |
| inputNosePositions |
	* CIAttributeDisplayName = Nose Positions;
	* CIAttributeDefault = [-1 -1];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputCalibrationData |
	* CIAttributeDisplayName = Calibration Data;
	* CIAttributeClass = AVCameraCalibrationData |
| CIAttributeFilterName | CIDepthBlurEffect |
| inputChinPositions |
	* CIAttributeDisplayName = Chin Positions;
	* CIAttributeDefault = [-1 -1];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.13 |
| CIAttributeFilterAvailable_iOS | 11 |
| inputLumaNoiseScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 0.1;
	* CIAttributeDisplayName = Luma Noise Scale;
	* CIAttributeMin = 0;
	* CIAttributeMax = 0.1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputDisparityImage |
	* CIAttributeDisplayName = Disparity Image;
	* CIAttributeClass = Image |
| inputScaleFactor |
	* CIAttributeDisplayName = Scale Factor;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0;
	* CIAttributeDefault = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 1 |
| inputMatteImage |
	* CIAttributeDescription = A matting image.;
	* CIAttributeDisplayName = Matte Image;
	* CIAttributeClass = Image |
| inputLeftEyePositions |
	* CIAttributeDisplayName = Left Eye Positions;
	* CIAttributeDefault = [-1 -1];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeReferenceDocumentation | [CIDepthBlurEffect Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDepthBlurEffect) |
| inputShape |
	* CIAttributeDisplayName = Shape;
	* CIAttributeClass = NSString |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputRightEyePositions |
	* CIAttributeDisplayName = Right Eye Positions;
	* CIAttributeDefault = [-1 -1];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputAuxDataMetadata |
	* CIAttributeDisplayName = Aux Data Metadata;
	* CIAttributeClass = CGImageMetadataRef |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterDisplayName | Depth Blur Effect |
| inputFocusRect |
	* CIAttributeDisplayName = Focus Rectangle;
	* CIAttributeIdentity = [-8.98847e+307 -8.98847e+307 1.79769e+308 1.79769e+308];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| inputAperture |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 22;
	* CIAttributeDisplayName = Aperture;
	* CIAttributeMin = 0;
	* CIAttributeMax = 22;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |


#### CIDither:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Dither |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDither |
| CIAttributeReferenceDocumentation | [CIDither Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDither) |
| inputIntensity |
	* CIAttributeDefault = 0.1;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the effect.;
	* CIAttributeMin = 0;
	* CIAttributeMax = 5;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIAreaMinimumAlpha:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Minimum Alpha |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinimumAlpha |
| CIAttributeReferenceDocumentation | [CIAreaMinimumAlpha Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinimumAlpha) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIDroste:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.6 |
| inputZoom |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 1;
	* CIAttributeSliderMax = 5;
	* CIAttributeDisplayName = Zoom;
	* CIAttributeMin = 0.01;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.01 |
| inputInsetPoint1 |
	* CIAttributeDisplayName = Inset Point 1;
	* CIAttributeDefault = [400 400];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterName | CIDroste |
| CIAttributeFilterDisplayName | Droste |
| inputRotation |
	* CIAttributeDisplayName = Rotation;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = 0;
	* CIAttributeDefault = 0;
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 6.283185307179586 |
| CIAttributeFilterAvailable_iOS | 9 |
| inputStrands |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 1;
	* CIAttributeSliderMax = 2;
	* CIAttributeDisplayName = Strands;
	* CIAttributeMin = -10;
	* CIAttributeMax = 10;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -2 |
| CIAttributeReferenceDocumentation | [CIDroste Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDroste) |
| inputPeriodicity |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 1;
	* CIAttributeSliderMax = 5;
	* CIAttributeDisplayName = Periodicity;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |
| inputInsetPoint0 |
	* CIAttributeDisplayName = Inset Point 0;
	* CIAttributeDefault = [200 200];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIFourfoldTranslatedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Fourfold Translated Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIFourfoldTranslatedTile |
| CIAttributeReferenceDocumentation | [CIFourfoldTranslatedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFourfoldTranslatedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputAcuteAngle |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The primary angle for the repeating translated tile. Small values create thin diamond tiles, and higher values create fatter translated tiles.;
	* CIAttributeDefault = 1.570796326794897;
	* CIAttributeDisplayName = Acute Angle;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeIdentity = 1.570796326794897;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIDepthOfField:
| Attribute | Value |
| ---------- | --------- |
| inputPoint0 |
	* CIAttributeDisplayName = Point 0;
	* CIAttributeDefault = [0 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.6 |
| inputPoint1 |
	* CIAttributeDisplayName = Point 1;
	* CIAttributeDefault = [300 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterName | CIDepthOfField |
| CIAttributeFilterDisplayName | Depth of Field |
| inputUnsharpMaskRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 10;
	* CIAttributeDefault = 2.5;
	* CIAttributeDisplayName = Unsharp Mask Radius;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputSaturation |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount to adjust the saturation.;
	* CIAttributeDefault = 1.5;
	* CIAttributeDisplayName = Saturation;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIDepthOfField Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDepthOfField) |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputUnsharpMaskIntensity |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 10;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Unsharp Mask Intensity;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance from the center of the effect.;
	* CIAttributeDefault = 6;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 30;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CITriangleTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Triangle Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CITriangleTile |
| CIAttributeReferenceDocumentation | [CITriangleTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITriangleTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISaliencyMapFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Saliency Map Filter |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryStylize |
| CIAttributeFilterName | CISaliencyMapFilter |
| CIAttributeReferenceDocumentation | [CISaliencyMapFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISaliencyMapFilter) |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CISaturationBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Saturation Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISaturationBlendMode |
| CIAttributeReferenceDocumentation | [CISaturationBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISaturationBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISourceAtopCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Source Atop |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISourceAtopCompositing |
| CIAttributeReferenceDocumentation | [CISourceAtopCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISourceAtopCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColumnAverage:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Column Average |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColumnAverage |
| CIAttributeReferenceDocumentation | [CIColumnAverage Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColumnAverage) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIFourfoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Fourfold Reflected Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIFourfoldReflectedTile |
| CIAttributeReferenceDocumentation | [CIFourfoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIFourfoldReflectedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputAcuteAngle |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The primary angle for the repeating reflected tile. Small values create thin diamond tiles, and higher values create fatter reflected tiles.;
	* CIAttributeDefault = 1.570796326794897;
	* CIAttributeDisplayName = Acute Angle;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeIdentity = 1.570796326794897;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIShadedMaterial:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Shaded Material |
| inputShadingImage |
	* CIAttributeDisplayName = Shading Image;
	* CIAttributeDescription = The image to use as the height field. The resulting image has greater heights with lighter shades, and lesser heights (lower areas) with darker shades.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIShadedMaterial |
| CIAttributeReferenceDocumentation | [CIShadedMaterial Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIShadedMaterial) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scale of the effect. The higher the value, the more dramatic the effect.;
	* CIAttributeDefault = 10;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.5 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CITwelvefoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Twelvefold Reflected Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CITwelvefoldReflectedTile |
| CIAttributeReferenceDocumentation | [CITwelvefoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITwelvefoldReflectedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIMaximumCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Maximum |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMaximumCompositing |
| CIAttributeReferenceDocumentation | [CIMaximumCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaximumCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBoxBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Box Blur |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBoxBlur |
| CIAttributeReferenceDocumentation | [CIBoxBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBoxBlur) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;
	* CIAttributeDefault = 10;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIBumpDistortionLinear:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Bump Distortion Linear |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 6.283185307179586;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the line around which the distortion occurs.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBumpDistortionLinear |
| CIAttributeReferenceDocumentation | [CIBumpDistortionLinear Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBumpDistortionLinear) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scale of the effect.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = -1;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 600;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIGaussianBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Gaussian Blur |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIGaussianBlur |
| CIAttributeReferenceDocumentation | [CIGaussianBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGaussianBlur) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;
	* CIAttributeDefault = 10;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVibrance:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Vibrance |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIVibrance |
| CIAttributeReferenceDocumentation | [CIVibrance Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVibrance) |
| inputAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount to adjust the saturation.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Amount;
	* CIAttributeSliderMin = -1;
	* CIAttributeMin = -1;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIMorphologyMaximum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Morphology Maximum |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMorphologyMaximum |
| CIAttributeReferenceDocumentation | [CIMorphologyMaximum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMorphologyMaximum) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The desired radius of the circular morphological operation to the image.;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 50;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIPhotoEffectInstant:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Instant |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectInstant |
| CIAttributeReferenceDocumentation | [CIPhotoEffectInstant Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectInstant) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIColorMap:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Color Map |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorMap |
| CIAttributeReferenceDocumentation | [CIColorMap Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorMap) |
| inputGradientImage |
	* CIAttributeDisplayName = Gradient Image;
	* CIAttributeDescription = The image data from this image transforms the source image values.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeGradient |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPageCurlTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the curling page.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| CIAttributeFilterName | CIPageCurlTransition |
| CIAttributeFilterDisplayName | Page Curl |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = The extent of the effect.;
	* CIAttributeDefault = [0 0 300 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| inputShadingImage |
	* CIAttributeDisplayName = Shading Image;
	* CIAttributeDescription = An image that looks like a shaded sphere enclosed in a square image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIPageCurlTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPageCurlTransition) |
| inputBacksideImage |
	* CIAttributeDescription = The image that appears on the back of the source image, as the page curls to reveal the target image.;
	* CIAttributeDisplayName = Backside Image;
	* CIAttributeClass = Image |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the curl.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 400;
	* CIAttributeMin = 0.01;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.01 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIStripesGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Stripes |
| inputColor1 |
	* CIAttributeDisplayName = Color 2;
	* CIAttributeDescription = A color to use for the even stripes.;
	* CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIStripesGenerator |
| inputColor0 |
	* CIAttributeDisplayName = Color 1;
	* CIAttributeDescription = A color to use for the odd stripes.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| CIAttributeReferenceDocumentation | [CIStripesGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStripesGenerator) |
| inputWidth |
	* CIAttributeDefault = 80;
	* CIAttributeDescription = The width of a stripe.;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 800;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The sharpness of the stripe pattern. The smaller the value, the more blurry the pattern. Values range from 0.0 to 1.0.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the stripe pattern.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAreaMinMaxRed:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Area Min and Max Red |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinMaxRed |
| CIAttributeReferenceDocumentation | [CIAreaMinMaxRed Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinMaxRed) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CICircularScreen:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Circular Screen |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryHalftoneEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICircularScreen |
| CIAttributeReferenceDocumentation | [CICircularScreen Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICircularScreen) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance between each circle in the pattern.;
	* CIAttributeDefault = 6;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 50;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 2 |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The sharpness of the circles. The larger the value, the sharper the circles.;
	* CIAttributeDefault = 0.7;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the circular screen pattern;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILightTunnel:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Light Tunnel Distortion |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILightTunnel |
| CIAttributeReferenceDocumentation | [CILightTunnel Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILightTunnel) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Center radius of the light tunnel.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 500;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputRotation |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Rotation angle of the light tunnel.;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = Rotation;
	* CIAttributeSliderMax = 1.570796326794897;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = Center of the light tunnel.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMultiplyBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Multiply Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMultiplyBlendMode |
| CIAttributeReferenceDocumentation | [CIMultiplyBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMultiplyBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorControls:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Controls |
| inputSaturation |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of saturation to apply. The larger the value, the more saturated the result.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Saturation;
	* CIAttributeSliderMax = 2;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorControls |
| CIAttributeReferenceDocumentation | [CIColorControls Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorControls) |
| inputBrightness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of brightness to apply. The larger the value, the brighter the result.;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = Brightness;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = -1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -1 |
| inputContrast |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of contrast to apply. The larger the value, the more contrast in the resulting image.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Contrast;
	* CIAttributeSliderMax = 4;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.25 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CITextImageGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Text Image Generator |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputText |
	* CIAttributeDisplayName = Text;
	* CIAttributeClass = NSString |
| CIAttributeFilterName | CITextImageGenerator |
| CIAttributeReferenceDocumentation | [CITextImageGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITextImageGenerator) |
| inputFontName |
	* CIAttributeDefault = HelveticaNeue;
	* CIAttributeDisplayName = Font Name;
	* CIAttributeClass = NSString |
| inputScaleFactor |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 4;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Scale Factor;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |
| inputFontSize |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 128;
	* CIAttributeDefault = 12;
	* CIAttributeDisplayName = Font Size;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 9 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILinearToSRGBToneCurve:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Linear to sRGB Tone Curve |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILinearToSRGBToneCurve |
| CIAttributeReferenceDocumentation | [CILinearToSRGBToneCurve Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearToSRGBToneCurve) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIColorPolynomial:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Polynomial |
| inputRedCoefficients |
	* CIAttributeDisplayName = Red Coefficients;
	* CIAttributeDescription = Polynomial coefficients for red channel;
	* CIAttributeIdentity = [0 1 0 0];
	* CIAttributeDefault = [0 1 0 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorPolynomial |
| CIAttributeReferenceDocumentation | [CIColorPolynomial Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorPolynomial) |
| inputGreenCoefficients |
	* CIAttributeDisplayName = Green Coefficients;
	* CIAttributeDescription = Polynomial coefficients for green channel;
	* CIAttributeIdentity = [0 1 0 0];
	* CIAttributeDefault = [0 1 0 0];
	* CIAttributeClass = Vector |
| inputAlphaCoefficients |
	* CIAttributeDisplayName = Alpha Coefficients;
	* CIAttributeDescription = Polynomial coefficients for alpha channel;
	* CIAttributeIdentity = [0 1 0 0];
	* CIAttributeDefault = [0 1 0 0];
	* CIAttributeClass = Vector |
| inputBlueCoefficients |
	* CIAttributeDisplayName = Blue Coefficients;
	* CIAttributeDescription = Polynomial coefficients for blue channel;
	* CIAttributeIdentity = [0 1 0 0];
	* CIAttributeDefault = [0 1 0 0];
	* CIAttributeClass = Vector |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIConstantColorGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Constant Color |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIConstantColorGenerator |
| CIAttributeReferenceDocumentation | [CIConstantColorGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConstantColorGenerator) |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The color to generate.;
	* CIAttributeDefault = (1 0 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIGlassLozenge:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Glass Lozenge |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIGlassLozenge |
| CIAttributeReferenceDocumentation | [CIGlassLozenge Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGlassLozenge) |
| inputPoint1 |
	* CIAttributeDisplayName = Point 1;
	* CIAttributeDescription = The x and y position that defines the center of the circle at the other end of the lozenge.;
	* CIAttributeDefault = [350 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the lozenge. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeSliderMax = 1000;
	* CIAttributeDisplayName = Radius;
	* CIAttributeDefault = 100;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputRefraction |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The refraction of the glass.;
	* CIAttributeSliderMax = 5;
	* CIAttributeDisplayName = Refraction;
	* CIAttributeDefault = 1.7;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputPoint0 |
	* CIAttributeDisplayName = Point 0;
	* CIAttributeDescription = The x and y position that defines the center of the circle at one end of the lozenge.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISixfoldRotatedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Sixfold Rotated Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISixfoldRotatedTile |
| CIAttributeReferenceDocumentation | [CISixfoldRotatedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISixfoldRotatedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CICopyMachineTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The color of the copier light.;
	* CIAttributeDefault = (0.6 1 0.8 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeOpaqueColor |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 6.283185307179586;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the copier light.;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of the copier light. ;
	* CIAttributeDefault = 200;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 500;
	* CIAttributeMin = 0.1;
	* CIAttributeIdentity = 200;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.1 |
| CIAttributeFilterName | CICopyMachineTransition |
| CIAttributeFilterDisplayName | Copy Machine |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that defines the extent of the effect.;
	* CIAttributeDefault = [0 0 300 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CICopyMachineTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICopyMachineTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputOpacity |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The opacity of the copier light. A value of 0.0 is transparent. A value of 1.0 is opaque.;
	* CIAttributeDefault = 1.3;
	* CIAttributeDisplayName = Opacity;
	* CIAttributeSliderMax = 3;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1.3;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIGloom:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Gloom |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIGloom |
| CIAttributeReferenceDocumentation | [CIGloom Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGloom) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the effect. The larger the radius, the greater the effect.;
	* CIAttributeDefault = 10;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputIntensity |
	* CIAttributeDefault = 0.5;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the effect. A value of 0.0 is no effect. A value of 1.0 is the maximum effect.;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISpotColor:
| Attribute | Value |
| ---------- | --------- |
| inputCenterColor2 |
	* CIAttributeDisplayName = Center Color 2;
	* CIAttributeDescription = The center value of the second color range to replace.;
	* CIAttributeDefault = (0.5255 0.3059 0.3451 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| CIAttributeFilterAvailable_Mac | 10.5 |
| inputCloseness2 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = A value that indicates how close the second color must match before it is replaced.;
	* CIAttributeDefault = 0.15;
	* CIAttributeDisplayName = Closeness 2;
	* CIAttributeSliderMax = 0.5;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputContrast1 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The contrast of the first replacement color.;
	* CIAttributeDefault = 0.98;
	* CIAttributeDisplayName = Contrast 1;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenterColor1 |
	* CIAttributeDisplayName = Center Color 1;
	* CIAttributeDescription = The center value of the first color range to replace.;
	* CIAttributeDefault = (0.0784 0.0627 0.0706 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| inputCloseness3 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = A value that indicates how close the third color must match before it is replaced.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Closeness 3;
	* CIAttributeSliderMax = 0.5;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputContrast3 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The contrast of the third replacement color.;
	* CIAttributeDefault = 0.99;
	* CIAttributeDisplayName = Contrast 3;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CISpotColor |
| CIAttributeFilterDisplayName | Spot Color |
| inputCloseness1 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = A value that indicates how close the first color must match before it is replaced.;
	* CIAttributeDefault = 0.22;
	* CIAttributeDisplayName = Closeness 1;
	* CIAttributeSliderMax = 0.5;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputContrast2 |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The contrast of the second replacement color.;
	* CIAttributeDefault = 0.98;
	* CIAttributeDisplayName = Contrast 2;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CISpotColor Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISpotColor) |
| inputReplacementColor1 |
	* CIAttributeDisplayName = Replacement Color 1;
	* CIAttributeDescription = A replacement color for the first color range.;
	* CIAttributeDefault = (0.4392 0.1922 0.1961 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| CIAttributeFilterCategories |
	* CICategoryBuiltIn;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryStylize |
| inputReplacementColor2 |
	* CIAttributeDisplayName = Replacement Color 2;
	* CIAttributeDescription = A replacement color for the second color range.;
	* CIAttributeDefault = (0.9137 0.5608 0.5059 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| inputCenterColor3 |
	* CIAttributeDisplayName = Center Color 3;
	* CIAttributeDescription = The center value of the third color range to replace.;
	* CIAttributeDefault = (0.9216 0.4549 0.3333 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| inputReplacementColor3 |
	* CIAttributeDisplayName = Replacement Color 3;
	* CIAttributeDescription = A replacement color for the third color range.;
	* CIAttributeDefault = (0.9098 0.7529 0.6078 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIAreaMinimum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Minimum |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinimum |
| CIAttributeReferenceDocumentation | [CIAreaMinimum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinimum) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CICrystallize:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Crystallize |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICrystallize |
| CIAttributeReferenceDocumentation | [CICrystallize Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICrystallize) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the effect. The larger the radius, the larger the resulting crystals.;
	* CIAttributeDefault = 20;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 1;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorDodgeBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Dodge Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorDodgeBlendMode |
| CIAttributeReferenceDocumentation | [CIColorDodgeBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorDodgeBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIWhitePointAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | White Point Adjust |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIWhitePointAdjust |
| CIAttributeReferenceDocumentation | [CIWhitePointAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIWhitePointAdjust) |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = A color to use as the white point.;
	* CIAttributeIdentity = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILinearDodgeBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Linear Dodge Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILinearDodgeBlendMode |
| CIAttributeReferenceDocumentation | [CILinearDodgeBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearDodgeBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CILinearBurnBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Linear Burn Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILinearBurnBlendMode |
| CIAttributeReferenceDocumentation | [CILinearBurnBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearBurnBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIClamp:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Clamp |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIClamp |
| CIAttributeReferenceDocumentation | [CIClamp Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIClamp) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that defines the extent of the effect.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIPhotoEffectTonal:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Tonal |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectTonal |
| CIAttributeReferenceDocumentation | [CIPhotoEffectTonal Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectTonal) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIDissolveTransition:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Dissolve |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDissolveTransition |
| CIAttributeReferenceDocumentation | [CIDissolveTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDissolveTransition) |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIHardLightBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Hard Light Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHardLightBlendMode |
| CIAttributeReferenceDocumentation | [CIHardLightBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHardLightBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPageCurlWithShadowTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.9 |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the curling page.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputShadowSize |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The maximum size in pixels of the shadow.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Shadow Size;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputShadowAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The strength of the shadow.;
	* CIAttributeDefault = 0.7;
	* CIAttributeDisplayName = Shadow Amount;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputShadowExtent |
	* CIAttributeDisplayName = Shadow Extent;
	* CIAttributeDescription = The rectagular portion of input image that will cast a shadow.;
	* CIAttributeDefault = [0 0 0 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterName | CIPageCurlWithShadowTransition |
| CIAttributeFilterDisplayName | Page Curl With Shadow |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = The extent of the effect.;
	* CIAttributeDefault = [0 0 0 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIPageCurlWithShadowTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPageCurlWithShadowTransition) |
| inputBacksideImage |
	* CIAttributeDescription = The image that appears on the back of the source image, as the page curls to reveal the target image.;
	* CIAttributeDisplayName = Backside Image;
	* CIAttributeClass = Image |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the curl.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 400;
	* CIAttributeMin = 0.01;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.01 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIGaussianGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Gaussian Gradient |
| inputColor1 |
	* CIAttributeDisplayName = Color 2;
	* CIAttributeDescription = The second color to use in the gradient.;
	* CIAttributeDefault = (0 0 0 0) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterCategories |
	* CICategoryGradient;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIGaussianGradient |
| inputColor0 |
	* CIAttributeDisplayName = Color 1;
	* CIAttributeDescription = The first color to use in the gradient.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeReferenceDocumentation | [CIGaussianGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGaussianGradient) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the Gaussian distribution.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBlendWithBlueMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Blend With Blue Mask |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithBlueMask |
| CIAttributeReferenceDocumentation | [CIBlendWithBlueMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithBlueMask) |
| inputMaskImage |
	* CIAttributeDisplayName = Mask Image;
	* CIAttributeDescription = A masking image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIHueAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Hue Adjust |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = An angle (in radians) to use to correct the hue of an image.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHueAdjust |
| CIAttributeReferenceDocumentation | [CIHueAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHueAdjust) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMorphologyMinimum:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Morphology Minimum |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMorphologyMinimum |
| CIAttributeReferenceDocumentation | [CIMorphologyMinimum Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMorphologyMinimum) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The desired radius of the circular morphological operation to the image.;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 50;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIStretchCrop:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Stretch Crop |
| inputCenterStretchAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Determine how much the center of the image is stretched if stretching is used. If value is 0 then the center of the image maintains the original aspect ratio. If 1 then the image is stretched uniformly.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Center Stretch Amount;
	* CIAttributeDefault = 0.25;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIStretchCrop |
| CIAttributeReferenceDocumentation | [CIStretchCrop Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStretchCrop) |
| inputCropAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Determines if and how much cropping should be used to achieve the target size. If value is 0 then only stretching is used. If 1 then only cropping is used.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Crop Amount;
	* CIAttributeDefault = 0.25;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputSize |
	* CIAttributeDisplayName = Size;
	* CIAttributeDescription = The size in pixels of the output image.;
	* CIAttributeDefault = [1280 720];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.6 |


#### CIBarsSwipeTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.5 |
| inputAngle |
	* CIAttributeDefault = 3.141592653589793;
	* CIAttributeSliderMax = 6.283185307179586;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the bars.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = 0 |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of each bar.;
	* CIAttributeDefault = 30;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 300;
	* CIAttributeMin = 2;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 2 |
| CIAttributeFilterName | CIBarsSwipeTransition |
| CIAttributeFilterDisplayName | Bars Swipe Transition |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIBarsSwipeTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBarsSwipeTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputBarOffset |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The offset of one bar with respect to another;
	* CIAttributeDefault = 10;
	* CIAttributeDisplayName = Bar Offset;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIEightfoldReflectedTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Eightfold Reflected Tile |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the tiled pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIEightfoldReflectedTile |
| CIAttributeReferenceDocumentation | [CIEightfoldReflectedTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEightfoldReflectedTile) |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of a tile.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 200;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 100;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CITemperatureAndTint:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Temperature and Tint |
| inputTargetNeutral |
	* CIAttributeIdentity = [6500 0];
	* CIAttributeDisplayName = Target Neutral;
	* CIAttributeDefault = [6500 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CITemperatureAndTint |
| CIAttributeReferenceDocumentation | [CITemperatureAndTint Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CITemperatureAndTint) |
| inputNeutral |
	* CIAttributeIdentity = [6500 0];
	* CIAttributeDisplayName = Neutral;
	* CIAttributeDefault = [6500 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| CIAttributeFilterAvailable_Mac | 10.7 |


#### CIConvolution9Vertical:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Vertical 9 Convolution |
| inputWeights |
	* CIAttributeDisplayName = Weights;
	* CIAttributeIdentity = [0 0 0 0 1 0 0 0 0];
	* CIAttributeDefault = [0 0 0 0 1 0 0 0 0];
	* CIAttributeClass = Vector |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIConvolution9Vertical |
| CIAttributeReferenceDocumentation | [CIConvolution9Vertical Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIConvolution9Vertical) |
| inputBias |
	* CIAttributeDisplayName = Bias;
	* CIAttributeIdentity = 0;
	* CIAttributeDefault = 0;
	* CIAttributeClass = NSNumber |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIGammaAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Gamma Adjust |
| inputPower |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = A gamma value to use to correct image brightness. The larger the value, the darker the result.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Power;
	* CIAttributeSliderMax = 4;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.25 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIGammaAdjust |
| CIAttributeReferenceDocumentation | [CIGammaAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIGammaAdjust) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIZoomBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8.3 |
| CIAttributeFilterDisplayName | Zoom Blur |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIZoomBlur |
| CIAttributeReferenceDocumentation | [CIZoomBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIZoomBlur) |
| inputAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The zoom-in amount. Larger values result in more zooming in.;
	* CIAttributeDefault = 20;
	* CIAttributeDisplayName = Amount;
	* CIAttributeSliderMax = 200;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = -200 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVignette:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Vignette |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIVignette |
| CIAttributeReferenceDocumentation | [CIVignette Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVignette) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance from the center of the effect.;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 2;
	* CIAttributeMin = 0;
	* CIAttributeMax = 2;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputIntensity |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the effect.;
	* CIAttributeMin = -1;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -1 |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIAccordionFoldTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputNumberOfFolds |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 3;
	* CIAttributeSliderMax = 10;
	* CIAttributeDisplayName = Number of Folds;
	* CIAttributeMin = 1;
	* CIAttributeMax = 50;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The duration of the effect.;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |
| CIAttributeFilterName | CIAccordionFoldTransition |
| CIAttributeFilterDisplayName | Accordion Fold Transition |
| inputBottomHeight |
	* CIAttributeDisplayName = Bottom Height;
	* CIAttributeMin = 0;
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 0;
	* CIAttributeType = CIAttributeTypeDistance |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeReferenceDocumentation | [CIAccordionFoldTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAccordionFoldTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputFoldShadowAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 0.1;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Fold Shadow Amount;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CISunbeamsGenerator:
| Attribute | Value |
| ---------- | --------- |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The duration of the effect.;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0 |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The color of the sun.;
	* CIAttributeDefault = (1 0.5 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| inputStriationStrength |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The intensity of the sunbeams. Higher values result in more intensity.;
	* CIAttributeDefault = 0.5;
	* CIAttributeDisplayName = Striation Strength;
	* CIAttributeSliderMax = 3;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0.5;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CISunbeamsGenerator |
| CIAttributeFilterDisplayName | Sunbeams |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the sunbeam pattern;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 9 |
| inputStriationContrast |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The contrast of the sunbeams. Higher values result in more contrast.;
	* CIAttributeDefault = 1.375;
	* CIAttributeDisplayName = Striation Contrast;
	* CIAttributeSliderMax = 5;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1.375;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CISunbeamsGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISunbeamsGenerator) |
| inputSunRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the sun.;
	* CIAttributeDefault = 40;
	* CIAttributeDisplayName = Sun Radius;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 40;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputMaxStriationRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the sunbeams.;
	* CIAttributeDefault = 2.58;
	* CIAttributeDisplayName = Maximum Striation Radius;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 2.58;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMaskedVariableBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Masked Variable Blur |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMaskedVariableBlur |
| CIAttributeReferenceDocumentation | [CIMaskedVariableBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaskedVariableBlur) |
| inputMask |
	* CIAttributeDisplayName = Mask;
	* CIAttributeClass = Image |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance from the center of the effect.;
	* CIAttributeDefault = 5;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIPinLightBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Pin Light Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIPinLightBlendMode |
| CIAttributeReferenceDocumentation | [CIPinLightBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPinLightBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMaskToAlpha:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Mask to Alpha |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMaskToAlpha |
| CIAttributeReferenceDocumentation | [CIMaskToAlpha Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMaskToAlpha) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CINinePartStretched:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Nine Part Stretched |
| inputGrowAmount |
	* CIAttributeDisplayName = Grow Amount;
	* CIAttributeDefault = [100 100];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CINinePartStretched |
| CIAttributeReferenceDocumentation | [CINinePartStretched Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CINinePartStretched) |
| inputBreakpoint0 |
	* CIAttributeDisplayName = Breakpoint0;
	* CIAttributeDescription = Lower left corner of image to retain before stretching begins.;
	* CIAttributeDefault = [50 50];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputBreakpoint1 |
	* CIAttributeDisplayName = Breakpoint1;
	* CIAttributeDescription = Upper right corner of image to retain after stretching ends.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIScreenBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Screen Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIScreenBlendMode |
| CIAttributeReferenceDocumentation | [CIScreenBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIScreenBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVignetteEffect:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Vignette Effect |
| inputIntensity |
	* CIAttributeDefault = 1;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Intensity;
	* CIAttributeDescription = The intensity of the effect.;
	* CIAttributeMin = -1;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -1 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIVignetteEffect |
| CIAttributeReferenceDocumentation | [CIVignetteEffect Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVignetteEffect) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance from the center of the effect.;
	* CIAttributeDefault = 150;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 2000;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputFalloff |
	* CIAttributeClass = NSNumber;
	* CIAttributeDefault = 0.5;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Falloff;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIRandomGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterDisplayName | Random Generator |
| CIAttributeFilterAvailable_Mac | 10.4 |
| CIAttributeReferenceDocumentation | [CIRandomGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRandomGenerator) |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIRandomGenerator |


#### CIDisintegrateWithMaskTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputMaskImage |
	* CIAttributeDisplayName = Mask Image;
	* CIAttributeDescription = An image that defines the shape to use when disintegrating from the source to the target image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterName | CIDisintegrateWithMaskTransition |
| CIAttributeFilterDisplayName | Disintegrate With Mask |
| inputShadowOffset |
	* CIAttributeDisplayName = Shadow Offset;
	* CIAttributeDescription = The offset of the shadow created by the mask.;
	* CIAttributeIdentity = [0 0];
	* CIAttributeDefault = [0 -10];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeOffset |
| inputShadowDensity |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The density of the shadow created by the mask.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Shadow Density;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0.65 |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CIDisintegrateWithMaskTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDisintegrateWithMaskTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputShadowRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the shadow created by the mask.;
	* CIAttributeDefault = 8;
	* CIAttributeDisplayName = Shadow Radius;
	* CIAttributeSliderMax = 50;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIMultiplyCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Multiply |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMultiplyCompositing |
| CIAttributeReferenceDocumentation | [CIMultiplyCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMultiplyCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPerspectiveTile:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Perspective Tile |
| inputTopRight |
	* CIAttributeDisplayName = Top Right;
	* CIAttributeDescription = The top right coordinate of a tile.;
	* CIAttributeDefault = [646 507];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryTileEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIPerspectiveTile |
| CIAttributeReferenceDocumentation | [CIPerspectiveTile Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPerspectiveTile) |
| inputBottomLeft |
	* CIAttributeDisplayName = Bottom Left;
	* CIAttributeDescription = The bottom left coordinate of a tile.;
	* CIAttributeDefault = [155 153];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputTopLeft |
	* CIAttributeDisplayName = Top Left;
	* CIAttributeDescription = The top left coordinate of a tile.;
	* CIAttributeDefault = [118 484];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputBottomRight |
	* CIAttributeDisplayName = Bottom Right;
	* CIAttributeDescription = The bottom right coordinate of a tile.;
	* CIAttributeDefault = [548 140];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILineOverlay:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.5 |
| inputNRNoiseLevel |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The noise level of the image (used with camera data) that gets removed before tracing the edges of the image. Increasing the noise level helps to clean up the traced edges of the image.;
	* CIAttributeSliderMax = 0.1;
	* CIAttributeDisplayName = NR Noise Level;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0.07000000000000001 |
| inputContrast |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of anti-aliasing to use on the edges produced by this filter. Higher values produce higher contrast edges (they are less anti-aliased).;
	* CIAttributeSliderMax = 200;
	* CIAttributeDisplayName = Contrast;
	* CIAttributeSliderMin = 0.25;
	* CIAttributeMin = 0.25;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 50 |
| inputThreshold |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = This value determines edge visibility. Larger values thin out the edges.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Threshold;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0.1 |
| CIAttributeFilterName | CILineOverlay |
| CIAttributeFilterDisplayName | Line Overlay |
| inputEdgeIntensity |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The accentuation factor of the Sobel gradient information when tracing the edges of the image. Higher values find more edges, although typically a low value (such as 1.0) is used.;
	* CIAttributeSliderMax = 200;
	* CIAttributeDisplayName = Edge Intensity;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 1 |
| CIAttributeFilterAvailable_iOS | 9 |
| inputNRSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of sharpening done when removing noise in the image before tracing the edges of the image. This improves the edge acquisition.;
	* CIAttributeSliderMax = 2;
	* CIAttributeDisplayName = NR Sharpness;
	* CIAttributeSliderMin = 0;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0.71 |
| CIAttributeReferenceDocumentation | [CILineOverlay Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILineOverlay) |
| CIAttributeFilterCategories |
	* CICategoryBuiltIn;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryStylize |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIColorCube:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Cube |
| inputCubeDimension |
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Cube Dimension;
	* CIAttributeMin = 2;
	* CIAttributeMax = 128;
	* CIAttributeIdentity = 2;
	* CIAttributeType = CIAttributeTypeCount;
	* CIAttributeDefault = 2 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCube |
| CIAttributeReferenceDocumentation | [CIColorCube Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCube) |
| inputCubeData |
	* CIAttributeDisplayName = Cube Data;
	* CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;
	* CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeClass = NSData |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILuminosityBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Luminosity Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILuminosityBlendMode |
| CIAttributeReferenceDocumentation | [CILuminosityBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILuminosityBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CISwipeTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The color of the swipe.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeOpaqueColor |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the swipe.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of the swipe;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 0.1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.1 |
| CIAttributeFilterName | CISwipeTransition |
| CIAttributeFilterDisplayName | Swipe |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = The extent of the effect.;
	* CIAttributeDefault = [0 0 300 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeReferenceDocumentation | [CISwipeTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISwipeTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputOpacity |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The opacity of the swipe.;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = Opacity;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIPixellate:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Pixelate |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIPixellate |
| CIAttributeReferenceDocumentation | [CIPixellate Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPixellate) |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The scale determines the size of the squares. Larger values result in larger squares.;
	* CIAttributeDefault = 8;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIExposureAdjust:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Exposure Adjust |
| inputEV |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount to adjust the exposure of the image by. The larger the value, the brighter the exposure.;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = EV;
	* CIAttributeSliderMax = 10;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -10 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIExposureAdjust |
| CIAttributeReferenceDocumentation | [CIExposureAdjust Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIExposureAdjust) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CILinearGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Linear Gradient |
| inputColor1 |
	* CIAttributeDisplayName = Color 2;
	* CIAttributeDescription = The second color to use in the gradient.;
	* CIAttributeDefault = (0 0 0 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeFilterCategories |
	* CICategoryGradient;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILinearGradient |
| inputColor0 |
	* CIAttributeDisplayName = Color 1;
	* CIAttributeDescription = The first color to use in the gradient.;
	* CIAttributeDefault = (1 1 1 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color;
	* CIAttributeType = CIAttributeTypeColor |
| CIAttributeReferenceDocumentation | [CILinearGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILinearGradient) |
| inputPoint1 |
	* CIAttributeDisplayName = Point 1;
	* CIAttributeDescription = The ending position of the gradient -- where the second color begins.;
	* CIAttributeDefault = [200 200];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| inputPoint0 |
	* CIAttributeDisplayName = Point 0;
	* CIAttributeDescription = The starting position of the gradient -- where the first color begins.;
	* CIAttributeDefault = [0 0];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CICMYKHalftone:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the pattern.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The sharpness of the pattern. The larger the value, the sharper the pattern.;
	* CIAttributeDefault = 0.7;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 1;
	* CIUIParameterSet = CIUISetBasic;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance between dots in the pattern.;
	* CIAttributeSliderMax = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMin = 2;
	* CIUIParameterSet = CIUISetBasic;
	* CIAttributeMin = -2;
	* CIAttributeIdentity = 6;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeDefault = 6 |
| inputUCR |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The under color removal value. The value can vary from 0.0 to 1.0. ;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Under Color Removal;
	* CIAttributeSliderMin = 0;
	* CIUIParameterSet = CIUISetIntermediate;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0.5;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 0.5 |
| CIAttributeFilterName | CICMYKHalftone |
| CIAttributeFilterDisplayName | CMYK Halftone |
| inputGCR |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The gray component replacement value. The value can vary from 0.0 (none) to 1.0.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Gray Component Replacement;
	* CIAttributeSliderMin = 0;
	* CIUIParameterSet = CIUISetIntermediate;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeDefault = 1 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the halftone pattern;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CICMYKHalftone Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICMYKHalftone) |
| CIAttributeFilterCategories |
	* CICategoryHalftoneEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CISoftLightBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Soft Light Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISoftLightBlendMode |
| CIAttributeReferenceDocumentation | [CISoftLightBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISoftLightBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIStarShineGenerator:
| Attribute | Value |
| ---------- | --------- |
| inputColor |
	* CIAttributeDisplayName = Color;
	* CIAttributeDescription = The color to use for the outer shell of the circular star.;
	* CIAttributeDefault = (1 0.8 0.6 1) <CGColorSpace 0x600002600720> (kCGColorSpaceDeviceRGB);
	* CIAttributeClass = Color |
| inputCrossScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The size of the cross pattern.;
	* CIAttributeDefault = 15;
	* CIAttributeDisplayName = Cross Scale;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 15;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterName | CIStarShineGenerator |
| CIAttributeFilterDisplayName | Star Shine |
| inputCrossWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of the cross pattern.;
	* CIAttributeDefault = 2.5;
	* CIAttributeDisplayName = Cross Width;
	* CIAttributeSliderMax = 10;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0.5 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the star.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 6 |
| inputCrossOpacity |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The opacity of the cross pattern.;
	* CIAttributeDefault = -2;
	* CIAttributeDisplayName = Cross Opacity;
	* CIAttributeSliderMax = 0;
	* CIAttributeMin = -8;
	* CIAttributeIdentity = -2;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -8 |
| CIAttributeReferenceDocumentation | [CIStarShineGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIStarShineGenerator) |
| inputCrossAngle |
	* CIAttributeDefault = 0.6;
	* CIAttributeDescription = The angle of the cross pattern.;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Cross Angle;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius of the star.;
	* CIAttributeDefault = 50;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 300;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputEpsilon |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The length of the cross spikes.;
	* CIAttributeDefault = -2;
	* CIAttributeDisplayName = Epsilon;
	* CIAttributeSliderMax = 0;
	* CIAttributeMin = -8;
	* CIAttributeIdentity = -2;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -8 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CICoreMLModelFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | CoreML Model Filter |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryStylize |
| CIAttributeFilterName | CICoreMLModelFilter |
| CIAttributeReferenceDocumentation | [CICoreMLModelFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICoreMLModelFilter) |
| inputModel |
	* CIAttributeDescription = The CoreML model to be used for applying effect on the image.;
	* CIAttributeDisplayName = Model;
	* CIAttributeClass = MLModel |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CIBlendWithAlphaMask:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Blend With Alpha Mask |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBlendWithAlphaMask |
| CIAttributeReferenceDocumentation | [CIBlendWithAlphaMask Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBlendWithAlphaMask) |
| inputMaskImage |
	* CIAttributeDisplayName = Mask Image;
	* CIAttributeDescription = A masking image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIHueSaturationValueGradient:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 10 |
| CIAttributeFilterDisplayName | Hue/Saturation/Value Gradient |
| inputColorSpace |
	* CIAttributeDisplayName = Color Space;
	* CIAttributeDescription = The CGColorSpaceRef that the color wheel should be generated in.;
	* CIAttributeDefault = <CGColorSpace 0x6000026007e0> (kCGColorSpaceICCBased; kCGColorSpaceModelRGB; sRGB IEC61966-2.1);
	* CIAttributeClass = NSObject |
| CIAttributeFilterCategories |
	* CICategoryGradient;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIHueSaturationValueGradient |
| CIAttributeReferenceDocumentation | [CIHueSaturationValueGradient Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIHueSaturationValueGradient) |
| inputDither |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 3;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Dither;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputValue |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 1;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Value;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance from the center of the effect.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputSoftness |
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 1;
	* CIAttributeDefault = 1;
	* CIAttributeDisplayName = Softness;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.12 |


#### CIColorInvert:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Invert |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorInvert |
| CIAttributeReferenceDocumentation | [CIColorInvert Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorInvert) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIRippleTransition:
| Attribute | Value |
| ---------- | --------- |
| inputTargetImage |
	* CIAttributeDisplayName = Target Image;
	* CIAttributeDescription = The target image for a transition.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputTime |
	* CIAttributeSliderMin = 0;
	* CIAttributeSliderMax = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Time;
	* CIAttributeDescription = The parametric time of the transition. This value drives the transition from start (at time 0) to end (at time 1).;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeTime;
	* CIAttributeDefault = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |
| inputWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The width of the ripple.;
	* CIAttributeDefault = 100;
	* CIAttributeDisplayName = Width;
	* CIAttributeSliderMax = 300;
	* CIAttributeMin = 1;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 10 |
| CIAttributeFilterName | CIRippleTransition |
| CIAttributeFilterDisplayName | Ripple |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that defines the extent of the effect.;
	* CIAttributeDefault = [0 0 300 300];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| inputShadingImage |
	* CIAttributeDisplayName = Shading Image;
	* CIAttributeDescription = An image that looks like a shaded sphere enclosed in a square image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The x and y position to use as the center of the effect;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_iOS | 9 |
| inputScale |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = A value that determines whether the ripple starts as a bulge (higher value) or a dimple (lower value).;
	* CIAttributeDefault = 50;
	* CIAttributeDisplayName = Scale;
	* CIAttributeSliderMax = 50;
	* CIAttributeMin = -50;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = -50 |
| CIAttributeReferenceDocumentation | [CIRippleTransition Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIRippleTransition) |
| CIAttributeFilterCategories |
	* CICategoryTransition;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |


#### CIAztecCodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Aztec Code Generator |
| inputMessage |
	* CIAttributeDescription = The message to encode in the Aztec Barcode;
	* CIAttributeDisplayName = Message;
	* CIAttributeClass = NSData |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAztecCodeGenerator |
| inputCorrectionLevel |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Aztec error correction value between 5 and 95;
	* CIAttributeDefault = 23;
	* CIAttributeDisplayName = Correction Level;
	* CIAttributeSliderMax = 95;
	* CIAttributeMin = 5;
	* CIAttributeMax = 95;
	* CIAttributeSliderMin = 5 |
| CIAttributeReferenceDocumentation | [CIAztecCodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAztecCodeGenerator) |
| inputLayers |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Aztec layers value between 1 and 32. Set to nil for automatic.;
	* CIAttributeSliderMax = 32;
	* CIAttributeDisplayName = Layers;
	* CIAttributeMin = 1;
	* CIAttributeMax = 32;
	* CIAttributeSliderMin = 1 |
| inputCompactStyle |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Force a compact style Aztec code to @YES or @NO. Set to nil for automatic.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Compact Style;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CIMotionBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8.3 |
| CIAttributeFilterDisplayName | Motion Blur |
| inputAngle |
	* CIAttributeDefault = 0;
	* CIAttributeSliderMax = 3.141592653589793;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle of the motion determines which direction the blur smears.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -3.141592653589793 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMotionBlur |
| CIAttributeReferenceDocumentation | [CIMotionBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMotionBlur) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;
	* CIAttributeDefault = 20;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMedianFilter:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Median |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryStillImage;
	* CICategoryVideo;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMedianFilter |
| CIAttributeReferenceDocumentation | [CIMedianFilter Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMedianFilter) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorCubeWithColorSpace:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Color Cube with ColorSpace |
| inputCubeDimension |
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Cube Dimension;
	* CIAttributeMin = 2;
	* CIAttributeMax = 128;
	* CIAttributeIdentity = 2;
	* CIAttributeType = CIAttributeTypeCount;
	* CIAttributeDefault = 2 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorCubeWithColorSpace |
| CIAttributeReferenceDocumentation | [CIColorCubeWithColorSpace Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorCubeWithColorSpace) |
| inputCubeData |
	* CIAttributeDisplayName = Cube Data;
	* CIAttributeDescription = Data containing a 3-dimensional color table of floating-point premultiplied RGBA values. The cells are organized in a standard ordering. The columns and rows of the data are indexed by red and green, respectively. Each data plane is followed by the next higher plane in the data, with planes indexed by blue.;
	* CIAttributeIdentity = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeDefault = <00000000 00000000 00000000 0000803f 0000803f 00000000 00000000 0000803f 00000000 0000803f 00000000 0000803f 0000803f 0000803f 00000000 0000803f 00000000 00000000 0000803f 0000803f 0000803f 00000000 0000803f 0000803f 00000000 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f 0000803f>;
	* CIAttributeClass = NSData |
| inputColorSpace |
	* CIAttributeDisplayName = Color Space;
	* CIAttributeClass = NSObject |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIAffineTransform:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Affine Transform |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryGeometryAdjustment;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAffineTransform |
| CIAttributeReferenceDocumentation | [CIAffineTransform Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAffineTransform) |
| inputTransform |
	* CIAttributeDisplayName = Transform;
	* CIAttributeDescription = A transform to apply to the image.;
	* CIAttributeIdentity = <NSAffineTransform: 0x600001786d00>;
	* CIAttributeDefault = <NSAffineTransform: 0x600001786d00>;
	* CIAttributeClass = NSAffineTransform;
	* CIAttributeType = CIAttributeTypeTransform |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPDF417BarcodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| inputDataColumns |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The number of data columns in the generated barcode;
	* CIAttributeSliderMax = 30;
	* CIAttributeDisplayName = Data Columns;
	* CIAttributeMin = 1;
	* CIAttributeMax = 30;
	* CIAttributeSliderMin = 1 |
| inputMinHeight |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The minimum height of the generated barcode in pixels.;
	* CIAttributeSliderMax = 283;
	* CIAttributeDisplayName = Min Height;
	* CIAttributeMin = 13;
	* CIAttributeMax = 283;
	* CIAttributeSliderMin = 13 |
| inputAlwaysSpecifyCompaction |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Force compaction style to @YES or @NO. Set to nil for automatic.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Always Specify Compaction;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeSliderMin = 0 |
| inputMinWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The minimum width of the generated barcode in pixels.;
	* CIAttributeSliderMax = 583;
	* CIAttributeDisplayName = Min Width;
	* CIAttributeMin = 56;
	* CIAttributeMax = 583;
	* CIAttributeSliderMin = 56 |
| inputMaxWidth |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The maximum width of the generated barcode in pixels.;
	* CIAttributeSliderMax = 583;
	* CIAttributeDisplayName = Max Width;
	* CIAttributeMin = 56;
	* CIAttributeMax = 583;
	* CIAttributeSliderMin = 56 |
| CIAttributeFilterName | CIPDF417BarcodeGenerator |
| CIAttributeFilterDisplayName | PDF417 Barcode Generator |
| inputMessage |
	* CIAttributeDescription = The message to encode in the PDF417 Barcode;
	* CIAttributeDisplayName = Message;
	* CIAttributeClass = NSData |
| inputCorrectionLevel |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The correction level ratio of the generated barcode;
	* CIAttributeSliderMax = 8;
	* CIAttributeDisplayName = Correction Level;
	* CIAttributeMin = 0;
	* CIAttributeMax = 8;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeReferenceDocumentation | [CIPDF417BarcodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPDF417BarcodeGenerator) |
| inputRows |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The number of rows in the generated barcode;
	* CIAttributeSliderMax = 90;
	* CIAttributeDisplayName = Rows;
	* CIAttributeMin = 3;
	* CIAttributeMax = 90;
	* CIAttributeSliderMin = 3 |
| inputMaxHeight |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The maximum height of the generated barcode in pixels.;
	* CIAttributeSliderMax = 283;
	* CIAttributeDisplayName = Max Height;
	* CIAttributeMin = 13;
	* CIAttributeMax = 283;
	* CIAttributeSliderMin = 13 |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| inputPreferredAspectRatio |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The preferred aspect ratio of the generated barcode;
	* CIAttributeSliderMax = 9223372036854775807;
	* CIAttributeDisplayName = Preferred Aspect Ratio;
	* CIAttributeMin = 0;
	* CIAttributeMax = 9223372036854775807;
	* CIAttributeSliderMin = 0 |
| inputCompactionMode |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The compaction mode of the generated barcode.;
	* CIAttributeSliderMax = 3;
	* CIAttributeDisplayName = Compaction Mode;
	* CIAttributeMin = 0;
	* CIAttributeMax = 3;
	* CIAttributeSliderMin = 0 |
| inputCompactStyle |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = Force a compact style Aztec code to @YES or @NO. Set to nil for automatic.;
	* CIAttributeSliderMax = 1;
	* CIAttributeDisplayName = Compact Style;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.11 |


#### CICode128BarcodeGenerator:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 8 |
| CIAttributeFilterDisplayName | Code 128 Barcode Generator |
| inputMessage |
	* CIAttributeDescription = The message to encode in the Code 128 Barcode;
	* CIAttributeDisplayName = Message;
	* CIAttributeClass = NSData |
| CIAttributeFilterCategories |
	* CICategoryGenerator;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CICode128BarcodeGenerator |
| inputQuietSpace |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The number of empty white pixels that should surround the barcode.;
	* CIAttributeDefault = 7;
	* CIAttributeDisplayName = Quiet Space;
	* CIAttributeSliderMax = 20;
	* CIAttributeMin = 0;
	* CIAttributeMax = 100;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeReferenceDocumentation | [CICode128BarcodeGenerator Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CICode128BarcodeGenerator) |
| inputBarcodeHeight |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The height of the generated barcode in pixels.;
	* CIAttributeDefault = 32;
	* CIAttributeDisplayName = Barcode Height;
	* CIAttributeSliderMax = 50;
	* CIAttributeMin = 1;
	* CIAttributeMax = 500;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 1 |
| CIAttributeFilterAvailable_Mac | 10.10 |


#### CISharpenLuminance:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Sharpen Luminance |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategorySharpen;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CISharpenLuminance |
| CIAttributeReferenceDocumentation | [CISharpenLuminance Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CISharpenLuminance) |
| inputSharpness |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of sharpening to apply. Larger values are sharper.;
	* CIAttributeDefault = 0.4;
	* CIAttributeDisplayName = Sharpness;
	* CIAttributeSliderMax = 2;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The distance from the center of the effect.;
	* CIAttributeDefault = 1.69;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 20;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIPhotoEffectTransfer:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 7 |
| CIAttributeFilterDisplayName | Photo Effect Transfer |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn;
	* CICategoryXMPSerializable |
| CIAttributeFilterName | CIPhotoEffectTransfer |
| CIAttributeReferenceDocumentation | [CIPhotoEffectTransfer Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIPhotoEffectTransfer) |
| CIAttributeFilterAvailable_Mac | 10.9 |


#### CIAreaMinMax:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 12 |
| CIAttributeFilterDisplayName | Area Min and Max |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaMinMax |
| CIAttributeReferenceDocumentation | [CIAreaMinMax Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaMinMax) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.14 |


#### CILabDeltaE:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Lab ∆E |
| inputImage2 |
	* CIAttributeDescription = The second input image for comparison.;
	* CIAttributeDisplayName = Image2;
	* CIAttributeClass = Image |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The first input image for comparison.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryColorEffect;
	* CICategoryVideo;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILabDeltaE |
| CIAttributeReferenceDocumentation | [CILabDeltaE Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILabDeltaE) |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CILightenBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Lighten Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CILightenBlendMode |
| CIAttributeReferenceDocumentation | [CILightenBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CILightenBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIMinimumCompositing:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Minimum |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryHighDynamicRange;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIMinimumCompositing |
| CIAttributeReferenceDocumentation | [CIMinimumCompositing Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIMinimumCompositing) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIVortexDistortion:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 6 |
| CIAttributeFilterDisplayName | Vortex Distortion |
| inputAngle |
	* CIAttributeDefault = 56.54866776461628;
	* CIAttributeSliderMax = 94.24777960769379;
	* CIAttributeClass = NSNumber;
	* CIAttributeDisplayName = Angle;
	* CIAttributeDescription = The angle (in radians) of the vortex.;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeAngle;
	* CIAttributeSliderMin = -94.24777960769379 |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryDistortionEffect;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIVortexDistortion |
| CIAttributeReferenceDocumentation | [CIVortexDistortion Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIVortexDistortion) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the distortion. The larger the radius, the wider the extent of the distortion.;
	* CIAttributeDefault = 300;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 800;
	* CIAttributeMin = 0;
	* CIAttributeIdentity = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputCenter |
	* CIAttributeDisplayName = Center;
	* CIAttributeDescription = The center of the effect as x and y coordinates.;
	* CIAttributeDefault = [150 150];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypePosition |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIAreaAverage:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Area Average |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to process.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryReduction;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIAreaAverage |
| CIAttributeReferenceDocumentation | [CIAreaAverage Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIAreaAverage) |
| inputExtent |
	* CIAttributeDisplayName = Extent;
	* CIAttributeDescription = A rectangle that specifies the subregion of the image that you want to process.;
	* CIAttributeDefault = [0 0 640 80];
	* CIAttributeClass = Vector;
	* CIAttributeType = CIAttributeTypeRectangle |
| CIAttributeFilterAvailable_Mac | 10.5 |


#### CIEdgeWork:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 9 |
| CIAttributeFilterDisplayName | Edge Work |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryStylize;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIEdgeWork |
| CIAttributeReferenceDocumentation | [CIEdgeWork Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEdgeWork) |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The thickness of the edges. The larger the value, the thicker the edges.;
	* CIAttributeDefault = 3;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 20;
	* CIAttributeMin = 0;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIColorBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Color Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIColorBlendMode |
| CIAttributeReferenceDocumentation | [CIColorBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIColorBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |


#### CIBokehBlur:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 11 |
| CIAttributeFilterDisplayName | Bokeh Blur |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryBlur;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIBokehBlur |
| CIAttributeReferenceDocumentation | [CIBokehBlur Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIBokehBlur) |
| inputSoftness |
	* CIAttributeDefault = 1;
	* CIAttributeClass = NSNumber;
	* CIAttributeSliderMax = 0.4;
	* CIAttributeDisplayName = Softness;
	* CIAttributeMin = 0;
	* CIAttributeMax = 10;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0.25 |
| inputRadius |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The radius determines how many pixels are used to create the blur. The larger the radius, the blurrier the result.;
	* CIAttributeDefault = 20;
	* CIAttributeDisplayName = Radius;
	* CIAttributeSliderMax = 100;
	* CIAttributeMin = 0;
	* CIAttributeMax = 500;
	* CIAttributeType = CIAttributeTypeDistance;
	* CIAttributeSliderMin = 0 |
| inputRingSize |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The size of extra emphasis at the ring of the bokeh;
	* CIAttributeDefault = 0.1;
	* CIAttributeDisplayName = Ring Size;
	* CIAttributeSliderMax = 0.2;
	* CIAttributeMin = 0;
	* CIAttributeMax = 0.2;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| inputRingAmount |
	* CIAttributeClass = NSNumber;
	* CIAttributeDescription = The amount of extra emphasis at the ring of the bokeh.;
	* CIAttributeDefault = 0;
	* CIAttributeDisplayName = Ring Amount;
	* CIAttributeSliderMax = 1;
	* CIAttributeMin = 0;
	* CIAttributeMax = 1;
	* CIAttributeType = CIAttributeTypeScalar;
	* CIAttributeSliderMin = 0 |
| CIAttributeFilterAvailable_Mac | 10.13 |


#### CIDarkenBlendMode:
| Attribute | Value |
| ---------- | --------- |
| CIAttributeFilterAvailable_iOS | 5 |
| CIAttributeFilterDisplayName | Darken Blend Mode |
| inputBackgroundImage |
	* CIAttributeDisplayName = Background Image;
	* CIAttributeDescription = The image to use as a background image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| inputImage |
	* CIAttributeDisplayName = Image;
	* CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
	* CIAttributeClass = Image;
	* CIAttributeType = CIAttributeTypeImage |
| CIAttributeFilterCategories |
	* CICategoryCompositeOperation;
	* CICategoryVideo;
	* CICategoryStillImage;
	* CICategoryInterlaced;
	* CICategoryNonSquarePixels;
	* CICategoryBuiltIn |
| CIAttributeFilterName | CIDarkenBlendMode |
| CIAttributeReferenceDocumentation | [CIDarkenBlendMode Reference](http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIDarkenBlendMode) |
| CIAttributeFilterAvailable_Mac | 10.4 |
