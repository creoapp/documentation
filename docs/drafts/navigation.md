## Navigation window
A container `Window` that defines a stack-based scheme for navigating hierarchical content.

### Links
- [Creo class documentation](../classes/Navigation)
- [Apple documentation](https://developer.apple.com/documentation/uikit/uinavigationcontroller)

### Overview
A navigation bar appears at the top of an app screen, below the status bar, and enables navigation through a series of hierarchical screens. When a new screen is displayed, a back button, often labeled with the title of the previous screen, appears on the left side of the bar. Sometimes, the right side of a navigation bar contains a control, like an Edit or a Done button, for managing the content within the active view. In a split view, a navigation bar may appear in a single pane of the split view. Navigation bars are translucent, may have a background tint, and can be configured to hide when the keyboard is onscreen, a gesture occurs, or a view resizes.

![Simple navigation controller](images/navigation8.png)
A simple navigation controller with a single child `Window`.

### When to use
Horizontal navigation is a popular navigation pattern widely used to display hierarchical content, ie:
- the setting of an app, and the user taps an element to open its subsettings
- a social item, and the user taps a preview to open its full description and details

A common App schema is to have a root `Window` like a [TabBar](tabbar) and a `Navigation Window` for each of its child.

### When not to use
If the navigation is not in a single direction (from generic to detail and viceversa) then the `Navigation Window` may not be appropriate.

### How to use
1. add a `Navigation Window` and customise the main `Navigation Bar`
1. add 1 or more child `Window`
1. for each child `Window` customize its `Navigation Bar` subsettings (bar visibility, title, prompt and buttons)
1. add or remove `Window` by _code_ or by _actions_

#### Example
Let's say you have a hierarchy like this, and your _Root_ is the startup window
```
- Navigation1
  - Root (startup window)
    - Button1
 - Details1
 - Details2
```

#### Interacting using Gravity

To push a new `Window` into the hierarchy, ie from a button `Action` call
```
Navigation1.push(Details1)
```

To pop one level:

```
Navigation1.pop()
```

or to pop to the root level:
```
Navigation1.popToRootWindow()
```

#### Interacting using Actions

1. select the `Button1` _Actions_ tab
1. select _Event_ -> _Action_ and tap _Add_
1. select _Open_ -> _Details1_
1. select _In_ -> _Current_
1. select _Using_ -> _Default_

![Simple navigation controller](images/navigation10.png)

### Subnodes of a child `Window`
The navigation bar can be customised by tapping the `Window` subnode icons (+).

![Custom navigation controller](images/navigation1.png)

Any child `Window` `Navigation Bar` may have:
- A custom title
- A custom prompt
- 1 or more left button
- 1 or more right button
- A custom back button

![Customizations](images/navigation13.png)

The buttons can both be custom (with a user provided title/image) or selected from the list of the iconic system buttons.
![System buttons](images/navigation2.png)

#### Note:
Without the _Title subnode_ the tile itself is automatically retrieved from the name of the current children `Window`.

### UI Properties
Several UI aspects can be configured but (see the inspector) but the `Navigation` title bar color and title size are the more importants.

![Inspector](images/navigation11.png)

![Large navigation bar](images/navigation12.png)
Compact navigation bar.

![Large navigation bar](images/navigation9.png)
Large navigation bar.