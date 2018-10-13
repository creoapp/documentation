A navigation bar appears at the top of an app screen, below the status bar, and enables navigation through a series of hierarchical screens. When a new screen is displayed, a back button, often labeled with the title of the previous screen, appears on the left side of the bar. Sometimes, the right side of a navigation bar contains a control, like an Edit or a Done button, for managing the content within the active view. In a split view, a navigation bar may appear in a single pane of the split view. Navigation bars are translucent, may have a background tint, and can be configured to hide when the keyboard is onscreen, a gesture occurs, or a view resizes.

![Simple navigation controller](images/Navigation_main.png)

### Best practices
Horizontal navigation is a popular navigation pattern widely used to display hierarchical content, ie:
* **the setting of an app**, and the user taps an element to open its subsettings
* **a social item**, and the user taps a preview to open its full description and details

A common App schema is to have a root `Window` like a [TabBar](tabbar) and a `Navigation` for each of its child.
If the navigation is not in a single direction (from generic to detail and viceversa) then `Navigation` may not be appropriate.

### How to use
1. Drop a `Navigation` and customize the main `Navigation Bar`
1. Drop 1 or more child `Window`
1. For each child `Window` customize its `Navigation Bar` subsettings (bar visibility, title, prompt and buttons)
1. Add or remove `Window` by _code_ or by _actions_

### Example
- Start adding a `Navigation` by tapping the _New Navigation_ button on the _bottom bar_

![New Navigation](images/Navigation14.png)

- Configure the `Navigation` appearance and the application hierarchy by adding `Window`child screens
- Configure each screen to add a `TABBAR Item`
- keep doing the same until you have a hierarchy like this

```
- Navigation1
  - Window1 (startup window)
    - Button1
 - Window2
 - Window3
```

### Interacting using Gravity
To push a new `Window` into the hierarchy, ie from a button `Action` call
```
Navigation1.push(Window2)
```

equivalent to

```
Window2.openIn(Navigation1)
```

To pop one level:

```
Navigation1.pop()
```

equivalent to

```
Window2.close()
```

To pop to the root level:
```
Navigation1.popToRootWindow()
```

### Interacting using Actions
1. select the `Button1` _Actions_ tab
1. select _Event_ -> _Action_ and tap _Add_
1. select _Open_ -> _Details1_
1. select _In_ -> _Current_
1. select _Using_ -> _Default_

![Simple navigation controller](images/Navigation10.png)

### Customize a navigation bar
The navigation bar can be customized by tapping the `Window` subnode icons (+).

![Custom navigation controller](images/Navigation1.png)

Any child `Window` `Navigation Bar` may have:
- A custom title
- A custom prompt
- 1 or more left button
- 1 or more right button
- A custom back button

![Customizations](images/Navigation13.png)

The buttons can both be custom (with a user provided title/image) or selected from the list of the iconic system buttons.
![System buttons](images/Navigation2.png)

**Note:** without the _Title subnode_ the title itself is automatically retrieved from the name of the current children `Window`.

### Most important properties
Several UI aspects can be configured but the most used are:
- `Style`, white with dark text or black with light text.
- `Translucent Navigation Bar`, when set _true_ the background is semitransparent.
- `Bar Color`, navigation bar background tint color.
- `Prefer Large Titles`, when set _true_ the title is displayed in a large format.
- `Hide Navigation Bar`, when set _true_ the navigation bar is hidden, usually just the root screen has the navigation bar hidden.

![Inspector](images/Navigation_inspector.png)

![Large navigation bar](images/Navigation12.png)
Compact navigation bar.

![Large navigation bar](images/Navigation9.png)
Large navigation bar.

### References
[Navigation](../classes/Navigation.html) contains a complete list of properties and methods that can be used to customize a `Navigation` object.