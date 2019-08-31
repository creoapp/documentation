**super**: **[Object](../gravity/object.md.md)**

A single action to present when the user swipes horizontally in a table row.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**(**cell**: **[TableViewCell](TableViewCell.md)**, **section**: **[Int](../gravity/int.md)**, **index**: **[Int](../gravity/int.md)**)
This event is called in response to the selection of the row action

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **style**: **TableViewRowActionStyle**
Destructive (default) or normal style. \(read-only\)

* **var** **title**: **[String](../gravity/string.md)**
Title of the button.

* **var** **image**: **[Image](Image.md)**
The image to display in the button. Only available on iOS 11.0+

* **var** **backgroundColor**: **[Color](Color.md)**
The background color for the action button. The default color depends on the style.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Initializers

* **func** **TableViewRowAction**(**style**: **<a href="#_enum_TableViewRowActionStyle">TableViewRowActionStyle</a>**, **title**: **[String](../gravity/string.md)**)
Create a new TableViewRowAction object.





### Enums

<div id="_enum_TableViewRowActionStyle"></div>

#### TableViewRowActionStyle
 * .Default
 * .Destructive
 * .Normal



