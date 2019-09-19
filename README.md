## Purpose 

Creates one sqlite database that is two database added, 
with identical schema.

**new_sqlite = master_sqlite + added_sqlite**

## Procedure

Copy one database schema and data to the copy.

After, read the second database adding rows.

To avoid overwrite unique keys, 

1) numbers: search for max previous key on database

2) strings: add a suffix to the key's value

Start from tables independent from other's tables keys, 
using foreign key property to parse relationships.

Apply transformation to the values on this firsts tables.

Afterwards, continue with tables that depend's on 
the tables just imported. Works one table after other, 
until every one is imported.

## Usage

Create the config.ini text file, 
specify the path of master database, appended database 
and the new database to create.


## To Do's

* Test, test, test

* Other types of data on keys, for example, keys that are timestamp or date.

* Avoid duplicate rows that has the same data.




