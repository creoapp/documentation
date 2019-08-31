**super**: **[Database](Database.md)**

CubeSQL is an object-relational database management system based on sqlite.

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

* **var** **username**: **[String](../gravity/string.md)**
Username required for access to the database.

* **var** **password**: **[String](../gravity/string.md)**
Password that is required for access to the database.

* **var** **hostname**: **[String](../gravity/string.md)**
Database host name or IP address of the database server.

* **var** **port**: **[Int](../gravity/int.md)**
The port to use to connect to the database server.

* **var** **password**: **[String](../gravity/string.md)**
Database password.

* **var** **database**: **[String](../gravity/string.md)**
Database name.

* **var** **url**: **[String](../gravity/string.md)**
Database url.

* **var** **affectedRows**: **[Int](../gravity/int.md)**
Returns the number of rows modified, inserted or deleted by the most recently completed INSERT, UPDATE or DELETE statement. Executing any other type of SQL statement does not modify the value returned by this function. \(read-only\)

* **var** **lastInsertedRowID**: **[Int](../gravity/int.md)**
Returns the rowid of the most recent successful INSERT into a rowid table. \(read-only\)

* **var** **errorCode**: **[Int](../gravity/int.md)**
Returns a numeric error code if the latest sql operation failed. \(read-only\)

* **var** **encryption**: **[Int](../gravity/int.md)**
Use this property to set an encryption database connection.

* **var** **isError**: **[Bool](../gravity/bool.md)**
Check if latest operation failed. \(read-only\)

* **var** **errorMessage**: **[String](../gravity/string.md)**
Returns an error message if the latest sql operation failed. \(read-only\)

* **var** **isConnected**: **[Bool](../gravity/bool.md)**
A flag that checks if database is connected. \(read-only\)

* **var** **useSchema**: **[Bool](../gravity/bool.md)**
A flag to check if current database engines supports schemas. \(read-only\)

* **var** **objectName**: **[String](../gravity/string.md)**
The name of the object.



### Methods

* **func** **connect**(**onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [Bool](../gravity/bool.md)</strong> 
Connect to the specified database. The optional <code>onSuccess</code> and <code>onError</code> closures can be used to execute the statement in a background thread so that the app remains responsive. The <code>onSuccess</code> closure, if set, is executed when the connection ends without errors. The <code>onError</code> closure, if set, is executed when the connection fails. The Database object is passed as the only argument in both closures. If at least one of the closures is set then the connection is executed in the UI thread (not recommended for time-consuming tasks) and this method immediately returns <code>false</code>; otherwise, the statement is executed in the UI thread (not recommended for time-consuming tasks) and the method returns <code>true</code> in case of success, <code>false</code> in case of failure.

* **func** **select**(**sql**: **[String](../gravity/string.md)**, **onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [CubeSQLRecordSet](CubeSQLRecordSet.md)</strong> 
Perform a SQL query. The optional <code>onSuccess</code> and <code>onError</code> <a href="../gravity/closure.html">closures</a> can be used to perform the query in a background thread so that the app remains responsive. The <code>onSuccess</code> closure, if set, is executed when the query ends without errors; this closure is invoked with two arguments: the Database itself and the produced <a href="RecordSet.html">RecordSet</a>. The <code>onError</code> closure, if set, is executed when the query fails and the Database object is passed as the only argument. If at least one of the closures is set then the query is executed in a background thread and this method immediately returns a <code>null</code> value; otherwise, the query is executed in the UI thread (not recommended for time-consuming tasks) and the method returns the produced <a href="RecordSet.html">RecordSet</a> in case of success, <code>null</code> in case of failure. The query fails if the Database is not connected.

* **func** **execute**(**sql**: **[String](../gravity/string.md)**, **onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [Bool](../gravity/bool.md)</strong> 
Execute a INSERT, UPDATE, DELETE SQL statement. The optional <code>onSuccess</code> and <code>onError</code> closures can be used to execute the statement in a background thread so that the app remains responsive. The <code>onSuccess</code> closure, if set, is executed when the statement ends without errors. The <code>onError</code> closure, if set, is executed when the statement fails. The Database object is passed as the only argument in both closures. If at least one of the closures is set then the statement is executed in a background thread and this method immediately returns <code>false</code>; otherwise, the statement is executed in the UI thread (not recommended for time-consuming tasks) and the method returns <code>true</code> in case of success, <code>false</code> in case of failure. The execution of the statement fails if the Database is not connected.

* **func** **schemas**(**onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [CubeSQLRecordSet](CubeSQLRecordSet.md)</strong> 
Retrieve a list of database schemas. The optional <code>onSuccess</code> and <code>onError</code> closures can be used to execute the request in a background thread so that the app remains responsive. The <code>onSuccess</code> closure, if set, is executed when list of schemas is retrieved without errors; this closure is invoked with two arguments: the Database itself and the produced <a href="RecordSet.html">RecordSet</a>. The <code>onError</code> closure, if set, is executed when the operation fails and the Database object is passed as the only argument of the closure. If at least one of the closures is set then the request is executed in a background thread and this method immediately returns a <code>null</code> value; otherwise, the statement is executed in the UI thread (not recommended for time-consuming tasks) and the method returns the produced <a href="RecordSet.html">RecordSet</a> in case of success, <code>null</code> in case of failure. The request fails if the Database is not connected.

* **func** **tables**(**onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [CubeSQLRecordSet](CubeSQLRecordSet.md)</strong> 
Retrieve a list of database tables. The optional <code>onSuccess</code> and <code>onError</code> closures can be used to execute the request in a background thread so that the app remains responsive. The <code>onSuccess</code> closure, if set, is executed when list of schemas is retrieved without errors; this closure is invoked with two arguments: the Database itself and the produced <a href="RecordSet.html">RecordSet</a>. The <code>onError</code> closure, if set, is executed when the operation fails and the Database object is passed as the only argument of the closure. If at least one of the closures is set then the request is executed in a background thread and this method immediately returns a <code>null</code> value; otherwise, the statement is executed in the UI thread (not recommended for time-consuming tasks) and the method returns the produced <a href="RecordSet.html">RecordSet</a> in case of success, <code>null</code> in case of failure. The request fails if the Database is not connected.

* **func** **tablesWithSchema**(**schema**: **[String](../gravity/string.md)**, **onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [CubeSQLRecordSet](CubeSQLRecordSet.md)</strong> 
Retrieve a list of database tables within the specified schema. The optional <code>onSuccess</code> and <code>onError</code> closures can be used to execute the request in a background thread so that the app remains responsive. The <code>onSuccess</code> closure, if set, is executed when list of schemas is retrieved without errors; this closure is invoked with two arguments: the Database itself and the produced <a href="RecordSet.html">RecordSet</a>. The <code>onError</code> closure, if set, is executed when the operation fails and the Database object is passed as the only argument of the closure. If at least one of the closures is set then the request is executed in a background thread and this method immediately returns a <code>null</code> value; otherwise, the statement is executed in the UI thread (not recommended for time-consuming tasks) and the method returns the produced <a href="RecordSet.html">RecordSet</a> in case of success, <code>null</code> in case of failure. The request fails if the Database is not connected.

* **func** **columnsForTableAndSchema**(**table**: **[String](../gravity/string.md)**, **schema**: **[String](../gravity/string.md)**, **extended**: **[Bool](../gravity/bool.md)**, **onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [CubeSQLRecordSet](CubeSQLRecordSet.md)</strong> 
Retrieve information about a given table in the specified schema. The optional <code>onSuccess</code> and <code>onError</code> closures can be used to execute the request in a background thread so that the app remains responsive. The <code>onSuccess</code> closure, if set, is executed when list of schemas is retrieved without errors; this closure is invoked with two arguments: the Database itself and the produced <a href="RecordSet.html">RecordSet</a>. The <code>onError</code> closure, if set, is executed when the operation fails and the Database object is passed as the only argument of the closure. If at least one of the closures is set then the request is executed in a background thread and this method immediately returns a <code>null</code> value; otherwise, the statement is executed in the UI thread (not recommended for time-consuming tasks) and the method returns the produced <a href="RecordSet.html">RecordSet</a> in case of success, <code>null</code> in case of failure. The request fails if the Database is not connected.

* **func** **addRecord**(**databaseRecord**: **[DatabaseRecord](DatabaseRecord.md)**, **table**: **[String](../gravity/string.md)**, **onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [Bool](../gravity/bool.md)</strong> 
Add DatabaseRecord to the current Database. The optional <code>onSuccess</code> and <code>onError</code> <a href="../gravity/closure.html">closures</a> can be used to perform the query in a background thread so that the app remains responsive.

* **func** **updateRecord**(**databaseRecord**: **[DatabaseRecord](DatabaseRecord.md)**, **table**: **[String](../gravity/string.md)**, **whereClause**: **[String](../gravity/string.md)**, **onSuccess**: **[Closure](../gravity/closure.md) = null**, **onError**: **[Closure](../gravity/closure.md) = null**)<strong>: [Bool](../gravity/bool.md)</strong> 
Update current Database using values from DatabaseRecord class. The whereClause String parameter is used to determine which rows will be affacted bu the UPDATE statement. If all rows need to be update then pass "1". The optional <code>onSuccess</code> and <code>onError</code> <a href="../gravity/closure.html">closures</a> can be used to perform the query in a background thread so that the app remains responsive.

* **func** **close**()
Close connection to the database.

* **func** **escape**(**identifier**: **[String](../gravity/string.md)**)<strong>: [String](../gravity/string.md)</strong> 
Escape an identifier.





