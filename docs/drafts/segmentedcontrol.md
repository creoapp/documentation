A segmented control is a linear set of two or more segments, each of which functions as a mutually exclusive button. Within the control, all segments are equal in width. Like `buttons`, segments can contain text or images. Segmented controls are often used to display different views. In Maps, for example, a segmented control lets you switch between Map, Transit, and Satellite views.

![Simple segmented control](images/segmentedcontrol1.png)
A simple `SegmentedControl`.

### Best practices
*Limit the number of segments to improve usability.* Wider segments are easier to tap. On iPhone, a segmented control should have five or fewer segments.

*Try to keep segment content size consistent.* Because all segments have equal width, it doesn’t look great if content fills some segments but not others.

*Avoid mixing text and images in a segmented control.* Although individual segments can contain text or images, mixing the two in a single control can lead to a disconnected and confusing interface.

*Position content appropriately in a custom segmented control.* If you change the background appearance of a segmented control, make sure content still looks good and doesn’t appear misaligned.

### How to use
1. Add a `SegmentedControl` to a `Window`
//2. Configure every desired propery from the `Inspector` like `Title` and `Style`
//3. Open the `Code Editor` clicking the `View` ->  `Actions Panel`  -> `Code Editor` menu item
//4. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`

![The `SegmentedControl` inspector](images/segmentedcontrol2.png)
The inspector where the `SegmentedControl` class can be configured.

![The `Code Editor` where to interact with events and write custom code](images/segmentedcontrol3.png)
The `Code Editor` where to interact with events and write custom code.

#### Example
How to show an `Alert` via source code.
```
var alert = Alert("Title", "Message")
alert.show()
```

### Most important properties
Several UI aspects can be configured in the `Button` class but the `Title` and `Style` are the most populars to be configured.
- TItle: you can specify a button’s title as a plain string or attributed string.
- Style: specifies the style of a button.

![The `Button` styles](images/button4.png)
The `Button` styles.
