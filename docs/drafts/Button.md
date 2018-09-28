Buttons initiate app-specific actions, have customizable backgrounds, and can include a title or an icon. The system provides a number of predefined button styles for most use cases. You can also design fully custom buttons.

![Simple button](images/button1.png)
A simple `Button`.

### Best practices
**Use verbs in titles.** An action-specific title shows that a button is interactive and says what happens when you tap it.

**Use title-case for titles.** Capitalize every word except articles, coordinating conjunctions, and prepositions of four or fewer letters.

**Keep titles short.** Overly long text can crowd your interface and may get truncated on smaller screens.

**Consider adding a border or a background only when necessary.** By default, a system button has no border or background. In some content areas, however, a border or background is necessary to denote interactivity. In the Phone app, bordered number keys reinforce the traditional model of making a call, and the background of the Call button provides an eye-catching target that’s easy to hit.

### How to use
1. Add a `Button` to a `Window`
2. Configure every desired propery from the `Inspector` like `Title` and `Style`
3. Open the `Code Editor` clicking the `View` ->  `Actions Panel`  -> `Code Editor` menu item
4. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`

![The `Button` inspector](images/button2.png)
The inspector where the `Button` class can be configured.

![The `Code Editor` where to interact with events and write custom code](images/button3.png)
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

![The `Button` styles](images/button4.png)
The `Button` styles.
