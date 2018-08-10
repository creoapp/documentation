#### Connect the database
```
func onSuccess(db) {
    // code to execute when the connection completes
}

func onError(db) {
    // code to execute in case of connection error
}

MyDatabase.connect(onSuccess, onConnectionError)
```

#### Execute an INSERT statement (with explicit closures)
How to execute a SQL INSERT statement, the code to execute when the statement completes or fails is defined in the <code>onSuccess</code> and <code>onError</code> <a href="../gravity/closure.html">closures</a>.
```
func onSuccess(db) {
    // code to execute when the connection when the connection completes
    Console.write("INSERT: Success")
}

func onError(db) {
    // code to execute when the connection when the connection completes
    Console.write("INSERT: Error \(db.errorMessage)")
}

var sql = 'INSERT INTO MyTable (Column1,Column2) VALUES ("value1","value2")'
MyDatabase.execute(sql, onSuccess, onError);
```

#### Execute an INSERT statement (with anonymous closures)
This is another way to execute the same SQL statement of the previous example. In this case we use two anonymous <a href="../gravity/closure.html">closures</a>.
```
var sql = 'INSERT INTO MyTable (Column1,Column2) VALUES ("value1","value2")'
MyDatabase.execute(sql, {Console.write("INSERT: Success")}, {Console.write("INSERT: Error \(MyDatabase.errorMessage)")});
```

#### Execute a SELECT statement
How to make a query and use the returned RecordSet (sample from the <a href="../technotes/new-dataset-in-each-row.html">New DataSet in each row</a> technote). 
```
func onSuccess(db,rs) {
    // The sender Database is the first argument of the closure.
	// The new RecordSet is the second argument of the closure,
    // it can be used, for example, to set the dataSet property of a control
    // (for example a Table, a Chart, ecc.)
    cell.CustomView1.Chart1.dataSet = rs
    cell.CustomView1.Chart1.reload(false)
}

func onError(db) {
	// The sender Database is the first argument of the closure,
    // it can be used to get the errorMessage
    cell.CustomView1.Chart1.dataSet = null
    cell.CustomView1.Chart1.reload(false)
    Console.write("Error: \(db.errorMessage)")
}

var sql = 'SELECT Total FROM main."invoices" where CustomerId = \(cell.identifier)'
MyDatabase.select(sql, onSuccess, onError)
```

#### Make sure the Database is connected and then execute an SQL statement
How to execute a SQL statement, in this case an INSERT, but first make sure the Database is connected otherwise the execution will fail. Using the onSuccess and onError closures for each database method call guarantees that each database operation is performed in a background thread so that the app remains responsive even if the operation is time-consuming.
```
// This closure will be called when the database completes its connection,
// now I can execute my SQL statement
func onConnectionSuccess(db) {
    // Here you can customize the SQL statement
    var sql = 'INSERT INTO MyTable (Column1,Column2) VALUES ("value1","value2")'

    // Log the last inserted row if the SQL statement is executed
    func onExecuteSuccess(db) {
        Console.write("MyDatabase did execute '\(sql)' successfully. Last inserted row \(db.lastInsertedRowID).")
    }

    // Show an alert if the execution ends with an error
    func onExecuteError(db) {
        var alert = Alert("MyDatabase execute error","\(db.errorCode) \(db.errorMessage)")
        alert.show()
    }

    // Perform the SQL statement
    MyDatabase.execute(sql, onExecuteSuccess, onExecuteError);
}

// Show an alert if the connection fails
func onConnectionError(db) {
  var alert = Alert("MyDatabase connection error","\(db.errorMessage)")
  alert.show()
}

// Connect the database and then run the onConnectionSuccess closure when connected.
// If the database is already connected then the onConnectionSuccess closure is
// immediately executed.
MyDatabase.connect(onConnectionSuccess, onConnectionError)
```
