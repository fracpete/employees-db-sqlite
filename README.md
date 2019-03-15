# employees-db-sqlite

This is an [SQLite](https://sqlite.org/) port of the 
[MySQL employees database](https://github.com/datacharmer/test_db).

Version: 1.0.6

## Where it comes from
The original data was created by Fusheng Wang and Carlo Zaniolo at Siemens
Corporate Research. The data is in XML format.
http://timecenter.cs.aau.dk/software.htm

Giuseppe Maxia made the relational schema and Patrick Crews exported the data
in relational format.

The database contains about 300,000 employee records with 2.8 million salary
entries. The export data is 167 MB, which is not huge, but heavy enough to be
non-trivial for testing.

The data was generated, and as such there are inconsistencies and subtle
problems. Rather than removing them, we decided to leave the contents
untouched, and use these issues as data cleaning exercises.

## Porting MySQL to SQLite

The MySQL data was ported using the [mysql2sqlite](https://github.com/dumblob/mysql2sqlite)
conversion tool.

## Database schema

A database schema can be found in the [MySQL documentation](https://dev.mysql.com/doc/employee/en/sakila-structure.html).

## Installation

* [download](https://raw.githubusercontent.com/fracpete/employees-db-sqlite/master/employees_db-full-1.0.6.db.gz) 
  the database
* decompress it: `gunzip employees_db-full-1.0.6.db.gz`
* open/access it with your favorite database tool (eg [DBeaver](https://dbeaver.io/))

## License
This work is licensed under the Creative Commons Attribution-Share Alike 3.0
Unported License. To view a copy of this license, visit
http://creativecommons.org/licenses/by-sa/3.0/ or send a letter to Creative
Commons, 171 Second Street, Suite 300, San Francisco, California, 94105, USA.
