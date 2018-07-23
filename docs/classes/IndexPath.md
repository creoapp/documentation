# IndexPath

**super**: [Object](Object.md)

The IndexPath class represents the path to a specific node in a tree of nested array collections. Each index in an index path represents the index into an array of children from one node in the tree to another, deeper, node.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).

</ul>

### Properties

* **var** **item**: **[Int](../gravity/types.md)**
The second index of the tree of nested array collection. For example, the index number identifying the item in a CollectionView section. \(read-only\)

* **var** **row**: **[Int](../gravity/types.md)**
The second index of the tree of nested array collection. For example, the index number identifying the row in a TableView section. \(read-only\)

* **var** **section**: **[Int](../gravity/types.md)**
The index of the root array of nodes. For example, the index number identifying a section in a CollectionView or a TableView object. \(read-only\)

* **var** **length**: **[Int](../gravity/types.md)**
The number of indexes in the index path. \(read-only\)

</ul>

### Initializers

* **func** **IndexPath**(**item**: <strong>[Int](../gravity/types.md)</strong>, **section**: <strong>[Int](../gravity/types.md)</strong>)
Returns an index-path object initialized with the indexes of a specific item and section.

</ul>

### Methods

* **func** **index**(**position**: <strong>[Int](../gravity/types.md)</strong>): <strong>[Int](../gravity/types.md)</strong> 
The index at a particular node in the index path.

* **func** **indexPathByAddingIndex**(**index**: <strong>[Int](../gravity/types.md)</strong>): <strong>[IndexPath](IndexPath.md)</strong> 
Returns a new index path by adding the new index to the current indexes.

* **func** **indexPathByRemovingLastIndex**(): <strong>[IndexPath](IndexPath.md)</strong> 
Provides an index path with the indexes in the receiving index path, excluding the last one.

</ul>

</ul>

