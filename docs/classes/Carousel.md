**super**: [UIView](UIView.md) on iOS

Carousel is a class designed to simplify the implementation of various types of carousel (paged, scrolling views). Carousel implements a number of common effects such as cylindrical, flat and CoverFlow style carousels, as well as providing hooks to implement your own bespoke effects. Unlike many other CoverFlow libraries, Carousel can work with any kind of view, not just images, so it is ideal for presenting paged data in a fluid and impressive way in your app. It also makes it extremely easy to swap between different carousel effects with minimal code changes.



### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidSelectCell**(**cell**: <strong>[CarouselCell](CarouselCell.md)</strong>, **index**: <strong>[Int](../gravity/types.md)</strong>)
Handle this event if you need to execute some code when a new cell is selected by the user.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **currentItemIndex**: **[Int](../gravity/types.md)**
The index of the currently centered item in the carousel. Setting this property is equivalent to calling scrollToItemAtIndex with the animated argument set to false.

* **var** **type**: **CarouselType**
Used to switch the carousel display type

* **var** **perspective**: **[Float](../gravity/types.md)**
Used to tweak the perspective foreshortening effect for the various 3D carousel views. Should be a positive value, greater than 0 and less than 1. Values outside of this range will yield very strange results. The default is 0.5.

* **var** **decelerationRate**: **[Float](../gravity/types.md)**
The rate at which the carousel decelerates when flicked. Higher values mean slower deceleration. The default value is 0.95. Values should be in the range 0.0 (carousel stops immediately when released) to 1.0 (carousel continues indefinitely without slowing down, unless it reaches the end).

* **var** **scrollSpeed**: **[Float](../gravity/types.md)**
This is the scroll speed multiplier when the user flicks the carousel with their finger. Defaults to 1.0.

* **var** **bounceDistance**: **[Float](../gravity/types.md)**
The maximum distance that a non-wrapped carousel will bounce when it overshoots the end. This is measured in multiples of the itemWidth, so a value of 1.0 would means the carousel will bounce by one whole item width, a value of 0.5 would be half an item's width, and so on. The default value is 1.0.

* **var** **scrollEnabled**: **[Bool](../gravity/types.md)**
Enables and disables user scrolling of the carousel. The carousel can still be scrolled programmatically if this property is set to false.

* **var** **pagingEnabled**: **[Bool](../gravity/types.md)**
Enables and disables paging. When paging is enabled, the carousel will stop at each item view as the user scrolls, much like the pagingEnabled property of a ScrollView.

* **var** **vertical**: **[Bool](../gravity/types.md)**
This property toggles whether the carousel is displayed horizontally or vertically on screen. All the built-in carousel types work in both orientations. Switching to vertical changes both the layout of the carousel and also the direction of swipe detection on screen. Note that custom carousel transforms are not affected by this property, however the swipe gesture direction will still be affected.

* **var** **wrapEnabled**: **[Bool](../gravity/types.md)**
Returns true if wrapping is enabled and false if it isn't. \(read-only\)

* **var** **bounces**: **[Bool](../gravity/types.md)**
Sets whether the carousel should bounce past the end and return, or stop dead. Note that this has no effect on carousel types that are designed to wrap, or where the wrapEnabled property is set to true.

* **var** **numberOfItems**: **[Int](../gravity/types.md)**
The number of items in the carousel (read only). Note that not all of these item views will be loaded or visible at a given point in time - the carousel loads item views on demand as it scrolls. \(read-only\)

* **var** **numberOfVisibleItems**: **[Int](../gravity/types.md)**
The maximum number of carousel item views to be displayed concurrently on screen. This property is important for performance optimisation, and is calculated automatically based on the carousel type and view frame. \(read-only\)

* **var** **dragging**: **[Bool](../gravity/types.md)**
Returns true if user has started scrolling the carousel and has not yet released it. \(read-only\)

* **var** **decelerating**: **[Bool](../gravity/types.md)**
Returns true if the user isn't dragging the carousel any more, but it is still moving. \(read-only\)

* **var** **scrolling**: **[Bool](../gravity/types.md)**
Returns true if user has started scrolling the carousel and has not yet released it. \(read-only\)

* **var** **scrollToItemBoundary**: **[Bool](../gravity/types.md)**
By default, the carousel will come to rest at an exact item boundary when it is flicked. If you set this property to NO, it will stop naturally and then - if scrollToItemBoundary is set to YES - scroll back or forwards to the nearest boundary.

* **var** **itemBackgroundColor**: **[Color](color.md)**
The background color of items displayed in the carousel.

* **var** **itemBorderWidth**: **[Float](../gravity/types.md)**
The border width of items displayed in the carousel.

* **var** **itemHasReflection**: **[Bool](../gravity/types.md)**
Set to true to add a reflection effect for each item displayed in the carousel.

* **var** **itemReflectionGap**: **[Float](../gravity/types.md)**
The reflection gap of items displayed in the carousel.

* **var** **itemReflectionAlpha**: **[Float](../gravity/types.md)**
The reflection alpha value of items displayed in the carousel.

* **var** **itemReflectionScale**: **[Float](../gravity/types.md)**
The reflection scale value of items displayed in the carousel.

* **var** **itemWidth**: **[Float](../gravity/types.md)**
The display width of items in the carousel.

* **var** **wrap**: **[Bool](../gravity/types.md)**
A boolean indicating whether the carousel should wrap when it scrolls to the end. Set to true if you want the carousel to wrap around when it reaches the end, and false if you want it to stop. Generally, circular carousel types will wrap by default and linear ones won't. Don't worry that the return type is a floating point value - any value other than 0.0 will be treated as true.

* **var** **showBackfaces**: **[Bool](../gravity/types.md)**
For some carousel types, e.g. Cylinder, the rear side of some views can be seen (InvertedCylinder now hides the back faces by default). If you wish to hide the backward-facing views set this option to false. This option may also be useful for custom carousel transforms that cause the back face of views to be displayed.

* **var** **tilt**: **[Float](../gravity/types.md)**
The tilt applied to the non-centered items in the CoverFlow, CoverFlow2 and TimeMachine carousel types. This value should be in the range 0.0 to 1.0.

* **var** **spacing**: **[Float](../gravity/types.md)**
The spacing between item views. This value is multiplied by the item width (or height, if the carousel is vertical) to get the total space between each item, so a value of 1.0 (the default) means no space between views (unless the views already include padding).

* **var** **fadeMin**: **[Float](../gravity/types.md)**
The minimum negative offset an item view can reach before it begins to fade.

* **var** **fadeMax**: **[Float](../gravity/types.md)**
The maximum positive offset a view can reach before if begins to fade.

* **var** **fadeRange**: **[Float](../gravity/types.md)**
The distance over which the fadeout occurs, measured in multiples of an item width (defaults to 1.0).

* **var** **fadeMinAlpha**: **[Float](../gravity/types.md)**
The minimum alpha value to which the views will fade (defaults to 0.0 - fully transparent).

* **var** **keyPath**: **[String](../gravity/types.md)**
The base keyPath to get a particular node of the <a href="DataSet.html">DataSet</a> value. The DataSet must provide a List of objects and each object represents a different item. If the DataSet value is not flat, for example a Map from a JSON result of an <a href="HTTPRequest.html">HTTPRequest</a>, the keyPath defines the list of keys used to browse the data tree to get a List node. The values for each exposed property of the cell are retrieved by adding the current index and the cell property key to the base keyPath.



### Methods

* **func** **reload**(**reloadDataSet**: <strong>[Bool](../gravity/types.md) = true</strong>)
Reload the content of the carousel.

* **func** **removeItemAtIndex**(**index**: <strong>[Int](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
This removes an item from the carousel. The remaining items will slide across to fill the gap. Note that the data source is not automatically updated when this method is called, so a subsequent call to reloadData will restore the removed item.

* **func** **insertItemAtIndex**(**index**: <strong>[Int](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
This inserts an item into the carousel. The new item will be requested from the dataSource, so make sure that the new item has been added to the data source data before calling this method, or you will get duplicate items in the carousel, or other weirdness.

* **func** **reloadItemAtIndex**(**index**: <strong>[Int](../gravity/types.md)</strong>, **animated**: <strong>[Bool](../gravity/types.md) = true</strong>)
This method will reload the specified item view. The new item will be requested from the dataSource. If the animated argument is true, it will cross-fade from the old to the new item view, otherwise it will swap instantly.

* **func** **scrollByOffset**(**offset**: <strong>[Float](../gravity/types.md)</strong>, **duration**: <strong>[Float](../gravity/types.md)</strong>)
This works the same way as scrollByNumberOfItems, but allows you to scroll by a fractional number of items. This may be useful if you wish to achieve a very precise animation effect. Note that if the scrollToItemBoundary property is set to true, the carousel will automatically scroll to the nearest item index after you call this method anyway.

* **func** **scrollToOffset**(**offset**: <strong>[Float](../gravity/types.md)</strong>, **duration**: <strong>[Float](../gravity/types.md)</strong>)
This works the same way as scrollToItemAtIndex, but allows you to scroll to a fractional offset. This may be useful if you wish to achieve a very precise animation effect. Note that if the scrollToItemBoundary property is set to true, the carousel will automatically scroll to the nearest item index after you call this method. anyway.

* **func** **scrollByNumberOfItems**(**itemCount**: <strong>[Int](../gravity/types.md)</strong>, **duration**: <strong>[Float](../gravity/types.md)</strong>)
This method allows you to scroll the carousel by a fixed distance, measured in carousel item widths. Positive or negative values may be specified for itemCount, depending on the direction you wish to scroll. Carousel gracefully handles bounds issues, so if you specify a distance greater than the number of items in the carousel, scrolling will either be clamped when it reaches the end of the carousel (if wrapping is disabled) or wrap around seamlessly.

* **func** **scrollToItemAtIndex**(**index**: <strong>[Int](../gravity/types.md)</strong>, **duration**: <strong>[Float](../gravity/types.md)</strong>)
This method allows you to control how long the carousel takes to scroll to the specified index.

* **func** **animate**(**duration**: <strong>[Float](../gravity/types.md)</strong>, **delay**: <strong>[Float](../gravity/types.md)</strong>, **options**: <strong><a href="#_enum_AnimationOption">AnimationOption</a></strong>, **closure**: <strong>[Closure](../gravity/closures.md)</strong>, **completion**: <strong>[Closure](../gravity/closures.md)</strong>)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### CarouselType
 * .Cylinder
 * .Flow
 * .Flow2
 * .InvertedCylinder
 * .InvertedRotary
 * .InvertedTimeMachine
 * .InvertedWheel
 * .Linear
 * .Rotary
 * .TimeMachine
 * .Wheel

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



