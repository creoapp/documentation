#### Create a filter and apply to an image:
```
// Create a Bokeh Blur filter
// for the list of filter names please see the Filter Reference
var filterBlur = ImageFilter.filterWithName('CIBokehBlur');

// prepare the completion closure
func completionClosure(image) {
    // use the filtered image passed as the argument of the closure
	ImageView1.image = image
}

// The var image is my source Image.
// Apply an array of filters (in this case just my filterBlur).
// The execution is performed in a background thread so the UI stays responsive.
// When the filtered image is ready, the completionClosure is called and the
// filtered image is passed as the only argument of the closure.
image.imageWithFilters([filterBlur], completionClosure)

```
