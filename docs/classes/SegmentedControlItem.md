# SegmentedControlItem

**super**: [Object](Object.md)

An SegmentedControlItem represents a segment of a SegmentedControl.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**()
This event is called when the item is selected by touching it in the SegmentedControl.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).

</ul>

### Properties

* **var** **title**: **[String](../gravity/types.md)**
The title assigned to item. An Item can only have image or title, not both.

* **var** **image**: **[Image](image.md)**
The image assigned to item. An Item can only have image or title, not both.

* **var** **width**: **[Float](../gravity/types.md)**
A float value specifying the width of the item. If the value is 0.0, SegmentedControl automatically sizes the item. Default is 0.0

* **var** **enabled**: **[Bool](../gravity/types.md)**
Use this property to enable or disable the item. By default, items are enabled.

</ul>

</ul>

