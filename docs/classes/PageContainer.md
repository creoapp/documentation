**super**: **[UIView](UIView.md)** (on iOS)

A PageContainer is a special built-in control that enables you to build complex dynamic navigations system using the standard <a href="DataSet.html">DataSet</a> and <a href="CustomView.html">Template</a> approach. Without this control if you wan to build an eBook with 50 pages (for simplicitly we can assume that each page is a jpeg image or an html page saved in a database) you would need to add a PageCurl or PageScroll navigation control to Layout and then add 50 Windows within it each one representing a page of the book. This would be a very time consuming and non flexible way to proceed.

With a PageContainer control you can just drop it to a new Window and then configure DataSet to a database or to a folder in 1s and Template to a previously created Template. Configuration is then completed when you bind Cell Properties. A real time preview in Design Board enables you to have complete control of the appearance in real time without executing your app.



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidSelectCell**(**cell**: **[PageContainerCell](PageContainerCell.md)**, **index**: **[Int](../gravity/int.md)**)
Handle this event if you need to execute some code when a new page is selected by the user.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **index**: **[Int](../gravity/int.md)**
Current index.

* **var** **style**: **PageContainerStyle**
Current style.

* **var** **dataSet**: **[Object](../gravity/object.md)**
The <a href="DataSet.html">DataSet</a> object provides information that PageContainer needs to construct its content. The dataSet must return a List of objects and each object represents a different row. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath property defines the list of keys used to browse the data tree to get a List node.

* **var** **keyPath**: **[String](../gravity/string.md)**
The base keyPath to get a particular node of the <a href="DataSet.html">DataSet</a> value. The DataSet must provide a List of objects and each object is shown in a different page. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath defines the list of keys used to browse the data tree to get a List node. The values for each exposed property of the cell are retrieved by adding the current index and the cell property key to the base keyPath.

* **var** **customView**: **[CustomView](CustomView.md)**
Custom view template set in the PageContainer inspector.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Initializers

* **func** **PageContainer**(**style**: **<a href="#_enum_PageContainerStyle">PageContainerStyle</a>**)
Create a new PageContainer with the specified style.



### Methods

* **func** **reload**(**reloadDataSet**: **[Bool](../gravity/bool.md)**)
Reloads the content of the PageContainer.

* **func** **goToPageAtIndex**(**index**: **[Int](../gravity/int.md)**, **animated**: **[Bool](../gravity/bool.md)**)
Go to a specific page inside the PageContainer.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control



* None

### Enums

<div id="_enum_PageContainerStyle"></div>

#### PageContainerStyle
 * .Curl
 * .Scroll

<div id="_enum_AnimationOption"></div>

#### AnimationOption
 * .AllowAnimatedContent
 * .AllowUserInteraction
 * .Autoreverse
 * .BeginFromCurrentState
 * .CurveEaseIn
 * .CurveEaseInOut
 * .CurveEaseOut
 * .CurveLinear
 * .LayoutSubviews
 * .OverrideInheritedCurve
 * .OverrideInheritedDuration
 * .OverrideInheritedOptions
 * .Repeat
 * .ShowHideTransitionViews
 * .TransitionCrossDissolve
 * .TransitionCurlDown
 * .TransitionCurlUp
 * .TransitionFlipFromBottom
 * .TransitionFlipFromLeft
 * .TransitionFlipFromRight
 * .TransitionFlipFromTop
 * .TransitionNone



