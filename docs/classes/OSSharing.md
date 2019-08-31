**super**: **[Object](../gravity/object.md)**

The OSSharing class provides support for sharing content from your app.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



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





