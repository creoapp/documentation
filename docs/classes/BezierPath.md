**super**: [Object](Object.md)

The BezierPath class lets you define a path consisting of straight and curved line segments and render that path in your views. You use this class initially to specify just the geometry for your path. Paths can define simple shapes such as rectangles, ovals, and arcs or they can define complex polygons that incorporate a mixture of straight and curved line segments. After defining the shape, you can use additional methods of this class to render the path in the current drawing context. Default stroke color is black and default fill color is not set.

### Events

* None

### Properties

* **var** **strokeColor**: **[Color](color.md)**
The color of subsequent stroke operations to the color

* **var** **fillColor**: **[Color](color.md)**
The color of subsequent fill operations to the color.

* **var** **lineWidth**: **[Float](../gravity/types.md)**
The line width defines the thickness of the receiver's stroked path. A width of 0 is interpreted as the thinnest line that can be rendered on a particular device. The actual rendered line width may vary from the specified width by as much as 2 device pixels, depending on the position of the line with respect to the pixel grid and the current anti-aliasing settings. The default line width is 1.0.

* **var** **lineCapStyle**: **LineCapStyle**
The shape of the paths end points when stroked.

* **var** **lineJoinStyle**: **LineJoinStyle**
The shape of the joints between connected segments of a stroked path.

* **var** **miterLimit**: **[Float](../gravity/types.md)**
The limiting value that helps avoid spikes at junctions between connected line segments.

* **var** **flatness**: **[Float](../gravity/types.md)**
The factor that determines the rendering accuracy for curved path segments.

* **var** **usesEvenOddFillRule**: **[Bool](../gravity/types.md)**
A Boolean indicating whether the even-odd winding rule is in use for drawing paths.

* **var** **isEmpty**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the path has any valid elements. \(read-only\)



### Methods

* **func** **image**(): <strong>[Image](image.md)</strong> 
Convert the BezierPath to an Image.

* **func** **stroke**()
Draws a line along the receiver’s path using the current drawing properties. The drawn line is centered on the path with its sides parallel to the path segment. This method applies the current drawing properties to the rendered path.

* **func** **fill**()
Paints the region enclosed by the receiver’s path using the current drawing properties. This method fills the path using the current fill color and drawing properties. If the path contains any open subpaths, this method implicitly closes them before painting the fill region. The painted region includes the pixels right up to, but not including, the path line itself. For paths with large line widths, this can result in overlap between the fill region and the stroked path (which is itself centered on the path line).

* **func** **moveToPoint**(**point**: <strong>[Point](point.md)</strong>)
Moves the receiver’s current point to the specified location. This method implicitly ends the current subpath (if any) and sets the current point to the value in the point parameter. When ending the previous subpath, this method does not actually close the subpath. Therefore, the first and last points of the previous subpath are not connected to each other.

* **func** **addLineToPoint**(**point**: <strong>[Point](point.md)</strong>)
Appends a straight line to the receiver’s path. This method creates a straight line segment starting at the current point and ending at the point specified by the point parameter. After adding the line segment, this method updates the current point to the value in point.

* **func** **close**()
Closes the most recent subpath. This method closes the current subpath by creating a line segment between the first and last points in the subpath. This method subsequently updates the current point to the end of the newly created line segment, which is also the first point in the now closed subpath.

* **func** **removeAllPoints**()
Removes all points from the receiver, effectively deleting all subpaths.

* **func** **fillWithBlendMode**(**blendMode**: <strong><a href="#_enum_BlendMode">BlendMode</a></strong>, **alpha**: <strong>[Float](../gravity/types.md)</strong>)
Paints the region enclosed by the receiver’s path using the specified blend mode and transparency values.

* **func** **strokeWithBlendMode**(**blendMode**: <strong><a href="#_enum_BlendMode">BlendMode</a></strong>, **alpha**: <strong>[Float](../gravity/types.md)</strong>)
Draws a line along the receiver’s path using the specified blend mode and transparency values.

* **func** **containsPoint**(**point**: <strong>[Point](point.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether the area enclosed by the receiver contains the specified point.

* **func** **addArc**(**point**: <strong>[Point](point.md)</strong>, **radius**: <strong>[Float](../gravity/types.md)</strong>, **startAngle**: <strong>[Float](../gravity/types.md)</strong>, **endAngle**: <strong>[Float](../gravity/types.md)</strong>, **clockwise**: <strong>[Bool](../gravity/types.md)</strong>)
This method adds the specified arc beginning at the current point. The created arc lies on the perimeter of the specified circle. Specifying a start angle of 0 radians, an end angle of π radians, and setting the clockwise parameter to true draws the bottom half of the circle. However, specifying the same start and end angles but setting the clockwise parameter set to false draws the top half of the circle.

* **func** **addCurve**(**point**: <strong>[Point](point.md)</strong>, **controlPoint**: <strong>[Point](point.md)</strong>, **controlPoint2**: <strong>[Point](point.md)</strong>)
This method appends a cubic Bézier curve from the current point to the end point specified by the endPoint parameter. The two control points define the curvature of the segment.

* **func** **addQuadCurve**(**point**: <strong>[Point](point.md)</strong>, **controlPoint**: <strong>[Point](point.md)</strong>)
This method appends a quadratic Bézier curve from the current point to the end point specified by the endPoint parameter.

* **func** **addRect**(**rect**: <strong>[Rect](rect.md)</strong>)
This method appends a rectangular path.

* **func** **addOval**(**rect**: <strong>[Rect](rect.md)</strong>)
This method appends an oval path inscribed in the specified rectangle.

* **func** **addRoundedRect**(**rect**: <strong>[Rect](rect.md)</strong>, **radius**: <strong>[Float](../gravity/types.md)</strong>)
This method appends a rounded rectangular path.

* **func** **addRoundedRectWithCorners**(**rect**: <strong>[Rect](rect.md)</strong>, **roundingCorners**: <strong><a href="#_enum_RectCorner">RectCorner</a></strong>, **size**: <strong>[Size](size.md)</strong>)
This method appends a rounded rectangular path by specifying the radius of each corner oval.

* **func** **appendPath**(**path**: <strong>[BezierPath](BezierPath.md)</strong>)
Appends the contents of the specified path object to the receiver’s path.





### Enumeration

#### LineCapStyle
 * .Butt
 * .Round
 * .Square

<br><br>#### LineJoinStyle
 * .Bevel
 * .Miter
 * .Round

<br><br>#### BlendMode
 * .Clear
 * .Color
 * .ColorBurn
 * .ColorDodge
 * .Copy
 * .Darken
 * .DestinationAtop
 * .DestinationIn
 * .DestinationOut
 * .DestinationOver
 * .Difference
 * .Exclusion
 * .HardLight
 * .Hue
 * .Lighten
 * .Luminosity
 * .Multiply
 * .Normal
 * .Overlay
 * .PlusDarker
 * .PlusLighter
 * .Saturation
 * .Screen
 * .SoftLight
 * .SourceAtop
 * .SourceIn
 * .SourceOut
 * .XOR

<br><br>#### RectCorner
 * .AllCorners
 * .BottomLeft
 * .BottomRight
 * .TopLeft
 * .TopRight

<br><br>

