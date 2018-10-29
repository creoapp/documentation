A switch is a visual toggle between two mutually exclusive states—on and off.

![Toggle](../images/creo/toggle1.png)

### Best practices
* **Consider adjusting a switch’s appearance to match the style of your app.** If it works well in your app, change the colors of a switch in its on and off states or use custom imagery to represent the switch.
* **Use switches in table rows only.** Switches are intended for use in tables, such as in a list of settings that can be toggled on and off. If you need similar functionality in a toolbar or navigation bar, use a button instead, and provide two distinct icons that communicate the states.
* **Avoid adding labels to describe the values of a switch.** Switches are either on or off. Providing labels that describe these states is redundant and clutters the interface.
* **Consider using switches to manage the availability of related interface elements.** Switches often affect other content onscreen. Enabling the Airplane Mode switch in Settings, for example, disables certain other settings, such as Cellular and Personal Hotspot. Disabling the Wi-Fi switch in Settings > Wi-Fi causes available networks and other options to disappear.

### How to use
1. Drop a `Toggle` control from the object panel to a `Window`
2. Use the `Toggle Inspector` to customize its properties like `selected`

If you need to write code for Toggle:

3. Open the `Code Editor` (cmd + 6)
4. Select the `Changed` item inside the `Events` area and write your custom code in the `Code Editor`

![`Toggle` inspector](../images/creo/toggle2.png)
The inspector where the `Toggle` class can be configured.

### Example
1. Open the `Code Editor` (cmd + 6)
2. Select the `Changed` item inside the `Events` area and write your custom code in the `Code Editor`
```
Console.write("Toggle value: \(self.value)")
```

### Most important properties
Several UI aspects can be configured in the `Toggle` class but the `selected` is the most common to be configured.
- `selected`: A Boolean value that determines the off/on state of the switch. This property allows you to retrieve and set (without animation) a value determining whether the UISwitch object is on or off.

### References
[Toggle class reference](../classes/Toggle.html) contains a complete list of properties and methods that can be used to customize a `Toggle` object.
