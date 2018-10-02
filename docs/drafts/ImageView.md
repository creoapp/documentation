An image view displays a single image or an animated sequence of images over a transparent or opaque background. Within an image view, images may be stretched, scaled, sized to fit, or pinned to a specific location. Image views are noninteractive by default.

![ImageView](images/imageview1.png)

### Best practices
* **If possible, make sure all images in an animated sequence are consistently sized.** Ideally, images should be prescaled to fit the view so the system doesn't have to do any scaling. If the system must perform scaling, it's easiest to achieve the desired results when all images are the same size and shape.

### How to use
1. Drop a `ImageView` control from the object panel to a `Window`
2. Use the `ImageView Inspector` to customize its properties like `prop1`, `prop2`, and `prop3`

![`ImageView` inspector](images/imageview2.png)
The inspector where the `ImageView` class can be configured.

### Example
```
Console.write("ImageView value: \(self.value)")
```

### Most important properties
Several UI aspects can be configured in the `ImageView` class but the `PROP1`, `PROP2`, and `PROP3` are the most populars to be configured.
- `PROP1`: A PROP1 description.
- `PROP2`: A PROP2 description.
- `PROP3`: A PROP3 description.

### References
[ImageView class reference](../classes/ImageView.html) contains a complete list of properties and methods that can be used to customize a `ImageView` object.
