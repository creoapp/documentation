**super**: [Database](Database.md)

SQLite is an embedded relational database management system. It is ACID-compliant and implements most of the SQL standard, using a dynamically and weakly typed SQL syntax. SQLite is a popular choice as embedded database software for local/client storage in application software such as web browsers. It is arguably the most widely deployed database engine, as it is used today by several widespread browsers, operating systems, and embedded systems (such as mobile phones), among others.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidConnect**()
Handle this event if you want to perform some operations when database is connected.

* **DidDisconnect**()
Handle this event if you want to perform some operations when database is disconnected.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **password**: **[String](../gravity/types.md)**
Database password.

* **var** **database**: **[String](../gravity/types.md)**
Database name.

* **var** **url**: **[String](../gravity/types.md)**
Database url.

* **var** **affectedRows**: **[Int](../gravity/types.md)**
Returns the number of rows modified, inserted or deleted by the most recently completed INSERT, UPDATE or DELETE statement. Executing any other type of SQL statement does not modify the value returned by this function. \(read-only\)

* **var** **lastInsertedRowID**: **[Int](../gravity/types.md)**
Returns the rowid of the most recent successful INSERT into a rowid table. \(read-only\)

* **var** **errorCode**: **[Int](../gravity/types.md)**
Returns a numeric error code if the latest sql operation failed. \(read-only\)

* **var** **secure**: **[Bool](../gravity/types.md)**
Use this property to set a secure database connection.

* **var** **isError**: **[Bool](../gravity/types.md)**
Check if latest operation failed. \(read-only\)

* **var** **errorMessage**: **[String](../gravity/types.md)**
Returns an error message if the latest sql operation failed. \(read-only\)

* **var** **isConnected**: **[Bool](../gravity/types.md)**
A flag that checks if database is connected. \(read-only\)

* **var** **useSchema**: **[Bool](../gravity/types.md)**
A flag to check if current database engines supports schemas. \(read-only\)



### Class Methods

* **func** **open**(**srcfile**: <strong>[Object](../gravity/types.md)</strong>): <strong>[Object](../gravity/types.md)</strong> 
Initializes and returns the SQLiteDatabase object with the content of the source file. The source file can be an URL or a <a href="File.html">File</a> object.



### Methods

* **func** **connect**(**onSuccess**: <strong>[Closure](../gravity/closures.md) = null</strong>, **onError**: <strong>[Closure](../gravity/closures.md) = null</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Connect to the specified database.

* **func** **select**(**sql**: <strong>[String](../gravity/types.md)</strong>, **onSuccess**: <strong>[Closure](../gravity/closures.md) = null</strong>, **onError**: <strong>[Closure](../gravity/closures.md) = null</strong>): <strong>[SQLiteRecordSet](SQLiteRecordSet.md)</strong> 
Perform a SQL query.

* **func** **execute**(**sql**: <strong>[String](../gravity/types.md)</strong>, **onSuccess**: <strong>[Closure](../gravity/closures.md) = null</strong>, **onError**: <strong>[Closure](../gravity/closures.md) = null</strong>): <strong>[Bool](../gravity/types.md)</strong> 
Execute a INSERT, UPDATE, DELETE SQL statement.

* **func** **schemas**(**onSuccess**: <strong>[Closure](../gravity/closures.md) = null</strong>, **onError**: <strong>[Closure](../gravity/closures.md) = null</strong>): <strong>[SQLiteRecordSet](SQLiteRecordSet.md)</strong> 
Retrieve a list of database schemas.

* **func** **tables**(**onSuccess**: <strong>[Closure](../gravity/closures.md) = null</strong>, **onError**: <strong>[Closure](../gravity/closures.md) = null</strong>): <strong>[SQLiteRecordSet](SQLiteRecordSet.md)</strong> 
Retrieve a list of database tables.

* **func** **tablesWithSchema**(**schema**: <strong>[String](../gravity/types.md)</strong>, **onSuccess**: <strong>[Closure](../gravity/closures.md) = null</strong>, **onError**: <strong>[Closure](../gravity/closures.md) = null</strong>): <strong>[List](../gravity/lists.md)</strong> 
Retrieve a list of database tables within the specified schema.

* **func** **columnsForTableAndSchema**(**table**: <strong>[String](../gravity/types.md)</strong>, **schema**: <strong>[String](../gravity/types.md)</strong>, **extended**: <strong>[Bool](../gravity/types.md)</strong>, **onSuccess**: <strong>[Closure](../gravity/closures.md) = null</strong>, **onError**: <strong>[Closure](../gravity/closures.md) = null</strong>): <strong>[List](../gravity/lists.md)</strong> 
Retrieve information about a given table in the specified schema.

* **func** **close**()
Close connection to the database.

* **func** **escape**(**identifier**: <strong>[String](../gravity/types.md)</strong>): <strong>[String](../gravity/types.md)</strong> 
Escape an identifier.





