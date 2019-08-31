**super**: **[BaseDataSet](BaseDataSet.md)**

A CameraRoll class manages system-supplied user interfaces for choosing saved images and movies for use in your app. A CameraRoll object can be used as DataSet in all the controls that accept a DataSet.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **NewImage**(**image**: **[Image](Image.md)**)
Event raised when a new Image is available from the CameraRoll.

* **NewVideo**(**videoPath**: **[String](../gravity/string.md)**)
Event raised when a new Video is available from the CameraRoll.

* **DidCancel**()
Event raised when last operation has been cancelled from the user.

* **SavedImage**(**image**: **[Image](Image.md)**, **error**: **[String](../gravity/string.md)**, **localIdentifier**: **[Object](../gravity/object.md)**)
Event raised when an Image has been saved to the CameraRoll.

* **SavedVideo**(**videoPath**: **[String](../gravity/string.md)**, **error**: **[String](../gravity/string.md)**)
Event raised when a Video has been saved to the CameraRoll.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: **[Object](../gravity/object.md)**)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Methods

* **func** **saveImage**(**image**: **[Image](Image.md)**, **metadata**: **[Map](../gravity/map.md) = null**)
Save an Image to the CameraRoll.

* **func** **saveVideo**(**videoPath**: **[String](../gravity/string.md)**)
Save a Video to the CameraRoll.



### Methods

* **func** **open**()
Open CameraRoll and let the user choose saved images and movies for use in your app.

* **func** **saveImage**(**image**: **[Image](Image.md)**, **metadata**: **[Map](../gravity/map.md) = null**)
Save an Image to the CameraRoll.

* **func** **saveVideo**(**videoPath**: **[String](../gravity/string.md)**)
Save a Video to the CameraRoll.

* **func** **openAsset**(**index**: **[Int](../gravity/int.md)**)
Open the asset at the specified index from the DataSet. The chosen image or video will be returned asynchronously with the NewImage or NewVideo event.

* **func** **openAssetResized**(**index**: **[Int](../gravity/int.md)**, **imageSize**: **[Size](Size.md)**, **CameraRollContentMode**: **[Int](../gravity/int.md)**)
Open the asset at the specified index from the DataSet. The chosen image or video will be returned asynchronously with the NewImage (scaled with the specified size and content mode) or NewVideo event.



* None

