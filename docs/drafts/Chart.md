The Chart class offers a built-in and ready to use control to easely display graphical representation of data. Chart supports five type of graphs representation: Bar, Pie, Line, Area and Scatter.

![Chart](images/chart1.png)

### Best practices
* Item1
* Item2

### How to use
1. Drop a `Chart` control from the object panel to a `Window`
2. Use the `Chart Inspector` to customize its properties like `Type`, `Colors`, and `DataSet`

![`Chart` inspector](images/chart2.png)
The inspector where the `Chart` class can be configured.

### Example
1. Drop a `Button` control from the object panel to a `Window`
2. Open the `Code Editor` (cmd + 6)
3. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`
```
Chart1.chartType = ChartType.Area
```

### Most important properties
Several UI aspects can be configured in the `Chart` class but the `chartType` and `dataSet` are the most populars to be configured.
- `chartType`:  The graphical representation type
- `dataSet`: The `DataSet` object provides information that Chart needs to construct its content.

### References
[Chart class reference](../classes/Chart.html) contains a complete list of properties and methods that can be used to customize a `Chart` object.
