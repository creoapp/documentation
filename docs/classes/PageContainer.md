**super**: [UIView](UIView.md) on iOS

A PageContainer is a special built-in control that enables you to build complex dynamic navigations system using the standard <a href="DataSet.html">DataSet</a> and <a href="CustomView.html">Template</a> approach. Without this control if you wan to build an eBook with 50 pages (for simplicitly we can assume that each page is a jpeg image or an html page saved in a database) you would need to add a PageCurl or PageScroll navigation control to Layout and then add 50 Windows within it each one representing a page of the book. This would be a very time consuming and non flexible way to proceed.

With a PageContainer control you can just drop it to a new Window and then configure DataSet to a database or to a folder in 1s and Template to a previously created Template. Configuration is then completed when you bind Cell Properties. A real time preview in Design Board enables you to have complete control of the appearance in real time without executing your app.



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidSelectCell**(**cell**: <strong>[PageContainerCell](PageContainerCell.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>)
Handle this event if you need to execute some code when a new page is selected by the user.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **index**: **[Int](../gravity/types.md)**
Current index.

* **var** **style**: **PageContainerStyle**
Current style.

* **var** **keyPath**: **[String](../gravity/types.md)**
The base keyPath to get a particular node of the <a href="DataSet.html">DataSet</a> value. The DataSet must provide a List of objects and each object is shown in a different page. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath defines the list of keys used to browse the data tree to get a List node. The values for each exposed property of the cell are retrieved by adding the current index and the cell property key to the base keyPath.

* **var** **customView**: **[CustomView](CustomView.md)**
Custom view template set in the PageContainer inspector.



### Initializers

* **func** **PageContainer**(**style**: <strong><a href="#_enum_PageContainerStyle">PageContainerStyle</a></strong>)
Create a new PageContainer with the specified style.



### Methods

* **func** **reload**(**reloadDataSet**: <strong>[Bool](../gravity/types.md)</strong>)
Reloads the content of the PageContainer.

* **func** **goToPageAtIndex**(**index**: <strong>[Int](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md)</strong>)
Go to a specific page inside the PageContainer.

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### PageContainerStyle
 * .Curl
 * .Scroll

<br><br>#### AnimationOption
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

<br><br>

