A collection manages an ordered set of content, such as a set of photos, and presents it in a customizable and highly visual layout. Because a collection doesn’t enforce a strictly linear format, it’s particularly well-suited to displaying items that vary in size. Generally speaking, collections are ideal for showing off image-based content. Backgrounds and other decorative views can optionally be implemented to visually distinguish subsets of items.
Collections support both interactivity and animation. By default, you can tap to select, touch and hold to edit, and swipe to scroll. If your app requires it, more gestures can be added for performing custom actions. Within a collection, animations can be enabled whenever items are inserted, deleted, or reordered, and custom animations are also supported.

![CollectionView](images/collectionview1.png)

### Best practices
* **Avoid creating radical new designs when a standard row or grid layout is sufficient.** A collection should enhance the user experience, not become the center of attention. Make it easy to select an item. If it’s hard to tap an item in your collection, people will get frustrated and lose interest before reaching the content they want. Use adequate padding around content to keep the layout clean and prevent overlapping of content.
* **Consider using a table instead of a collection for text.** It’s generally simpler and more efficient to view and digest textual information when it’s displayed in a scrollable list.
* **Use caution when making dynamic layout changes.** The layout of a collection can be changed at any time. If you dynamically change the layout while people are viewing and interacting with it, be sure the change makes sense and is easy to track. Unmotivated layout changes can make your app seem unpredictable and difficult to use. If context is lost due to a layout change, people are likely to feel like they’re no longer in control.

### How to use
1. Drop a `CollectionView` control from the object panel to a `Window`
2. Use the `CollectionView Inspector` to customize its properties like `Layout Type`, `Template`, `DataSet`, `KeyPath`, and `Allows Selection`

If you need to write code for CollectionView:

3. Open the `Code Editor` (cmd + 6)
4. Select the `DidSelectCell` item inside the `Events` area and write your custom code in the `Code Editor`

![`CollectionView` inspector](images/collectionview2.png)
The inspector where the `CollectionView` class can be configured.

### How to customize
The `CollectionView` can be customized by tapping the subnode icons (+).

![`CollectionView` customizations](images/collectionview3.png)
The `CollectionView` customizations.

### CollectionViewCell
A `CollectionViewCell` for placement on a `CollectionView` that can be configured by dropping a control like `ImageView` and `Label`.

![`CollectionView` cell](images/collectionview4.png)
The `CollectionView` cell.

### How to use
1. Select the `CollectionView Custom Cell` from the layout panel
2. Drop a control from the object panel to the custom `View` like the `ImageView` and `Label`

![`CollectionView` cell](images/collectionview5.png)
The `CollectionView` cell.

### Example
1. Drop a `CameraRoll` control from the object panel to a `Window`
2. Drop a `Button` control from the object panel to a `Window`
3. Open the `Code Editor` (cmd + 6)
4. Select the `Action` item inside the `Events` area and write your custom code in the `Code Editor`
```
CollectionView1.dataSet = CameraRoll1
CollectionView1.reload(true)
```

### Most important properties
Several UI aspects can be configured in the `CollectionView` class but the `layoutType`, `itemSize`, `allowsSelection`, `dataSet`, and `keyPath` are the most commons to be configured.
- `layoutType`: A PROP1 description.
- `itemSize`: A PROP2 description.
- `allowsSelection`: A PROP3 description.
- `dataSet`: A PROP3 description.
- `keyPath`: A PROP3 description.

### References
[CollectionView class reference](../classes/CollectionView.html) contains a complete list of properties and methods that can be used to customize a `CollectionView` object.
