```
// How to programmatically stretch a background image to fill a button background
// Add this code in the button Load() function.

// Load a generic button background image, it's middle content can be stretched but not the corners!
var img = Image("button_image");

// Create an EdgeInset according to the button's shape to "cut-out" the corners (20x20 is a size measured in points)
var edge = EdgeInsets(20, 20, 20, 20);

// Create a new image with the loaded button background and the properly set EdgeInsets
img = img.resizableImageWithCapInsets(edge, ImageResizingMode.Stretch);

// Set the image as the new background image for the current button
self.setBackgroundImageForState(img, ControlState.Normal);
```

