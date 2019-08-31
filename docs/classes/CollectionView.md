**super**: **[UICollectionView](UICollectionView.md)** (on iOS)

The CollectionView class manages an ordered collection of data items and presents them using customizable layouts. Collection views provide the same general function as <a href="TableView.html">TableView(s)</a> except that a collection view is able to support more than just single-column layouts. The collection view presents items onscreen using the built-in cell or a user-defined <a href="CustomView.html">CustomView</a>.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **CellSize**(**section**: **[Int](../gravity/int.md)**, **index**: **[Int](../gravity/int.md)**): <strong>[Size](Size.md)</strong> 
This event asks for the size of the specified item’s cell. If you do not implement this method, the collection view uses the values in its itemSize property to set the size of items instead. Your implementation of this method can return a fixed set of sizes or dynamically adjust the sizes based on the cell’s content. Only applies to the normal flow layout type.

* **DidSelectCell**(**cell**: **[CollectionViewCell](CollectionViewCell.md)**, **section**: **[Int](../gravity/int.md)**, **index**: **[Int](../gravity/int.md)**)
This event is called when the specified cell is selected.

* **DidDeselectCell**(**cell**: **[CollectionViewCell](CollectionViewCell.md)**, **section**: **[Int](../gravity/int.md)**, **index**: **[Int](../gravity/int.md)**)
This event is called when the specified cell is deselected.

* **ShouldShowMenu**(**section**: **[Int](../gravity/int.md)**, **index**: **[Int](../gravity/int.md)**)
Asks if an action menu should be displayed for the specified item. This event is not called in the Creo simulator for Mac.

* **CanPerformAction**(**action**: **[String](../gravity/string.md)**, **section**: **[Int](../gravity/int.md)**, **index**: **[Int](../gravity/int.md)**)
Asks if it can perform the specified action on an item in the collection view. This method is invoked after the ShouldShowMenu event. It gives you the opportunity to exclude commands from the editing menu. For example, the user might have copied some content from one item and wants to paste it into another item that cannot accept the content. In such a case, your method could return false to prevent the display of the relevant command. The default actions are <code>cut:</code>, <code>copy:</code> and <code>paste:</code>. This event is not called in the CREO simulator for Mac.

* **PerformAction**(**action**: **[String](../gravity/string.md)**, **section**: **[Int](../gravity/int.md)**, **index**: **[Int](../gravity/int.md)**)
This event lets you perform the specified action on an item in the collection view. This event is not called in the Creo simulator for Mac.

* **DidScroll**()
This event is called when the user scrolls the content view.

* **DidEndDragging**(**decelerate**: **[Bool](../gravity/bool.md)**)
This event is called when dragging ended in the scroll view. The scroll view sends this event when the user’s finger touches up after dragging content. The decelerating property of the scroll view controls deceleration. The decelerate value is true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is NO, scrolling stops immediately upon touch-up.

* **DidEndDecelerating**()
This event is called when the scroll view ends decelerating the scrolling movement.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **layoutType**: **CollectionViewLayoutType**
The layout defines the organization and location of all cells and supplementary views inside the collection view. The layout type property allows you to choose between two mail styles (the simple flow and the balanced flow) while other layout properties (minimumLineSpacing, preferredRowSize, etc.) enable you to configure some details of the choosen layout style.
With the simple flow the items in the collection view flow from one row or column (depending on the scrolling direction) to the next, with each row comprising as many cells as will fit.  Cells can be the same sizes or different sizes (see the ItemSize event).
With the balanced flow, the collection view displays items of different sizes in a grid without wasting any visual space.

* **var** **minimumInteritemSpacing**: **[Float](../gravity/float.md)**
The minimum spacing to use between items in the same row. For a vertically scrolling grid, this value represents the minimum spacing between items in the same row. For a horizontally scrolling grid, this value represents the minimum spacing between items in the same column. This spacing is used to compute how many items can fit in a single line, but after the number of items is determined, the actual spacing may possibly be adjusted upward.

* **var** **minimumLineSpacing**: **[Float](../gravity/float.md)**
The minimum spacing to use between lines of items in the grid. For a vertically scrolling grid, this value represents the minimum spacing between successive rows. For a horizontally scrolling grid, this value represents the minimum spacing between successive columns. This spacing is not applied to the space between the header and the first line or between the last line and the footer.

* **var** **preferredRowSize**: **[Float](../gravity/float.md)**
The preferred size for each row measured in the scroll direction. Only applies to the balanced flow layout type.

* **var** **itemSize**: **[Size](Size.md)**
The default size to use for cells. This results in cells that all have the same size. The default size value is (50.0, 50.0). Only applies to the simple flow layout type.

* **var** **scrollDirection**: **CollectionViewScrollDirection**
The scroll direction of the grid. The grid layout scrolls along one axis only, either horizontally or vertically. For the non scrolling axis, the width of the collection view in that dimension serves as starting width of the content. The default value is CollectionViewScrollDirection.Vertical.

* **var** **allowsSelection**: **[Bool](../gravity/bool.md)**
A Boolean value that indicates whether users can select items in the collection view. The default value is true.

* **var** **allowsMultipleSelection**: **[Bool](../gravity/bool.md)**
A Boolean value that determines whether users can select more than one item in the collection view. The default value is false.

* **var** **selectedItems**: **[List](../gravity/list.md)**
Returns nil or an array of selected index paths. \(read-only\)

* **var** **dataSet**: **[Object](../gravity/object.md)**
The <a href="DataSet.html">DataSet</a> object provides information that CollectionView needs to construct its content. The dataSet must return a List of objects and each object represents a different row. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath property defines the list of keys used to browse the data tree to get a List node.

* **var** **keyPath**: **[String](../gravity/string.md)**
The base keyPath to get a particular node of the <a href="DataSet.html">DataSet</a> value. The DataSet must provide a List of objects and each object represents a different item. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath defines the list of keys used to browse the data tree to get a List node. The values for each exposed property of the cell are retrieved by adding the current index and the cell property key to the base keyPath.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **reload**(**reloadDataSet**: **[Bool](../gravity/bool.md) = true**)
Reloads the content of the collection view.

* **func** **numberOfSections**(): <strong>[Int](../gravity/int.md)</strong> 
Returns the number of sections displayed by the collection view.

* **func** **numberOfItemsInSection**(**section**: **[Int](../gravity/int.md)**): <strong>[Int](../gravity/int.md)</strong> 
Returns the number of items in the specified section.

* **func** **selectItem**(**indexPath**: **[IndexPath](IndexPath.md)**, **animated**: **[Bool](../gravity/bool.md) = true**, **scrollPosition**: **<a href="#_enum_CollectionViewScrollPosition">CollectionViewScrollPosition</a> = 0**)
Selects the item at the specified index path and optionally scrolls it into view.

* **func** **deselectItem**(**indexPath**: **[IndexPath](IndexPath.md)**, **animated**: **[Bool](../gravity/bool.md) = true**)
Deselects the item at the specified index.

* **func** **indexPathForItemAtPoint**(**point**: **[Point](Point.md)**): <strong>[IndexPath](IndexPath.md)</strong> 
Returns the index path of the item at the specified point in the collection view.

* **func** **indexPathsForVisibleItems**(): <strong>[List](../gravity/list.md)</strong> 
An array of the index paths of the visible items in the collection view.

* **func** **indexPathForCell**(**cell**: **[CollectionViewCell](CollectionViewCell.md)**): <strong>[IndexPath](IndexPath.md)</strong> 
Returns the index path of the specified cell.

* **func** **cellForItemAtIndexPath**(**indexPath**: **[IndexPath](IndexPath.md)**): <strong>[CollectionViewCell](CollectionViewCell.md)</strong> 
Returns the visible cell object at the specified index path.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_CollectionViewLayoutType"></div>

#### CollectionViewLayoutType
 * .BalancedFlow
 * .Flow

<div id="_enum_CollectionViewScrollDirection"></div>

#### CollectionViewScrollDirection
 * .Horizontal
 * .Vertical

<div id="_enum_CollectionViewScrollPosition"></div>

#### CollectionViewScrollPosition
 * .Bottom
 * .CenteredHorizontally
 * .CenteredVertically
 * .Left
 * .None
 * .Right
 * .Top

<div id="_enum_AnimationOption"></div>

#### AnimationOption
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



