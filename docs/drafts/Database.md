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

### Database queries and dataset
For all supported databases, _Creo_ provides a tool to create and test static SQL queries.

A new SQL query is created by tapping the (+) button of a database.

![Database connect](images/Database_query.png)

**Note:** to help writing correct queries the tool supports dragging fields from the left pane to the right pane.

In _Creo_ any database query is also a `Dataset` and can be used as an input to populate any UI control that require one. For instance, controls like `TableView`, `CollectionView` and `PageProvider` all requires a `Dataset`.

### Databases and Gravity code

TODO