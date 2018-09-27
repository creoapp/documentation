## Navigation window
A container `Window` that defines a stack-based scheme for navigating hierarchical content.

### Links
- [Creo class documentation](../classes/Navigation)
- [Apple documentation](https://developer.apple.com/documentation/uikit/uinavigationcontroller)

### Overview
A `Navigation Window` is a container that manages one or more `Window` in a navigation interface. In this type of interface, only one `Window` is visible at a time. Tapping the back button in the navigation bar at the top of the interface removes the top `Window`, thereby revealing the `Window` underneath.

![Simple navigation controller](images/navigation3.png)
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

![Simple navigation controller](images/navigation7.png)

### Subnodes of a child `Window`
The navigation bar can be customised by tapping the `Window` subnode icons (+).

![Custom navigation controller](images/navigation1.png)

Any child `Window` `Navigation Bar` may have:
- A custom title
- A custom prompt
- 1 or more left button
- 1 or more right button
- A custom back button

The buttons can both be custom (with a user provided title/image) or selected from the list of the iconic system buttons.
![System buttons](images/navigation2.png)

#### Note:
Without the _Title subnode_ the tile itself is automatically retrieved from the name of the current children `Window`

### UI Properties
Several UI aspects can be configured but (see the inspector) but the `Navigation` title bar color and title size are the more importants.

![Inspector](images/navigation6.png)

![Large navigation bar](images/navigation4.png)
Compact navigation bar.

![Large navigation bar](images/navigation5.png)
Large navigation bar.