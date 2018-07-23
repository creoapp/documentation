# Preferences

**super**: [DataSet](DataSet.md)

A Preferences object lets you manage persistent app's preferences in a convenient key/value form.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidStart**()
Event raised when DataSet started retrieving data.

* **NewValue**(**value**: <strong>[Object](../gravity/types.md)</strong>)
Event raised when a new value becomes available.

* **DidFinish**()
Event raised when DataSet finished retrieving data.

* **DidFail**()
Event raised in case of DataSet error.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).

</ul>

### Methods

* **func** **read**(**key**: <strong>[String](../gravity/types.md)</strong>): <strong>[Object](../gravity/types.md)</strong> 
Reads the value specified by a previously saved key.

* **func** **write**(**key**: <strong>[String](../gravity/types.md)</strong>, **value**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether the specified key/value entry has been succesfully written to app's preferences. Accepts and writes properly Map, List, Int, Float, String, Bool and Null objects.

* **func** **reset**()
Removes all the preferencies set by the user. After calling this method, the <i>read</i> method will return the default values for the keys specified in the Preferences panel (Main menu -> Project -> Preferences). To just reset the value of single key, you can use the <i>write</i> method with null value.

</ul>

</ul>

