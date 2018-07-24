**super**: [DataSet](DataSet.md)

A FileManager object lets you examine the contents of the file system and make changes to it. A file manager object is typically your primary mode of interaction with the file system. You use it to locate, create, copy, and move files and directories. You also use it to get information about a file or directory or change some of its attributes.

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



### Methods

* **func** **open**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>, **mode**: <strong><a href="#_enum_FileMode">FileMode</a> = 0</strong>): <strong>[File](File.md)</strong> 
Opens the specified file using the optional file mode and returns a File object.

* **func** **directory**(**SearchPath**: <strong><a href="#_enum_SearchPath">SearchPath</a></strong>): <strong>[String](../gravity/types.md)</strong> 
This method is intended to locate known and common directories in the system.

* **func** **appendPath**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>, **component**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Creates a new path appending component path (second parameter) to the source path (first path).

* **func** **exists**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether the specified file exists on the underline file system.

* **func** **copy**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>, **destFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Copies the src file at the specified URL to a new location. Returns true if the file was copied successfully.

* **func** **move**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>, **destFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Moves the src file at the specified URL to a new location. Returns true if the file was copied successfully.

* **func** **delete**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Deletes file passed as paramerer. Returns true if the file was deleted successfully.

* **func** **createDirectory**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Creates a directory at the specified URL. Returns true if the directory was created successfully.

* **func** **createFile**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>, **content**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Creates a file with the specified content at the specified URL. Returns true if the operation was successful.

* **func** **isReadable**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether the specified file appears to be readable.

* **func** **isWritable**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether the specified file appears to be writable.

* **func** **isExecutable**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether the specified file appears to be executable.

* **func** **isDeletable**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether the specified file appears to be deletable.

* **func** **isDirectory**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value that indicates whether the specified file is a directory.

* **func** **contentsOfDirectory**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[List](../gravity/lists.md)</strong> 
Returs a List of url that contains all the files/folders inside the specified directory.

* **func** **readData**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[Data](data.md)</strong> 
Returns a Data value that contains the content of the file specified as parameter.

* **func** **readString**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Returns a String value that contains the content of the file specified as parameter.

* **func** **name**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Returns a String that contains file name.

* **func** **extension**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Returns a String that contains file extesion.

* **func** **path**(**sourceFilePath**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Returns a String that contains file full path.





### Enumeration

#### FileMode
 * .Read
 * .Update
 * .Write

<br><br>#### SearchPath
 * .ApplicationSupport
 * .Assets
 * .Bundle
 * .Caches
 * .Documents
 * .Inbox
 * .Temp

<br><br>

