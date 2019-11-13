**super**: **[Object](../gravity/object.md)**

The OSSharing class provides support for printing and sharing content from your app.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Properties

* **var** **isPrintingAvailable**: **[Bool](../gravity/bool.md)**
Returns a Boolean indicating whether the device supports printing.



### Properties

* **var** **items**: **[List](../gravity/list.md)**
The array of data objects on which to perform the activity. The type of objects in the array is variable and dependent on the data your application manages. For example, the data might consist of one or more string or image objects representing the currently selected content.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **shareImage**(**image**: **[Image](Image.md)**)
Share image with others apps.

* **func** **shareData**(**data**: **[Data](Data.md)**)
Share raw data with others apps.

* **func** **shareString**(**string**: **[String](../gravity/string.md)**)
Share a string with others apps.

* **func** **shareURL**(**string**: **[String](../gravity/string.md)**)
Share URL with others apps.





### Methods

* **func** **show**()
Display sharing dialog to the user.

* **func** **addExcludedType**(**options**: **[Int](../gravity/int.md)**)
Add a service that you do not want displayed to the user. You might exclude services that you feel are not suitable for the content you are providing. For example, you might not want to allow the user to print a specific image. If the value of this property is nil, no services are excluded.

* **func** **printImage**(**image**: **[Image](Image.md)**)
Presents the printing user interface in a sheet to print an image.

* **func** **printText**(**text**: **[String](../gravity/string.md)**)
Presents the printing user interface in a sheet to print a String.

* **func** **printMarkupText**(**text**: **[String](../gravity/string.md)**)
Presents the printing user interface in a sheet to print a Markup String.

* **func** **printData**(**data**: **[Data](Data.md)**)
Presents the printing user interface in a sheet to print Data.

* **func** **printItem**(**item**: **[Object](../gravity/object.md)**)
Presents the printing user interface in a sheet to print an item (can be an URL, a path, a TextView, a MapView or a WebView.

* **func** **printFile**(**path**: **[String](../gravity/string.md)**)
Presents the printing user interface in a sheet to print a file.

* **func** **printItems**(**items**: **[List](../gravity/list.md)**)
Presents the printing user interface in a sheet to print a List of items (usually a sequence of Images).





