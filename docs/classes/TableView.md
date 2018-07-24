**super**: [UITableView](UITableView.md) on iOS

A TableView displays a list of items in a single column. The TableView uses a TableViewCell template to draw the visible rows of the table. The values for the cells are obtained with the DataSet approach; you can use the built-in data grid (to edit the data grid, double click on the TableView from the design board) or use another object that inherit from the <a href="DataSet.html">DataSet</a> (recordsets from a databases, sensors, network datasources, etc).

#### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **RowHeight**(**section**: <strong>[Int](../gravity/types.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>): <strong>[Float](../gravity/types.md)</strong> 
This event lets you specify a different height depending of the section and row indexes. If this event is implemented, the return value of this event is used to define the height of the specified row instead of the <code>rowHeight</code> property of the TableView.

* **DidSelectCell**(**cell**: <strong>[TableViewCell](TableViewCell.md)</strong>, **section**: <strong>[Int](../gravity/types.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>)
This event is called when a row is selected. The parameters contain the instance of the <a href="TableViewCell.html">TableViewCell</a>, the section index and the row index of the selected cell.

* **DidDeselectCell**(**cell**: <strong>[TableViewCell](TableViewCell.md)</strong>, **section**: <strong>[Int](../gravity/types.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>)
This event is called when a row is deselected. The parameters contain the instance of the <a href="TableViewCell.html">TableViewCell</a>, the section index and the row index of the deselected cell.

* **CanEditCell**(**cell**: <strong>[TableViewCell](TableViewCell.md)</strong>, **section**: <strong>[Int](../gravity/types.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
The event allows you to exclude individual rows from being treated as editable. Editable rows display the insertion or deletion control in their cells. If this event is not implemented, all rows are assumed to be editable. Return true if you want the cell to be editable, false otherwise.

* **CommitEdit**(**cell**: <strong>[TableViewCell](TableViewCell.md)</strong>, **section**: <strong>[Int](../gravity/types.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>, **editingMode**: <strong><a href="#_enum_TableViewCellEditingStyle">TableViewCellEditingStyle</a></strong>): <strong>[Bool](../gravity/types.md)</strong> 
This event is called when users tap the insertion (green plus) control of an editing row or the Delete confirmation button after a left swipe gesture or after pressing the Delete (red minus) button of an editing row. This event lets you commit the change. If the event returns true, the TableView assumes that the DataSet has been updated and proceeds to insert/remove the row depending on the <code>editingMode</code> otherwise, if it returns false, the TableView just dismiss the presented action.

* **WillReload**()
This event is called when the table and its dataSet are about to be reloaded because of the user did perform the pull-to-reload gesture. Only applies if the reloadOnPull property is true.

* **DidReload**()
This event is called when the dataSet of the table completes a reload.

* **DidScroll**()
This event is called when the user scrolls the content view.

* **DidEndDragging**(**decelerate**: <strong>[Bool](../gravity/types.md)</strong>)
This event is called when dragging ended in the scroll view. The scroll view sends this event when the user’s finger touches up after dragging content. The decelerating property of the scroll view controls deceleration. The decelerate value is true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is NO, scrolling stops immediately upon touch-up.

* **DidEndDecelerating**()
This event is called when the scroll view ends decelerating the scrolling movement.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



#### Properties

* **var** **style**: **TableViewStyle**
Returns the style of the table view. \(read-only\)

* **var** **rowHeight**: **[Float](../gravity/types.md)**
The height of each row.

* **var** **separatorStyle**: **TableViewCellSeparatorStyle**
The style for table cells used as separators. By default it uses a single line running across its width.

* **var** **separatorColor**: **[Color](color.md)**
The color of separator rows in the table view.

* **var** **sectionHeaderHeight**: **[Float](../gravity/types.md)**
The height of section headers in the table view.

* **var** **sectionFooterHeight**: **[Float](../gravity/types.md)**
The height of section footers in the table view.

* **var** **editing**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether the table view is in editing mode.

* **var** **allowsSelection**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether users can select a row.

* **var** **allowsSelectionDuringEditing**: **[Bool](../gravity/types.md)**
A Boolean value that determines whether users can select cells while the table view is in editing mode.

* **var** **allowsMultipleSelection**: **[Bool](../gravity/types.md)**
A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

* **var** **allowsMultipleSelectionDuringEditing**: **[Bool](../gravity/types.md)**
Description not yet ready.

* **var** **reloadOnPull**: **[Bool](../gravity/types.md)**
A Boolean value that controls whether the dataSet and the table must be reloaded when the user drags the table over the top.

* **var** **pullTitle**: **[String](../gravity/types.md)**
The text to display in the refresh control.

* **var** **pullColor**: **[Color](color.md)**
The tint color for the title and the activity indicator of the refresh control. If nil, the title and the activity indicator will use their default color.

* **var** **selectedRow**: **[IndexPath](IndexPath.md)**
Returns an index path identifying the row and section at the given point. \(read-only\)

* **var** **selectedRows**: **[List](../gravity/lists.md)**
The index paths of the selected rows. \(read-only\)

* **var** **keyPath**: **[String](../gravity/types.md)**
The base keyPath to get a particular node of the <a href="DataSet.html">DataSet</a> value. The DataSet must provide a List of objects and each object represents a different row. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath defines the list of keys used to browse the data tree to get a List node. The values for each exposed property of the cell are retrieved by adding the current index and the cell property key to the base keyPath.



#### Methods

* **func** **reload**(**reloadDataSet**: <strong>[Bool](../gravity/types.md) = true</strong>, **keepSelection**: <strong>[Bool](../gravity/types.md) = true</strong>)
Reloads the content of the table view.

* **func** **setEditing**(**editing**: <strong>[Bool](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
When you call this method with the value of editing set to true, the table view goes into editing mode by calling on each visible row. Calling this method with editing set to false turns off editing mode. In editing mode, the cells of the table might show an insertion or deletion control on the left side of each cell and a reordering control on the right side, depending on how the cell is configured. You can selectively exclude cells from editing mode by implementing the CanEditItem event.

* **func** **numberOfRows**(**section**: <strong>[Int](../gravity/types.md)</strong>): <strong>[Int](../gravity/types.md)</strong> 
Returns the number of rows in a specified section.

* **func** **numberOfSections**(): <strong>[Int](../gravity/types.md)</strong> 
The number of sections in the table view.

* **func** **indexPathForRowAtPoint**(**point**: <strong>[Point](point.md)</strong>): <strong>[IndexPath](IndexPath.md)</strong> 
Returns an index path identifying the row and section at the given point.

* **func** **selectRow**(**indexPath**: <strong>[IndexPath](IndexPath.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>, **scrollPosition**: <strong><a href="#_enum_TableViewScrollPosition">TableViewScrollPosition</a> = 0</strong>)
Selects a row in the table view identified by index path, optionally scrolling the row to a location in the table view. The scrollPosition is a constant that identifies a relative position in the table view (top, middle, bottom) for the row when scrolling concludes. See TableViewScrollPosition for descriptions of valid constants.

* **func** **deselectRow**(**indexPath**: <strong>[IndexPath](IndexPath.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
Deselects a given row identified by index path, with an option to animate the deselection.

* **func** **scrollToRow**(**indexPath**: <strong>[IndexPath](IndexPath.md)</strong>, **scrollPosition**: <strong><a href="#_enum_TableViewScrollPosition">TableViewScrollPosition</a> = 0</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
Scrolls through the table view until a row identified by index path is at a particular location on the screen.

* **func** **deleteRows**(**indexPaths**: <strong>[List](../gravity/lists.md)</strong>, **rowAnimation**: <strong><a href="#_enum_TableViewRowAnimation">TableViewRowAnimation</a> = 100</strong>)
Deletes the rows specified by an array of index paths, with an option to animate the deletion (the animation is not simulated in the Creo Simulator for Mac).

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





#### Enumeration

#### TableViewCellEditingStyle
 * .Delete
 * .Insert
 * .None

<br><br>#### TableViewStyle
 * .Grouped
 * .Plain

<br><br>#### TableViewCellSeparatorStyle
 * .None
 * .SingleLine

<br><br>#### TableViewScrollPosition
 * .Bottom
 * .Middle
 * .None
 * .Top

<br><br>#### TableViewRowAnimation
 * .Automatic
 * .Bottom
 * .Fade
 * .Left
 * .Middle
 * .None
 * .Right
 * .Top

<br><br>#### AnimationOption
 * .AllowAnimatedContent
 * .AllowUserInteraction
 * .Autoreverse
 * .BeginFromCurrentState
 * .CurveEaseIn
 * .CurveEaseInOut
 * .CurveEaseOut
 * .CurveLinear
 * .LayoutSubviews
 * .OverrideInheritedCurve
 * .OverrideInheritedDuration
 * .OverrideInheritedOptions
 * .Repeat
 * .ShowHideTransitionViews
 * .TransitionCrossDissolve
 * .TransitionCurlDown
 * .TransitionCurlUp
 * .TransitionFlipFromBottom
 * .TransitionFlipFromLeft
 * .TransitionFlipFromRight
 * .TransitionFlipFromTop
 * .TransitionNone

<br><br>

