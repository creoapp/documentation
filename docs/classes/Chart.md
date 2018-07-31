**super**: **[UIView](UIView.md)** (on iOS)

The Chart class offers a built-in and ready to use control to easely display graphical representation of data. Chart supports five type of graphs representation: Bar, Pie, Line, Area and Scatter.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **chartType**: **ChartType**
The graphical representation type

* **var** **animated**: **[Bool](../gravity/types.md)**
If true, animates its presentation; otherwise, does not.

* **var** **itemWidth**: **[Float](../gravity/types.md)**
Width of each item, measured in points. Depending on the chartType, the item can be a bar (Bar type) or a point (Line, Area or Scatter). This property is not used in the Pie chart.

* **var** **itemDistance**: **[Float](../gravity/types.md)**
Distance between the center of two items, measured in points. If 0, the system automatically calculates a distance value. This property is not used in the Pie and in the Scatter charts.

* **var** **itemBorderWidth**: **[Float](../gravity/types.md)**
The width of the border line of the items, measured in points.

* **var** **itemBorderColor**: **[Color](Color.md)**
The color of the border line of the items.

* **var** **itemPointStyle**: **ChartPointStyle**
The shape of the point. Applies only for the Line, the Area and the Scatter chart types.

* **var** **itemCornerRadius**: **[Float](../gravity/types.md)**
The corner radius of bars. Applies only for the Bar chart type.

* **var** **itemDecorationStyle**: **ChartDecorationStyle**
The type of decoration applied to the items fill color. Applies only for the Bar chart type.

* **var** **showsAxisX**: **[Bool](../gravity/types.md)**
If true, shows the X axis line; otherwise, does not.

* **var** **showsLabelX**: **[Bool](../gravity/types.md)**
If true, shows the X axis labels; otherwise, does not.

* **var** **showsAxisY**: **[Bool](../gravity/types.md)**
If true, shows the Y axis line; otherwise, does not.

* **var** **showsLabelY**: **[Bool](../gravity/types.md)**
If true, shows the Y axis labels; otherwise, does not.

* **var** **dataSet**: **[Object](../gravity/types.md)**
The <a href="DataSet.html">DataSet</a> object provides information that Chart needs to construct its content.



### Methods

* **func** **reload**(**reloadDataSet**: **[Bool](../gravity/types.md)**)
Reload the content of the chart.

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### ChartType
 * .Area
 * .Bar
 * .Line
 * .Pie
 * .Scatter

#### ChartPointStyle
 * .Circle
 * .None
 * .Square

#### ChartDecorationStyle
 * .Glossy1
 * .Glossy2
 * .Gradient
 * .None

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



