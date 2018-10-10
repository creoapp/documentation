Represents a rectangle shape (with optional rounded corners).

![RectShape](images/rectshape1.png)

### How to use
1. Drop a `RectShape` control from the object panel to a `Window`
2. Use the `RectShape Inspector` to customize its properties like `Fill Color`, `Thickness`, `Radius`, and `Border Color`

![`RectShape` inspector](images/rectshape2.png)
The inspector where the `RectShape` class can be configured.

### Example
1. Drop a `Button` control from the object panel to a `Window`
2. Open the `Code Editor` (cmd + 6)
3. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`
```
RectShape1.fillColor = Color.red
RectShape1.borderColor = Color.black
RectShape1.borderWidth = 4
```

### Most important properties
Several UI aspects can be configured in the `RectShape` class but the `radius`, `fillColor`, `borderColor`  and `borderWidth` are the most commons to be configured.
- `radius`: Radius value in case of rounded rect.
- `fillColor`: Color used to fill the shape.
- `borderColor`: The color of the view’s border.
- `borderWidth`: The width of the view's border. When this value is greater than 0.0, the layer draws a border using the current borderColor value. The border is drawn inset from the receiver’s bounds by the value specified in this property. It is composited above the receiver’s contents and sublayers and includes the effects of the cornerRadius property.

### References
[RectShape class reference](../classes/RectShape.html) contains a complete list of properties and methods that can be used to customize a `RectShape` object.
