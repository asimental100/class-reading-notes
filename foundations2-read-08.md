SQL (Structured Query Language) = a language designed to allow both technical and non-technical user query, manipulate and transform data from a relational detabase. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.
  1. Relational Databases - represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.
  2. To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned.
  3. Select query with contraints syntax below:
     SELECT column, another_column, …
     FROM mytable
     WHERE condition
        AND/OR another_condition
        AND/OR …;
  4. When an ORDER BY clause is specified, each row is sorted alpha-numerically based on the specified column's value. In some databases, you can also specify a collation to better sort data containing international text.
  5. SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.
  
Overall the sqlbolt.com and the w3 editiors are very helpful (and frustrating at times) in helping me get a better unserstanding of SQL but, I definitely need to spend more time playing around with them when I'm less brain dead. 
