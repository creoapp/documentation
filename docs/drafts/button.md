Buttons initiate app-specific actions, have customizable backgrounds, and can include a title or an icon. The system provides a number of predefined button styles for most use cases. You can also design fully custom buttons.

![Simple button](images/button1.png)
A simple `Button`.

### Best practices
When you tap a button, the button performs an action where the user can execute custom source code.
A button is tipically used by the user to execute custom actions like open a `Window` or just play an `Animation`.

### How to use
1. Add a button to a `Window`
2. Configure every desired propery from the `Inspector` like `Title` and `Style`
3. Open the `Code Editor` clicking the `View` ->  `Actions Panel`  -> `Code Editor` menu item
4. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`

![The `Button` inspector](images/button2.png)
The inspector where the `Button` class can be configured.

![How to open the `Code Editor` using the application menu](images/button3.png)
How to open the `Code Editor` using the application menu.

![The `Code Editor` where to interact with events and write custom code](images/button4.png)
The `Code Editor` where to interact with events and write custom code.

#### Example
How to show an `Alert` via source code.
```
var alert = Alert("Title", "Message")
alert.show()
```

### Most important properties
Several UI aspects can be configured in the `Button` class but the `Title` and `Style` are the most populars to be configured.
- TItle
You can specify a button’s title as a plain string or attributed string.

- Style
Specifies the style of a button.

![The `Button` styles](images/button5.png)
[The `Button` styles.

### Links
- [Creo class documentation](../classes/Button)
- [Apple documentation](https://developer.apple.com/documentation/uikit/uibutton)
