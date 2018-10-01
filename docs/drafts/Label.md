A label describes an onscreen interface element or provides a short message. Although people can’t edit labels, they can sometimes copy the content of labels. Labels can display any amount of static text, but are best kept short.

![Label](images/label1.png)

### Best practices
* **Keep labels legible.** Labels can include plain or styled text. If you adjust the style of a label or use custom fonts, be sure to not sacrifice legibility. It’s best to adopt Dynamic Type so your labels still look good when a user changes text size on their device.

### How to use
1. Drop a `Label` control from the object panel to a `Window`
2. Use the `Label Inspector` to customize its properties like `prop1`, `prop2`, and `prop3`

If you need to write code for Label:

3. Open the `Code Editor` (cmd + 6)
4. Select the `MAIN_ACTION_NAME_HERE` item inside the `Events` area and write your custom code in the `Code Editor`

![`Label` inspector](images/label2.png)
The inspector where the `Label` class can be configured.

### Example
A very simple example about Label. Sample code should be as simple as possible, a Console.write most of the time makes a lot of sense. DO NOT USE Control1.value if value is passed as parameter and in any case use self.value. DO NOT HARDCODE control's name otherwise you'll end up with NON PORTABLE CODE,
```
Console.write("Label value: \(self.value)")
```

### Most important properties
Several UI aspects can be configured in the `Label` class but the `PROP1`, `PROP2`, and `PROP3` are the most populars to be configured.
- `PROP1`: A PROP1 description.
- `PROP2`: A PROP2 description.
- `PROP3`: A PROP3 description.

### References
[Label class reference](../classes/Label.html) contains a complete list of properties and methods that can be used to customize a `Label` object.
