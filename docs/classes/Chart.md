**super**: **[UIView](UIView.md)** (on iOS)

The Chart class offers a built-in and ready to use control to easely display graphical representation of data. Chart supports five type of graphs representation: Bar, Pie, Line, Area and Scatter.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
The view is about to be added to the App's views hierarchy.

* **WillHide**()
The view is about to be removed from the App's views hierarchy.

* **DidShow**()
The view has been added to the App's views hierarchy.

* **DidHide**()
The view has been removed from the App's views hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **chartType**: **<a href="#_enum_ChartType">ChartType</a>**
The graphical representation type

* **var** **animated**: **[Bool](../gravity/bool.md)**
If true, animates its presentation; otherwise, does not.

* **var** **itemWidth**: **[Float](../gravity/float.md)**
Width of each item, measured in points. Depending on the chartType, the item can be a bar (Bar type) or a point (Line, Area or Scatter). This property is not used in the Pie chart.

* **var** **itemDistance**: **[Float](../gravity/float.md)**
Distance between the center of two items, measured in points. If 0, the system automatically calculates a distance value. This property is not used in the Pie and in the Scatter charts.

* **var** **itemBorderWidth**: **[Float](../gravity/float.md)**
The width of the border line of the items, measured in points.

* **var** **itemBorderColor**: **[Color](Color.md)**
The color of the border line of the items.

* **var** **itemPointStyle**: **<a href="#_enum_ChartPointStyle">ChartPointStyle</a>**
The shape of the point. Applies only for the Line, the Area and the Scatter chart types.

* **var** **itemCornerRadius**: **[Float](../gravity/float.md)**
The corner radius of bars. Applies only for the Bar chart type.

* **var** **itemDecorationStyle**: **<a href="#_enum_ChartDecorationStyle">ChartDecorationStyle</a>**
The type of decoration applied to the items fill color. Applies only for the Bar chart type.

* **var** **showsAxisX**: **[Bool](../gravity/bool.md)**
If true, shows the X axis line; otherwise, does not.

* **var** **showsLabelX**: **[Bool](../gravity/bool.md)**
If true, shows the X axis labels; otherwise, does not.

* **var** **showsAxisY**: **[Bool](../gravity/bool.md)**
If true, shows the Y axis line; otherwise, does not.

* **var** **showsLabelY**: **[Bool](../gravity/bool.md)**
If true, shows the Y axis labels; otherwise, does not.

* **var** **dataSet**: **[Object](../gravity/object.md)**
The <a href="DataSet.html">DataSet</a> object provides information that Chart needs to construct its content.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **reload**(**reloadDataSet**: **[Bool](../gravity/bool.md)**)
Reload the content of the chart.

* **func** **animate**(**duration**: **[Float](../gravity/float.md)**, **delay**: **[Float](../gravity/float.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **animations**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="animations ()" data-content="The animations closure, if set, contains the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value.">Closure</a>**, **completion**: **<a href="../gravity/closure.html" data-toggle="popover" data-trigger="hover" title="completion (finished: Bool)" data-content="The completion closure, if set, is executed when the animation sequence ends. This block has no return value and takes a single Bool argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle.">Closure</a>**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enums

<div id="_enum_ChartType"></div>

#### ChartType
 * .Area
 * .Bar
 * .Line
 * .Pie
 * .Scatter

<div id="_enum_ChartPointStyle"></div>

#### ChartPointStyle
 * .Circle
 * .None
 * .Square

<div id="_enum_ChartDecorationStyle"></div>

#### ChartDecorationStyle
 * .Glossy1
 * .Glossy2
 * .Gradient
 * .None

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



