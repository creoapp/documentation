**super**: **[Object](Object.md)**

A regular expression is a special text string for describing a search pattern. Usually this pattern is used by string searching algorithms for find or find and replace operations on strings, or for input validation.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Class Methods

* **func** **count**(**pattern**: **[String](../gravity/string.md)**, **string**: **[String](../gravity/string.md)**, **options**: **[Int](../gravity/int.md) = 0**): <strong>[Int](../gravity/int.md)</strong> 
Returns the number of matches of the regular expression within the specified string.

* **func** **search**(**pattern**: **[String](../gravity/string.md)**, **string**: **[String](../gravity/string.md)**, **options**: **[Int](../gravity/int.md) = 0**): <strong>[List](../gravity/list.md)</strong> 
Returns an array containing all the matches of the regular expression in the string.

* **func** **ranges**(**pattern**: **[String](../gravity/string.md)**, **string**: **[String](../gravity/string.md)**, **options**: **[Int](../gravity/int.md) = 0**): <strong>[List](../gravity/list.md)</strong> 
Returns an array containing all the ranges of the regular expression in the string.

* **func** **replace**(**pattern**: **[String](../gravity/string.md)**, **string**: **[String](../gravity/string.md)**, **template**: **[String](../gravity/string.md)**, **options**: **[Int](../gravity/int.md) = 0**): <strong>[String](../gravity/string.md)</strong> 
Returns a new string containing matching regular expressions replaced with the template string.



* None

