**super**: **[Object](../gravity/object.md)**

The IndexPath class represents the path to a specific node in a tree of nested array collections. Each index in an index path represents the index into an array of children from one node in the tree to another, deeper, node.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **item**: **[Int](../gravity/int.md)**
The second index of the tree of nested array collection. For example, the index number identifying the item in a CollectionView section. \(read-only\)

* **var** **row**: **[Int](../gravity/int.md)**
The second index of the tree of nested array collection. For example, the index number identifying the row in a TableView section. \(read-only\)

* **var** **section**: **[Int](../gravity/int.md)**
The index of the root array of nodes. For example, the index number identifying a section in a CollectionView or a TableView object. \(read-only\)

* **var** **length**: **[Int](../gravity/int.md)**
The number of indexes in the index path. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Constructors

* **func** **IndexPath**(**item**: **[Int](../gravity/int.md)**, **section**: **[Int](../gravity/int.md)**)
Returns an index-path object initialized with the indexes of a specific item and section.



### Methods

* **func** **index**(**position**: **[Int](../gravity/int.md)**)-> <strong>[Int](../gravity/int.md)</strong> 
The index at a particular node in the index path.

* **func** **indexPathByAddingIndex**(**index**: **[Int](../gravity/int.md)**)-> <strong>[IndexPath](IndexPath.md)</strong> 
Returns a new index path by adding the new index to the current indexes.

* **func** **indexPathByRemovingLastIndex**()-> <strong>[IndexPath](IndexPath.md)</strong> 
Provides an index path with the indexes in the receiving index path, excluding the last one.





