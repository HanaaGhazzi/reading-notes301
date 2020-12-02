# Database Normalization

**Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.**

### Reasons for Database Normalization

1. to minimize duplicate data
2. to minimize or avoid data modification issues
3. to simplify queries. 

### Duplicated information presents two problems:

- It increases storage and decrease performance.
- It becomes more difficult to maintain data changes.



__First Normal Form__ – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
__Second Normal Form__ – The table is in first normal form and all the columns depend on the table’s primary key.
__Third Normal Form__– the table is in second normal form and all of its columns are not transitively dependent on the primary key.