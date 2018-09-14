#### Iterate through each record
```
while (rs.hasRow) {
	// access the values for the current row of the recordset
	// in this example we print the value of the column 'id' for the current row
	Console.write("ID: \(rs.id)")
	rs.moveNext();
}
```
