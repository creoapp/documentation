Carousel is a class designed to simplify the implementation of various types of carousel (paged, scrolling views). Carousel implements a number of common effects such as cylindrical, flat and CoverFlow style carousels, as well as providing hooks to implement your own bespoke effects. Unlike many other CoverFlow libraries, Carousel can work with any kind of view, not just images, so it is ideal for presenting paged data in a fluid and impressive way in your app. It also makes it extremely easy to swap between different carousel effects with minimal code changes.

![Carousel](images/carousel1.png)

### Best practices
* Item1
* Item2

### How to use
1. Drop a `Carousel` control from the object panel to a `Window`
2. Use the `Carousel Inspector` to customize its properties like `Type`, `Perspective`, `Spacing` and `DataSet`

If you need to write code for Carousel:

3. Open the `Code Editor` (cmd + 6)
4. Select the `DidSelectCell` item inside the `Events` area and write your custom code in the `Code Editor`

![`Carousel` inspector](images/carousel2.png)
The inspector where the `Carousel` class can be configured.

### Example
1. Drop a `Slider` control from the object panel to a `Window`
2. Open the `Code Editor` (cmd + 6)
3. Select the `Changed` item inside the `Events` area and write your custom code in the `Code Editor`
```
Carousel1.currentItemIndex = Slider1.value
```
4. Drop a `Button` control from the object panel to a `Window`
5. Open the `Code Editor` (cmd + 6)
6. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`
```
Slider1.maximumValue = Carousel1.numberOfItems
```

### Most important properties
Several UI aspects can be configured in the `Carousel` class but the `type`, `currentItemIndex`, and `numberOfItems` are the most populars to be configured.
- `type`: Used to switch the carousel display type.
- `currentItemIndex`: The index of the currently centered item in the carousel. Setting this property is equivalent to calling scrollToItemAtIndex with the animated argument set to false.
- `numberOfItems`: The number of items in the carousel (read only). Note that not all of these item views will be loaded or visible at a given point in time - the carousel loads item views on demand as it scrolls. 

### References
[Carousel class reference](../classes/Carousel.html) contains a complete list of properties and methods that can be used to customize a `Carousel` object.
