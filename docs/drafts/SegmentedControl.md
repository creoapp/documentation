A segmented control is a linear set of two or more segments, each of which functions as a mutually exclusive button. Within the control, all segments are equal in width. Like `buttons`, segments can contain text or images. Segmented controls are often used to display different views. In Maps, for example, a segmented control lets you switch between Map, Transit, and Satellite views.

![Simple segmented control](images/segmentedcontrol1.png)
A simple `SegmentedControl`.

### Best practices
**Limit the number of segments to improve usability.** Wider segments are easier to tap. On iPhone, a segmented control should have five or fewer segments.

**Try to keep segment content size consistent.** Because all segments have equal width, it doesn’t look great if content fills some segments but not others.

**Avoid mixing text and images in a segmented control.** Although individual segments can contain text or images, mixing the two in a single control can lead to a disconnected and confusing interface.

**Position content appropriately in a custom segmented control.** If you change the background appearance of a segmented control, make sure content still looks good and doesn’t appear misaligned.

### How to use
1. Add a `SegmentedControl` to a `Window`
2. Add one or more `SegmentedControl` items by clicking on the `+` button on the right side of the selected `SegmentedControl` item into the layout area
3. Select the `SegmentedControl` item you want to configure and from the inspector change every property as requested
3. Open the `Code Editor` clicking the `View` ->  `Actions Panel`  -> `Code Editor` menu item
4. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`

![The 'Add' button where the user can add `SegmentedControl` items](images/segmentedcontrol5.png)
The 'Add' button where the user can add `SegmentedControl` items.

![The `SegmentedControl` inspector](images/segmentedcontrol2.png)
The inspector where the `SegmentedControl` can be configured.

![The `SegmentedControl` item inspector](images/segmentedcontrol3.png)
The inspector where the `SegmentedControl` item can be configured.

![The `Code Editor` where to interact with events and write custom code](images/segmentedcontrol4.png)
The `Code Editor` where to interact with events and write custom code.

#### Example
How to show an `Alert` via source code by selecting different `SegmentedControl` items.

1. Select `Item1` from the layout area
2. From the `Source Code` area select `Events` -> `Action`  and place the code below in he code editor
```
var alert = Alert("Title", "You have selected '" + Item1.title + "'")
alert.show()
```
3. Select `Item2` from the layout area
4. From the `Source Code` area select `Events` -> `Action`  and place the code below in he code editor
```
var alert = Alert("Title", "You have selected '" + Item2.title + "'")
alert.show()
```

### SegmentedControl most important properties
Several UI aspects can be configured in the `SegmentedControl` class but the `Momentary` is the most popular to be configured.
- Momentary: A Boolean value that determines whether segments in the receiver show selected state.

### SegmentedControlItem most important properties
Several UI aspects can be configured in the `SegmentedControlItem` class but the `Title` and `Image` are the most populars to be configured.
- `Title`: The title assigned to item. An Item can only have image or title, not both.
- `Image`: The image assigned to item. An Item can only have image or title, not both.
