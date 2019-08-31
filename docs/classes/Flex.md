**super**: **[Object](../gravity/object.md)**

This class is reserved and cannot be directly instantiated.





### Properties

* **var** **enabled**: **[Bool](../gravity/bool.md)**
Decides during layout/sizing whether or not styling properties should be applied

* **var** **includedInLayout**: **[Bool](../gravity/bool.md)**
Decides if we should include this view when calculating layout

* **var** **enabledAndInLayout**: **[Bool](../gravity/bool.md)**
Same as isEnabled and isIncludedInLayout

* **var** **grow**: **[Float](../gravity/float.md)**
Describes how any space within a container should be distributed among its children along the main axis

* **var** **shrink**: **[Float](../gravity/float.md)**
Describes how to shrink children along the main axis in the case that the total size of the children overflow the size of the container on the main axis

* **var** **direction**: **Direction**
Specifies the direction in which children and text in a hierarchy should be laid out

* **var** **flexDirection**: **FlexDirection**
Controls the direction in which children of a view are laid out. This is also referred to as the main axis

* **var** **justifyContent**: **Justify**
Describes how to align children within the main axis of their container

* **var** **alignContent**: **Align**
Defines the distribution of lines along the cross-axis. This only has effect when items are wrapped to multiple lines using flex wrap.

* **var** **alignItems**: **Align**
Describes how to align children along the cross axis of their container

* **var** **alignSelf**: **Align**
Has the same options and effect as align items but instead of affecting the children within a container, you can apply this property to a single child to change its alignment within its parent

* **var** **wrap**: **Wrap**
Controls what happens when children overflow the size of the container along the main axis

* **var** **display**: **Display**
display is flex or none, with none the view is removed from the flex layout

* **var** **aspectRatio**: **[Float](../gravity/float.md)**
Aspect ratio, the ratio between the width and the height of a view

* **var** **positionType**: **PositionType**
Defines how it is positioned within its parent; absolute remove the view from the flex flow and position it at the given position

* **var** **basis**: **[FlexValue](FlexValue.md)**
Flex basis, default size of a view along the main axis

* **var** **width**: **[FlexValue](FlexValue.md)**
Width in FlexValue, width dimension of the view

* **var** **height**: **[FlexValue](FlexValue.md)**
Height in FlexValue, height dimension of the view

* **var** **minWidth**: **[FlexValue](FlexValue.md)**
Minimum width in FlexValue, minimum width of the view

* **var** **maxWidth**: **[FlexValue](FlexValue.md)**
Maximum width in FlexValue, maximum width of the view

* **var** **minHeight**: **[FlexValue](FlexValue.md)**
Minimum height in FlexValue, minimum height of the view

* **var** **maxHeight**: **[FlexValue](FlexValue.md)**
Maximum height in FlexValue, maximum height of the view

* **var** **left**: **[FlexValue](FlexValue.md)**
Left position in FlexValue when position type is absolute.

* **var** **top**: **[FlexValue](FlexValue.md)**
Top position in FlexValue when position type is absolute.

* **var** **right**: **[FlexValue](FlexValue.md)**
Right position in FlexValue when position type is absolute.

* **var** **bottom**: **[FlexValue](FlexValue.md)**
Bottom position in FlexValue when position type is absolute.

* **var** **start**: **[FlexValue](FlexValue.md)**
Start position in FlexValue when position type is absolute; it depends on text and childrens direction.

* **var** **end**: **[FlexValue](FlexValue.md)**
End position in FlexValue when position type is absolute; it depends on text and childrens direction.

* **var** **marginLeft**: **[FlexValue](FlexValue.md)**
Margin left in FlexValue, affects the spacing around the outside of a view

* **var** **marginTop**: **[FlexValue](FlexValue.md)**
Margin top in FlexValue, affects the spacing around the outside of a view

* **var** **marginRight**: **[FlexValue](FlexValue.md)**
Margin right in FlexValue, affects the spacing around the outside of a view

* **var** **marginBottom**: **[FlexValue](FlexValue.md)**
Margin bottom in FlexValue, affects the spacing around the outside of a view

* **var** **marginStart**: **[FlexValue](FlexValue.md)**
Margin start in FlexValue, it depends on text and childrens direction. Affects the spacing around the outside of a view

* **var** **marginEnd**: **[FlexValue](FlexValue.md)**
Margin end in FlexValue, it depends on text and childrens direction. Affects the spacing around the outside of a view

* **var** **marginHorizontal**: **[FlexValue](FlexValue.md)**
Margin horizontal in FlexValue, affects the spacing around the outside of a view

* **var** **marginVertical**: **[FlexValue](FlexValue.md)**
Margin vertical in FlexValue

* **var** **margin**: **[FlexValue](FlexValue.md)**
Margin in FlexValue, affects the spacing around the outside of a view

* **var** **paddingLeft**: **[FlexValue](FlexValue.md)**
Padding left in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children

* **var** **paddingTop**: **[FlexValue](FlexValue.md)**
Padding top in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children

* **var** **paddingRight**: **[FlexValue](FlexValue.md)**
Padding right in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children

* **var** **paddingBottom**: **[FlexValue](FlexValue.md)**
Padding bottom in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children

* **var** **paddingStart**: **[FlexValue](FlexValue.md)**
Padding start in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children, it depends on text and childrens direction

* **var** **paddingEnd**: **[FlexValue](FlexValue.md)**
Padding end in FlexValue, it depends on text and childrens direction

* **var** **paddingHorizontal**: **[FlexValue](FlexValue.md)**
Padding horizontal in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children

* **var** **paddingVertical**: **[FlexValue](FlexValue.md)**
Padding vertical in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children

* **var** **padding**: **[FlexValue](FlexValue.md)**
Padding in FlexValue, affects the size of the view it is applied to and eventually offset the location of any children

* **var** **borderLeftWidth**: **[Float](../gravity/float.md)**
Border left width, acts exactly like padding. Does not do any drawing.

* **var** **borderTopWidth**: **[Float](../gravity/float.md)**
Border top width, acts exactly like padding. Does not do any drawing.

* **var** **borderRightWidth**: **[Float](../gravity/float.md)**
Border right width, acts exactly like padding. Does not do any drawing.

* **var** **borderBottomWidth**: **[Float](../gravity/float.md)**
Border bottom width, acts exactly like padding. Does not do any drawing.

* **var** **borderStartWidth**: **[Float](../gravity/float.md)**
Border start width, it depends on text and childrens direction

* **var** **borderEndWidth**: **[Float](../gravity/float.md)**
Border end width, it depends on text and childrens direction

* **var** **borderWidth**: **[Float](../gravity/float.md)**
Border width, acts exactly like padding. Does not do any drawing.

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **applyLayout**()
Apply layout preserving origin

* **func** **calculateLayoutWithSize**(**value**: **[Size](Size.md)**)<strong>: [Size](Size.md)</strong> 
Returns the size of the view based on provided constraints. Pass Layout.undefined for an unconstrained dimension.

* **func** **applyLayoutPreservingOrigin**(**value**: **[Bool](../gravity/bool.md)**)
Apply layout preserving origin

* **func** **markDirty**()
Mark that a view's layout needs to be recalculated. Only works for leaf views





### Enums

<div id="_enum_Direction"></div>

#### Direction
 * .Inherit
 * .LTR
 * .RTL

<div id="_enum_FlexDirection"></div>

#### FlexDirection
 * .Column
 * .Row

<div id="_enum_Justify"></div>

#### Justify
 * .Center
 * .FlexEnd
 * .FlexStart
 * .SpaceAround
 * .SpaceBetween
 * .SpaceEvenly

<div id="_enum_Align"></div>

#### Align
 * .Auto
 * .Baseline
 * .Center
 * .FlexEnd
 * .FlexStart
 * .SpaceAround
 * .SpaceBetween
 * .Stretch

<div id="_enum_Wrap"></div>

#### Wrap
 * .No
 * .Yes

<div id="_enum_Display"></div>

#### Display
 * .Flex
 * .None

<div id="_enum_PositionType"></div>

#### PositionType
 * .Absolute
 * .Relative



