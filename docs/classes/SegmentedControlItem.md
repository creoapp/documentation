**super**: **[Object](Object.md)**

An SegmentedControlItem represents a segment of a SegmentedControl.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called when the item is selected by touching it in the SegmentedControl.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **title**: **[String](../gravity/string.md)**
The title assigned to item. An Item can only have image or title, not both.

* **var** **image**: **[Image](Image.md)**
The image assigned to item. An Item can only have image or title, not both.

* **var** **width**: **[Float](../gravity/float.md)**
A float value specifying the width of the item. If the value is 0.0, SegmentedControl automatically sizes the item. Default is 0.0

* **var** **enabled**: **[Bool](../gravity/bool.md)**
Use this property to enable or disable the item. By default, items are enabled.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



* None

