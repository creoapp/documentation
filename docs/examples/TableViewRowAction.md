```
// How to programmatically add a create a new TableViewRowAction:

// create the new row action with a style and a title
var newAction = TableViewRowAction(TableViewRowActionStyle.Destructive,"Title");

// if you want to set an image to be shown instead of the title
// only available on iOS 11.0 or higher
// newAction.image = // you image here;

// add the closure that will be called if the action is selected
var closure = func(TableViewCell, section, index) { 
	// your code here
	Console.write("newAction \(index)");	
} 
newAction.bind("Action",closure);

// add the new action to the cell array of actions (left o right)
cell.leftActions = [newAction];
```

