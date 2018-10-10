Represents a line (with an optional shadow).

![LineShape](images/lineshape1.png)

### Best practices
* Use the line shape control in your user interface to separates a control between different sections of the user interface.

### How to use
1. Drop a `LineShape` control from the object panel to a `Window`
2. Use the `LineShape Inspector` to customize its properties like `Line Orientation` and `Line Color`

![`LineShape` inspector](images/lineshape2.png)
The inspector where the `LineShape` class can be configured.

### Example
1. Drop a `Button` control from the object panel to a `Window`
2. Open the `Code Editor` (cmd + 6)
3. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`
```
LineShape1.isHorizontal = false
LineShape1.lineColor = Color.red
```

### Most important properties
Several UI aspects can be configured in the `LineShape` class but the `isHorizontal` and `lineColor` are the most commons to be configured.
- `isHorizontal`: Flag to set line position from horizontal to vertical.
- `lineColor`: Main line color.

### References
[LineShape class reference](../classes/LineShape.html) contains a complete list of properties and methods that can be used to customize a `LineShape` object.
