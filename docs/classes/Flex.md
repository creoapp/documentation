**super**: **[Object](Object.md)**

This class is reserved and cannot be directly instantiated.



### Events

* None

### Properties

* **var** **enabled**: **[Bool](../gravity/types.md)**
Decides during layout/sizing whether or not styling properties should be applied

* **var** **includedInLayout**: **[Bool](../gravity/types.md)**
Decides if we should include this view when calculating layout

* **var** **enabledAndInLayout**: **[Bool](../gravity/types.md)**
Same as isEnabled and isIncludedInLayout

* **var** **grow**: **[Float](../gravity/types.md)**
Describes how any space within a container should be distributed among its children along the main axis

* **var** **shrink**: **[Float](../gravity/types.md)**
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

* **var** **overflow**: **Overflow**
overflow

* **var** **display**: **Display**
display

* **var** **aspectRatio**: **[Float](../gravity/types.md)**
Aspect ratio

* **var** **positionType**: **PositionType**
Defines how it is positioned within its parent

* **var** **basis**: **[FlexValue](FlexValue.md)**
Flex basis

* **var** **width**: **[FlexValue](FlexValue.md)**
Width in FlexValue

* **var** **height**: **[FlexValue](FlexValue.md)**
Height in FlexValue

* **var** **minWidth**: **[FlexValue](FlexValue.md)**
Minimum width in FlexValue

* **var** **maxWidth**: **[FlexValue](FlexValue.md)**
Maximum width in FlexValue

* **var** **minHeight**: **[FlexValue](FlexValue.md)**
Minimum height in FlexValue

* **var** **maxHeight**: **[FlexValue](FlexValue.md)**
Maximum height in FlexValue

* **var** **left**: **[FlexValue](FlexValue.md)**
Left position in FlexValue when position type is absolute.

* **var** **top**: **[FlexValue](FlexValue.md)**
Top position in FlexValue when position type is absolute.

* **var** **right**: **[FlexValue](FlexValue.md)**
Right position in FlexValue when poosition type is absolute.

* **var** **bottom**: **[FlexValue](FlexValue.md)**
Bottom position in FlexValue when position type is absolute.

* **var** **start**: **[FlexValue](FlexValue.md)**
Start position in FlexValue when position type is absolute; it depends on text and childrens direction.

* **var** **end**: **[FlexValue](FlexValue.md)**
End position  in FlexValue when position type is absolute; it depends on text and childrens direction.

* **var** **marginLeft**: **[FlexValue](FlexValue.md)**
Margin left in FlexValue

* **var** **marginTop**: **[FlexValue](FlexValue.md)**
Margin top in FlexValue

* **var** **marginRight**: **[FlexValue](FlexValue.md)**
Margin right in FlexValue

* **var** **marginBottom**: **[FlexValue](FlexValue.md)**
Margin bottom in FlexValue

* **var** **marginStart**: **[FlexValue](FlexValue.md)**
Margin start in FlexValue, it depends on text and childrens direction

* **var** **marginEnd**: **[FlexValue](FlexValue.md)**
Margin end in FlexValue, it depends on text and childrens direction

* **var** **marginHorizontal**: **[FlexValue](FlexValue.md)**
Margin horizontal in FlexValue

* **var** **marginVertical**: **[FlexValue](FlexValue.md)**
Margin vertical in FlexValue

* **var** **margin**: **[FlexValue](FlexValue.md)**
Margin in FlexValue

* **var** **paddingLeft**: **[FlexValue](FlexValue.md)**
Padding left in FlexValue

* **var** **paddingTop**: **[FlexValue](FlexValue.md)**
Padding top in FlexValue

* **var** **paddingRight**: **[FlexValue](FlexValue.md)**
Padding right in FlexValue

* **var** **paddingBottom**: **[FlexValue](FlexValue.md)**
Padding bottom in FlexValue

* **var** **paddingStart**: **[FlexValue](FlexValue.md)**
Padding start in FlexValue, it depends on text and childrens direction

* **var** **paddingEnd**: **[FlexValue](FlexValue.md)**
Padding end in FlexValue, it depends on text and childrens direction

* **var** **paddingHorizontal**: **[FlexValue](FlexValue.md)**
Padding horizontal in FlexValue

* **var** **paddingVertical**: **[FlexValue](FlexValue.md)**
Padding vertical in FlexValue

* **var** **padding**: **[FlexValue](FlexValue.md)**
Padding in FlexValue

* **var** **borderLeftWidth**: **[Float](../gravity/types.md)**
Border left width

* **var** **borderTopWidth**: **[Float](../gravity/types.md)**
Border top width

* **var** **borderRightWidth**: **[Float](../gravity/types.md)**
Border right width

* **var** **borderBottomWidth**: **[Float](../gravity/types.md)**
Border bottom width

* **var** **borderStartWidth**: **[Float](../gravity/types.md)**
Border start width, it depends on text and childrens direction

* **var** **borderEndWidth**: **[Float](../gravity/types.md)**
Border end width, it depends on text and childrens direction

* **var** **borderWidth**: **[Float](../gravity/types.md)**
Border width



### Methods

* **func** **applyLayout**()
Apply layout preserving origin

* **func** **calculateLayoutWithSize**(**value**: **[Size](Size.md)**): <strong>[Size](Size.md)</strong> 
Returns the size of the view based on provided constraints. Pass Layout.undefined for an unconstrained dimension.

* **func** **applyLayoutPreservingOrigin**(**value**: **[Bool](../gravity/types.md)**)
Apply layout preserving origin

* **func** **markDirty**()
Mark that a view's layout needs to be recalculated. Only works for leaf views





### Enumeration

#### Direction
 * .Inherit
 * .LTR
 * .RTL

#### FlexDirection
 * .Column
 * .Row

#### Justify
 * .Center
 * .FlexEnd
 * .FlexStart
 * .SpaceAround
 * .SpaceBetween
 * .SpaceEvenly

#### Align
 * .Auto
 * .Baseline
 * .Center
 * .FlexEnd
 * .FlexStart
 * .SpaceAround
 * .SpaceBetween
 * .Stretch

#### Wrap
 * .No
 * .Yes

#### Overflow
 * .Hidden
 * .Scroll
 * .Visible

#### Display
 * .Flex
 * .None

#### PositionType
 * .Absolute
 * .Relative



