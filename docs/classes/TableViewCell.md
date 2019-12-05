**super**: **[UITableViewCell](UITableViewCell.md)** (on iOS)

This class is reserved and cannot be directly instantiated.

The TableViewCell class defines the attributes and behavior of the cells that appear in TableView controls.

### Events

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **PrepareForReuse**()
This event is invoked just before the cell is reused by a TableView. For performance reasons, you should only reset attributes of the cell that are not directly updated from the TableView's DataSet. For example, if the content of an ImageView is set with an URL you can prepare it for reuse by setting its image property to nil or to a placeholder image that will be shown until the final image is downloaded from the assigned URL.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.



### Properties

* **var** **identifier**: **[String](../gravity/string.md)**
Identifier set in the cell property inspector.

* **var** **text**: **[String](../gravity/string.md)**
The main textual content.

* **var** **detailText**: **[String](../gravity/string.md)**
The text of the secondary label of the cell.

* **var** **image**: **[Image](Image.md)**
The image of the cell.

* **var** **customView**: **[CustomView](CustomView.md)**
Custom view instance presented in the contentView of the cell.

* **var** **rightActions**: **[List](../gravity/list.md)**
Array of swipe actions to display on the right edge of the row

* **var** **leftActions**: **[List](../gravity/list.md)**
Array of swipe actions to display on the left edge of the row

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.





