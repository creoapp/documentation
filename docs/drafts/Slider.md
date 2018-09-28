A slider is a horizontal track with a control called a thumb, which you can slide with your finger to move between a minimum and maximum value, such as screen brightness level or position during media playback. As a slider’s value changes, the portion of track between the minimum value and the thumb fills with color. A slider can optionally display left and right icons that illustrate the meaning of the minimum and maximum values.

![Simple button](images/slider1.png)
A simple `Slider`.

### Best practices
**Customize a slider’s appearance if it adds value.** A slider’s appearance, including track color, thumb image, and left and right icons, can be adjusted to blend with your app’s design and to communicate intent. A slider that adjusts image size, for example, could show a small image icon on the left and a large image icon on the right.

### How to use
1. Add a `Slider` to a `Window`
2. Configure every desired propery from the `Inspector` like `Title` and `Style`
3. Open the `Code Editor` clicking the `View` ->  `Actions Panel`  -> `Code Editor` menu item
4. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`

![The `Slider` inspector](images/slider2.png)
The inspector where the `Slider` class can be configured.

![The `Code Editor` where to interact with events and write custom code](images/slider3.png)
The `Code Editor` where to interact with events and write custom code.

#### Example
How to show an `Alert` via source code.
```
var alert = Alert("Title", "Message")
alert.show()
```

### Most important properties
Several UI aspects can be configured in the `Button` class but the `Title` and `Style` are the most populars to be configured.
- `TItle`: you can specify a button’s title as a plain string or attributed string.
- `Style`: specifies the style of a button.
