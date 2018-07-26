**super**: **[UIPickerView](UIPickerView.md)** (on iOS)

The PickerView class implements objects, called picker views, that use a spinning-wheel or slot-machine metaphor to show one or more sets of values. Users select values by rotating the wheels so that the desired row of values aligns with a selection indicator. The user interface provided by a picker view consists of components and rows. A component is a wheel, which has a series of items (rows) at indexed locations on the wheel. Each component also has an indexed location (left to right) in a picker view. Each row on a component has content, which is either a string or a view object such as a label (<a href="Label.html">Label</a>) or an image (<a href="ImageView.html">ImageView</a>)).

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidSelectCell**(**column**: **[Int](../gravity/types.md)**, **row**: **[Int](../gravity/types.md)**)
This event is called by the picker view when the user selects a row in a column.

* **RowHeight**(**column**: **[Int](../gravity/types.md)**): <strong>[Float](../gravity/types.md)</strong> 
This event is called by the picker view when it needs the row height to use for drawing row content in the specified column.

* **ColumnWidth**(**column**: **[Int](../gravity/types.md)**): <strong>[Float](../gravity/types.md)</strong> 
This event is called by the picker view when it needs the column width.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **pickerSize**: **PickerViewSize**
Description not yet ready.

* **var** **showsSelectionIndicator**: **[Bool](../gravity/types.md)**
Description not yet ready.

* **var** **numberOfComponents**: **[Int](../gravity/types.md)**
Description not yet ready. \(read-only\)



### Methods

* **func** **reload**(**reloadDataSet**: **[Bool](../gravity/types.md)**)
Reloads all components of the picker view.

* **func** **reloadComponent**(**identifier**: **[Int](../gravity/types.md)**)
Reloads a particular component of the picker view. Calling this method causes the picker view to query the delegate for new data for the given component.

* **func** **numberOfRowsInComponent**(**identifier**: **[Int](../gravity/types.md)**): <strong>[Int](../gravity/types.md)</strong> 
Returns the number of rows for a component. A picker view fetches the value of this property from the data source and and caches it. The default value is zero.

* **func** **selectRowInComponent**(**row**: **[Int](../gravity/types.md)**, **identifier**: **[Int](../gravity/types.md)**, **animated**: **[Bool](../gravity/types.md)**)
Selects a row in a specified component of the picker view.

* **func** **selectedRowInComponent**(**identifier**: **[Int](../gravity/types.md)**): <strong>[Int](../gravity/types.md)</strong> 
Returns the index of the selected row in a given component. A zero-indexed number identifying the selected row, or -1 if no row is selected.

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### PickerViewSize
 * .Default
 * .Mini
 * .Small

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



