This example assumes that you have a valid connection with a [Database](Database.html).
That DB database object should contain an **images** table (id int column as primary key and a data column as BLOB):
```
// INSERT EXAMPLE

// extract PNG data from and Image
var image = image1.PNGRepresentation();

// prepare database record
var rec = DatabaseRecord();
rec.bindInt("id", 1);
rec.bindData("data", image);

// insert record into table images
DB.addRecord(rec, "images");
if (DB.isError) Console.write(DB.errorMessage);
```

```
// UPDATE EXAMPLE

// extract PNG data from and Image
var image = image1.PNGRepresentation();

// prepare database record
var rec = DatabaseRecord();
rec.bindInt("id", 1);
rec.bindData("data", image);

// update record into table images WHERE id=1
DB.updateRecord(rec, "images", "id=1");
if (DB.isError) Console.write(DB.errorMessage);
```



