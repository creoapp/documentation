```
// How to programmatically add a new item:

// create the new item
var newItem = SegmentedControlItem()
// set the title (or the image)
newItem.title = "Item Title"

// add the closure that will be called if the item is selected
var closure = func() { 
	// your code here	
} 
newItem.bind("Action",closure)

// add the new item to your SegmentedControl, in this case SegmentedControl1
SegmentedControl1.addItem(newItem)
```

