A `Window` presents and manages a hierarchy of views and controls. Each `Window` owns a portion of your app’s user interface. For example, one Window might display a table of items while a different `Window` displays the selected item from that table. Usually, only the views from one `Window` are visible at a time. A `Window` can be presented by another window as a modal window or inside a window container.

![A simple Window inside a Navigation](images/Window_main.png)

### How to use
1. Select an item in the layout panel where you want to add the new `Window`. If the selected item is a window container, the new `Window` will be created inside the container. If you select a `Window`, the new `Window` will be created in the same container of the selected `Window`. If you don’t have any item selected, the new `Window` will be created at the root level.
2. Add a new `Window` with the _new window_ button in the containers panel located below the Layout section (see the following screenshot).
3. Use the `Window Inspector` to customize its properties like `Background Color`, `Tint Color`, and `Supported Orientation`.

![How to create a new Window](images/Window_create.png)
How to create a new Window.

### Events
* `Load`, `Unload`: use these events to customise properties of the `Window` when the object is created.
* `WillShow`, `DidShow`, `WillHide`, `DidHide`: use these events to customise the content of the `Window`, all the content of the `Window` is loaded when these events are called (ref: [Availability](#Availability) section).
* `KeyboadWillShow`, `KeyboadDidShow`, `KeyboadWillHide`, `KeyboadDidHide`: use these events to update the interface of the `Window` in response to the appearing/disappearing of the keyboard, for example [Scrolling interface when Keyboard appears](../technotes/keyboard-avoiding-textfields.html).
* `DidShake`: receives a notification when the user perform a shake gesture.

### Open a Window
Windows can be accessed in Gravity through a variable with the name of the `Window` which is unique in the project. Windows are globally defined and are created during the App startup process. A `Window` instance can be used anywhere and anytime from Gravity code.

A window can be programmatically opened using one of the following methods of the `Window` object that you want to open:
* openIn(destination, completion): opens the calling `Window` in the specified destination. If the destination is a `Window`, the calling `Window` is presented modally with the default transition. If the destination is a window container (`Navigation`,`TabBar`,`PageSplit`,`PageCurl` or `PageSplit`), the `Window` is presented by the destination's specific implementation of the `openWindow(window,closure)` method. If the destination object is not contained in the currently presented stack of windows/containers, the `openIn` has no visible effects until the destination object is presented on screen. The completion [closure](../gravity/closure.html) parameter is optional.
* open(completion): opens the calling `Window` in the current top-most container, if any, or as a modal `Window` if the currently presented `Window` is the root object or is presented as a modal `Window`. The completion [closure](../gravity/closure.html) parameter is optional.
* openModal(TransitionStyle, completion): the calling `Window` is presented modally in the current top-most window or container, using the specified transition. The completion [closure](../gravity/closure.html) parameter is optional.

Another way to open a Window is to use the `openWindow(window,completion)` of an existing container.
If the `Window` is already contained in the container, the `Window` is presented by selecting it between the contained windows.

### Example
Let's say you have a hierarchy like this
```
- Navigation1
  - Window1
```

If your want to open a `Window` named _Window2_ in the current context of your App (in this case, push the _Window2_ at the top of the stack of the _Navigation1_, with a back button to return to _Window1_), you can use the following code:
```
// for example from within the `Action` event of a `Button`
Window2.open()
```

The same result could be achieved with the this code:
```
Window2.openIn(Navigation1)
```

or with this code:
```
Navigation1.openWindow(Window2)
```

If you want to open the _Window2_ as a modal window instead of as inside the _Navigatin1_, use the following code:
```
// you can use any of the supported transition styles
Window2.openModal(TransitionStyle.Default)
```

### Customization
The appearance of a `Window` can be customized based on where it will be presented.

If the `Window` is presented inside a `NavigationBar`, you can customize the items shown in the bar by adding `NavigationBar` items:
1. Press the '+' button near the window's name in the project's layout.
2. Choose the desired item to customize from the `NavigationBar` section of the pop-up menu:
	* `Title Item` to customize properties like `Title`, `Large Title Mode` and `Prompt`. You can add only one `Title Item` per `Window`.
	* `Back Item` to customize the properties of the back button presented when the `Window` is immediately below the top item in the `NavigationBar`'s stack. You can add only one `Back Item` per `Window`.
	* `Left Item` to add a `BarButtonItem` in the left part of the bar.
	* `Right Item` to add a `BarButtonItem` in the right part of the bar.
3. Use the `Inspector` of the selected item to customize its properties.

![How to customize a NavigationBar item](images/Window_navBarItem.png)
How to customize a NavigationBar item.

If the `Window` is presented inside a `TabBar`, you can customize the `TabBarItem` that represents the `Window` in the `TabBar`:
1. Press the '+' button near the window's name in the project's layout.
2. Choose `Item` value in the `TabBar` section of the pop-up menu.
3. Use the `TabBarItem Inspector` to customize its properties like `Title`, `Image` and `Badge`.

### Objects
You can add controls, views, databases, gesture recognizers, network objects, sensors, etc. by dropping the desired class from the object panel. For further information on how to add and configure a specific object, please refer to the documentation of that specific class.

### <a id="Availability"></a>Availability
A `Window` is created during the loading of the App and its properties are immediately configured with the values specified through its inspectors. All its properties and methods can be used anytime inside the App.
Instead, objects added inside a `Window` (controls, databases, etc.) are loaded when the `Window` is about to be presented for the first time for efficiency and performance reasons.

For example, if you want to open a `Window` name _Window2_ and configure `text` of a `Label` named _Label1_ inside _Window2_, you should be sure that the _Label1_ is loaded before using `Window2.Label1.text = "New Text"`.
You can safely use the content of a `Window` in the following ways:
* in the `WillShow` or `DidShow` events of the `Window`
* in the completion [closure](../gravity/closure.html) of the open methods (see the following example)

```
func completion() {
	Window2.Label1.text = "New Text"
}

Window2.open(completion)
```

The `open` method is executed asynchronously and it returns immediately (that means that it doesn't wait for `Window2` to be presented and available). It is not right to write any code that access _Window2_'s content immediately after its open method.

The following sequence of steps is performed during the presentation of a `Window`:
1. if the Window's content has not yet been loaded (the first time that the `Window` is presented) all its subnodes are created and added to the `Window`.
2. the `WillShow` event of the `Window` is called.
3. if a completion closure has been set as a parameter of the open method, it is executed.
4. the `Window` is added to a view hierarchy and the presenting animation is performed.
5. when the presenting animation ends, the `DidShow` event of the `Window` is called.

For the complete list of the open methods, please refer to the documentation of the [Window](../classes/Window.html) class and to the documentation of the window containers.

### Classes
- [Window](../classes/Window.html) contains a complete list of properties and methods that can be used to customize a `Window` object.

### Tutorials
- [ToDo](../tutorials/todo.html)
- [Lets Cook Navigation](../tutorials/lets-cook-nav.html)

### TechNotes
- [Scrolling interface when Keyboard appears](../technotes/keyboard-avoiding-textfields.html)
