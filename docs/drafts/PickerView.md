A picker includes one or more scrollable lists of distinct values, each of which has a single selected value—appearing in darker text in the center of the view. A picker is often displayed at the bottom of the screen or in a popover when the user is editing a field or tapping a menu. Pickers can also appear inline, such as while editing a date in a Calendar event. The height of a picker is roughly the height of five rows of list values. The width of a picker is either the width of the screen or its enclosing view, depending on the device and context.

![PickerView](images/pickerview1.png)

### Best practices
* **Use predictable and logically ordered values.** Many values in a picker may be hidden when the scrollable lists are stationary. It's best when people can predict what these values are, such as with a list of alphabetized countries, so they can move through the lists quickly.
* **Avoid switching screens to show a picker.** A picker works well when displayed in context, below or in close proximity to the field being edited.
* **Use a table instead of a picker for large value lists.** Long lists can be tedious to navigate in a picker. A table has adjustable height and can include an index, making scrolling much faster.

### How to use
1. Drop a `PickerView` control from the object panel to a `Window`
2. Use the `PickerView Inspector` to customize its properties like `Size`, `DataSet`, and `KeyPath`

If you need to write code for PickerView:

3. Open the `Code Editor` (cmd + 6)
4. Select the `DidSelectCell` item inside the `Events` area and write your custom code in the `Code Editor`

![`PickerView` inspector](images/pickerview2.png)
The inspector where the `PickerView` class can be configured.

### Example
1. Open the `Code Editor` (cmd + 6)
2. Select the `Changed` item inside the `Events` area and write your custom code in the `Code Editor`
```
Console.write("PickerView Column: \(column) Row: \(row)")
```

### Most important properties
Several UI aspects can be configured in the `PickerView` class but the `dataSet` is the most popular to be configured.
- `dataSet`: The dataset object provides information that PickerView needs to construct its content.

### References
[PickerView class reference](../classes/PickerView.html) contains a complete list of properties and methods that can be used to customize a `PickerView` object.
