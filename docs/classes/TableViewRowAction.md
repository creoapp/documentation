**super**: **[Object](Object.md)**

A single action to present when the user swipes horizontally in a table row.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Action**(**cell**: **[TableViewCell](TableViewCell.md)**, **section**: **[Int](../gravity/types.md)**, **index**: **[Int](../gravity/types.md)**)
This event is called in response to the selection of the row action

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **style**: **TableViewRowActionStyle**
Destructive (default) or normal style. \(read-only\)

* **var** **title**: **[String](../gravity/types.md)**
Title of the button.

* **var** **image**: **[Image](Image.md)**
The image to display in the button. Only available on iOS 11.0+

* **var** **backgroundColor**: **[Color](Color.md)**
The background color for the action button. The default color depends on the style.



### Initializers

* **func** **TableViewRowAction**(**style**: **<a href="#_enum_TableViewRowActionStyle">TableViewRowActionStyle</a>**, **title**: **[String](../gravity/types.md)**)
Create a new TableViewRowAction object.





### Enumeration

#### TableViewRowActionStyle
 * .Default
 * .Destructive
 * .Normal



