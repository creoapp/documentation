For more information: [Core Image Filter Reference](https://developer.apple.com/library/archive/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html)

#### CIEdges:
* **CIAttributeFilterAvailable_iOS**: 9
* **CIAttributeFilterDisplayName**: Edges
* **inputImage**:
    * CIAttributeDisplayName = Image;
    * CIAttributeDescription = The image to use as an input image. For filters that also use a background image, this is the foreground image.;
    * CIAttributeClass = CIImage;
    * CIAttributeType = CIAttributeTypeImage
* **CIAttributeFilterCategories**:
    * CICategoryStylize;
    * CICategoryVideo;
    * CICategoryStillImage;
    * CICategoryBuiltIn;
* **CIAttributeFilterName**: CIEdges
* **CIAttributeReferenceDocumentation**: http://developer.apple.com/library/mac/documentation/GraphicsImaging/Reference/CoreImageFilterReference/index.html#//apple_ref/doc/filter/ci/CIEdges
* **inputIntensity**:
    * CIAttributeDefault = 1;
    * CIAttributeSliderMax = 10;
    * CIAttributeClass = NSNumber;
    * CIAttributeDisplayName = Intensity;
    * CIAttributeDescription = The intensity of the edges. The larger the value, the higher the intensity.;
    * CIAttributeMin = 0;
    * CIAttributeIdentity = 0;
    * CIAttributeType = CIAttributeTypeScalar;
    * CIAttributeSliderMin = 0
* **CIAttributeFilterAvailable_Mac**: 10.4
