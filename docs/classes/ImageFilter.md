**super**: **[Object](Object.md)**

An image processor that produces an image by manipulating one or more input images or by generating new image data.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Properties

* **var** **categories**: **[List](../gravity/list.md)**
List of available categories.



### Properties

* **var** **inputKeys**: **[List](../gravity/list.md)**
Returns a list containing the names of all inputs in the filter \(read-only\)

* **var** **outputKeys**: **[List](../gravity/list.md)**
Returns a list containing the names of all outputs in the filter. \(read-only\)

* **var** **attributes**: **[Map](../gravity/map.md)**
Returns a map containing key/value pairs describing the filter. This map contains two kinds of key-value pairs:<ul><li>Keys like 'CIAttributeFilterName', 'CIAttributeFilterDisplayName', 'CIAttributeDescription', 'CIAttributeReferenceDocumentation', 'CIAttributeFilterCategories' describe the filter, providing information such as a human-readable name and categories you can use to organize filters in your app’s UI.</li><li>Other keys starting with “input” or “output”, one for each value in inputKeys and outputKeys properties, describe parameters that control the filter’s behavior. For each parameter key, the corresponding value is another dictionary describing possible values for that parameter, such as the value type, class and minimum/maximum values. You can use this information to build a UI to control the filter.</li></ul> \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **filterWithName**(**name**: **[String](../gravity/string.md)**): <strong>[ImageFilter](ImageFilter.md)</strong> 
Creates a new filter of type 'name', all input values will be set to default values.

* **func** **filterNamesInCategory**(**category**: **[String](../gravity/string.md)**): <strong>[List](../gravity/list.md)</strong> 
Returns an array containing all published filter names in a category.

* **func** **localizedDescriptionForFilterName**(**name**: **[String](../gravity/string.md)**): <strong>[String](../gravity/string.md)</strong> 
Returns the localized description of a filter for display in the UI.



### Methods

* **func** **setDefaults**()
Sets all inputs to their default values (where default values are defined, other inputs are left as-is).

* **func** **getValue**(**key**: **[String](../gravity/string.md)**): <strong>[Object](../gravity/object.md)</strong> 
Get the current value for the property specified by the key. Valid values for the key parameters are listed in the inputKeys and outputKeys properties.

* **func** **setValue**(**value**: **[Object](../gravity/object.md)**, **key**: **[String](../gravity/string.md)**)
Set a new value for the property specified by the key. Valid values for the key parameters are listed in the inputKeys properties.

* **func** **outputImage**(**outputImageClosure**: **[Closure](../gravity/closure.md) = null**, **rectToRender**: **[Rect](Rect.md) = null**, **scale**: **[Float](../gravity/float.md) = 1**, **orientation**: **<a href="#_enum_ImageOrientation">ImageOrientation</a> = 0**): <strong><a href="#_enum_ImageOrientation">ImageOrientation</a></strong> 
Executes the filter and produces the rendered image. If the closure parameter is set the execution is performed in a background thread so the UI stays responsive, the methods immediately returns with null value and, when the image is ready, it is passed as the only parameter of the closure; otherwise, the execution is performed in the main thread and the methods returns the resulting image. The optional rectToRender parameter defines the region of the image to render. If not set, the extent of the filtered image is used instead and the image is completely rendered (if the extent of the image is infinite, the rect is too big to be rendered so the resulting image is NULL).





### Enums

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



