A `Window` presents and manages a hierarchy of views and controls. Each `Window` owns a portion of your app’s user interface. For example, one Window might display a table of items while a different `Window` displays the selected item from that table. Usually, only the views from one `Window` are visible at a time. A `Window` can be presented by another window as a modal window or inside a window container.

![A simple Window inside a Navigation](images/Window1.png)
A simple `Window` inside a `Navigation`.

### How to use
// SCREENSHOT WHERE A WINDOW CAN BE CREATED

### Events
// I REMOVED THE Create a Window section because user has no control over creation

### Open a Window
Windows can be accessed in Gravity through a variable with the name of the `Window` which is unique in the project. Windows are globally defined and are created during the App startup process. A `Window` instance can be used anywhere and anytime from Gravity code.

### Example
If your project has two Windows, `Window1` and `Window2`, you can use the following code to open the `Window2` inside `Window1`: (WHAT DOES INSIDE MEANS)
```
// for example from within the `Action` event of a `Button`
Window2.open()
```

### Availability
A `Window` is created during the loading of the App and its properties are immediately configured with the  values specified through its inspectors. All its properties and methods can be used anytime inside the App. (NOT TRUE, a Window is created during App startup ONLY if it is a Startup Window, if you try to use properties and methods of a never opened Window you'll end up with NULL values. WE SHOULD CLARIFY WHEN controls CAN BE USED.)

### Customization
A appearance of a `Window` can be customized based on where it will be presented.
...
TabBar items and Navigation Bar items are immediately loaded after the creation of the `Window` instance because the container (`TabBar` or `Navigation`) needs to use these objects before presenting the visible content of the `Window`.

The TabBar items and Navigation Bar items can be added to a `Window` by pressing the '+' button near the window's name in the project's layout:

![How to add TabBar items and Navigation Bar items](images/Window2.png)
How to add TabBar items and Navigation Bar items


### Objects
Objects configured inside the `Window`'s hierarchy (controls, views, databases, sensors, gestures, network objects, etc.) are loaded when the `Window` is about to be presented for the first time.

Controls, views and other non-UI objects can be added by dragging the desired object class from the Objects collection in the bottom-right section of the Creo interface.

THE FOLLOWING SECTION IS NOT CLEAR
If you want to open a `Window` and get/set a property of an object of the second group, you have to be sure that `Window` has been presented at least once before accessing that object. You can achieve this by writing the code in the `WillShow` event of the `Window` or in the completion [closure](../gravity/closure.html) of the `open` method. The following example shows how to reliably set the `text` of a `Label` in `Window2`:

```
func completion() {
	Window2.Label1.text = "New Text"
}

Window2.open(completion)
```

The `open` method is executed asynchronously and it returns immediately (that means that it doesn't wait for `Window2` to be presented and available). It is not right to write any code that access `Window2` immediately after its open method. 
If you need to write initialization code for a Window you can use the Will/DidShow event or pass a closure to its open method: EXPLAIN HERE

The following sequence of steps is performed during the presentation of a `Window`:
1. if the Window's content has not yet been loaded (the first time that the `Window` is presented) all its subnodes are created and added to the `Window`'s hierarchy if needed.
2. the `WillShow` event of the `Window` is called.
3. if a completion closure has been set as a parameter of the open method, it is executed.
4. the `Window` is added to a view hierarchy and the presenting animation is performed.
5. when the presenting animation ends the `DidShow` event of the `Window` is called.

For the complete list of the open methods, please refer to the documentation of the [Window](../classes/Window.html) class and to the documentation of the window containers.

### Classes
- [Window](../classes/Window.html)

### Tutorials
- [ToDo](../tutorials/todo.html)
- [Lets Cook Navigation](../tutorials/lets-cook-nav.html)