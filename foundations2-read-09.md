A join operation allows you to retrieve data from multiple tables in a single SELECT query. Two tables can be joined by a single join operator, but the result can be joined again with other tables. There must exist a same or similar column between the tables being joined.

Inner JOIN: This is the simplest, most understood Join and is the most common. This query will return all of the records in the left table (table A) that have a matching record in the right table (table B).

Left JOIN: This query will return all of the records in the left table (table A) regardless if any of those records have a match in the right table (table B). It will also return any matching records from the right table.

Right JOIN: This query will return all of the records in the right table (table B) regardless if any of those records have a match in the left table (table A). It will also return any matching records from the left table.

Outer JOIN: This Join can also be referred to as a FULL OUTER JOIN or a FULL JOIN. This query will return all of the records from both tables, joining records from the left table (table A) that match records from the right table (table B).

Outer Exlcuding JOIN: This query will return all of the records in the left table (table A) and all of the records in the right table (table B) that do not match. I have yet to have a need for using this type of Join, but all of the others, I use quite frequently.

Data Normalization: is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.

First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.

Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.

Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key
