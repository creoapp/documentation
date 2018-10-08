A database is a collection of informations organized so that they can be easily accessed, updated and deleted.
Data is organized into rows, columns and tables, and it is indexed to make it faster to find relevant information. Data gets updated, expanded and deleted as new informations are added.

### Supported databases
_Creo_ supports connection to relational databases such as `SQLite`, `MySQL` and `Postgres` and provide specific tools to easily create and test queries.

The common companion of an application is usually an `SQLite` database to benefit from locally stored data that does not require a connection to an external resource like a `MySQL` or `Postgres` servers.

### Database connections

![Database connect](images/Database_connect.png)

A new database connection is created dragging a database _Object_ from the bottom left _Objects_ view to _Project_ -> _Globals_.
Then using the _Inspector_ is possible to configure the database specific properties and _Test_ the connection.

### SQLite extra properties
`SQLite` databases are files distributed with the application, they may be associated with an _Assets file_ and can configued to be:
* **read-only** (default option), the DB is opened from the application bundle and can not be modified.
* **persistent on a file**, the original provided DB is _copied once_ to a writeable folder and then opened.
* **in-memory**, the DB is lost when the application quits.

When it comes to SQLite databases _Creo_ provides an extra tool to create tables and rows.

Tap _DB Configurator_ from the database _Inspector_ panel to open the tool.

![Database connect](images/Database_create.png)

The tool is not limited to creating rows and tables but can also be used to setup constraints as well:
* by pressing the T button next to a table name.
* by pressing the constraints buttons next to a field name.

**Note:** a table primary key could be set using both ways but just one is needed. In case of miss configurations a yellow _Warning sign_ is show at the top, click on it to read the problem's description.

### Database queries and dataset
For all supported databases, _Creo_ provides a tool to create and test static SQL queries.
Query can also be created from code when they depend from user inputs or other parameters.

Using the UI a new SQL query is created by tapping the (+) button of a database.

![Database connect](images/Database_query.png)

**Note:** to help writing correct queries the tool supports dragging fields from the left pane to the right pane.

In _Creo_ any database query is also a `Dataset` and can be used as an input to populate any UI control that require one. 

For instance, controls like `TableView`, `CollectionView` and `PageProvider` all requires a `Dataset`.

### Gravity code
Gravity can be used to interact with the database; you can use a query object created with the UI or write plain sql.

### Using Gravity with an UI generated query
Let's say you have a database named `SQLite1` and a query named `users`.

From Gravity `SQLite1.users` is an object of type [RecordSet](../classes/RecordSet.html)

to run the query and wait for the result you have to _bind_ the `DidFinish` event of the object:

```
var finish = {
    Console.write("Did Finish fired")
    while (SQLite1.users.hasRow) {
        Console.write("ID: \(SQLite1.users.id)")
        SQLite1.users.moveNext()
    }
}

SQLite1.users.bind("DidFinish", finish)
SQLite1.users.run()
```

Binding by code is not mandatory, you can also write the code directly in the code editor:

1. Open the `Code Editor` (cmd + 6)
2. Select the `DidFinish` item inside the `Events` area and write your custom code in the `Code Editor`

![Database finish](images/Database_didfinish.png)

**Note:** anytime you call `run` on a query, all controll that use that as a dataset gets refreshed.

**Beware, `run` is an async call:** sometimes you may be tempted to write:

```
SQLite1.users.run()
while (SQLite1.users.hasRow) {
        Console.write("ID: \(SQLite1.users.id)")
        SQLite1.users.moveNext()
}
```

unfortunately this is an **error** and is not guaranteed to work; `run` is an asynchronous call and the _while condtion_ will most of the time return _false_ if executed just after `run`. The proper way is to _bind_ to the `DidFinish` event and execute any logic from there.

#### RecorSet

`RecordSet` has several methods and provides an easy way to change the plain sql code too:

```
SQLite1.users.sql = "select * from users where name = 'nicola'"
SQLite1.users.run()
```

it also offers a convenient way to access the row result by their column's name, ie in this case the table _users_ has 3 columns, _id_, _name_ and _surname_:

```
...
Console.write("ID: \(SQLite1.users.id)")
Console.write("Name: \(SQLite1.users.name)")
Console.write("Surname: \(SQLite1.users.surname)")
...
```

where `SQLite1` is the dabatase, `users` is the query and `id` `name` `surname` are the column's name.

### Using Gravity with custom sql
Let's say you have an `SQLite` database named `SQLite1` with a table named `users`.

For reference in _Gravity_ the database object is of type [SQLiteDatabase](../classes/SQLiteDatabase.html) and we start by connecting to the database.

There are 2 way to connect to a database:

1. Synchronus, the connection waits until the attempt succeed or fails
1. Asynchronus, the function returns immediately and a callback is called to signal success or failure

Both ways use the method `connect`

Synchronus, no parameters

```
if (SQLite1.connect() == true) {
    Console.write("Connected")
} else {
    Console.write("Error connecting")
}
```

Asynchronus, we also pass 2 params that are the functions called when the connection attemp complete.

```
var onSuccess = func(db) {
    Console.write("Connected")
}

var onError = func(db) {
    Console.write("Error: \(db.errorMessage)")
}

SQLite.connect(onSuccess, onError)
```

Once the connection is estabilished, we can run a _select_ with `select` or an update / insert with `execute`.
Both methods works like the connect, they accept one parameter with the plain sql and eventually two functions called when the execution ends.

Synchronous
```
var sql = "SELECT * FROM users"
var recordSet = SQLite1.select(sql)
...
```

Asynchronous
```
var onSuccess = func(db, recordSet) {
    ...
}

var onError = func(db, recordSet) {
    Console.write("Error: \(db.errorMessage)")
}

var sql = "SELECT * FROM users"
SQLite1.select(sql, onSuccess, onError)
```
