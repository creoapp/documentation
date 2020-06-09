**super**: **[Object](../gravity/object.md)**

A Movie object from the Asset. It can be played by a MoviePlayer.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **path**: **[String](../gravity/string.md)**
The URL of the movie file

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Class Methods

* **func** **createMP4**(**array**: **[List](../gravity/list.md)**, **outputFile**: **[String](../gravity/string.md)**, **fps**: **[Int](../gravity/int.md) = 24**, **completion**: **[Closure](../gravity/closure.md)**)
Create an MP4 movie.

* **func** **createGIF**(**array**: **[List](../gravity/list.md)**, **outputFile**: **[String](../gravity/string.md)**, **repeats**: **[Int](../gravity/int.md) = 0**, **delay**: **[Float](../gravity/float.md) = 0.02**, **completion**: **[Closure](../gravity/closure.md)**)
Create a GIF file.





