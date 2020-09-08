Inside a Computer
  1. Motherboard: the computer's main circuit board. It's a thin plate that holds the CPU, memory, connectors for the hard drive and optical drives, expansion cards to control the video and audio, and connections to your computer's ports (such as USB ports).
  2. CPU (Central Processing Unit): is located inside the computer case on the motherboard. It is sometimes called the brain of the computer, and its job is to carry out commands. Whenever you press a key, click the mouse, or start an application, you're sending instructions to the CPU. The CPU fits into the motherboard's CPU socket, which is covered by the heat sink, an object that absorbs heat from the CPU. 
  3. RAM (Random Access Memory): Your computer system's short-term memory. This short-term memory disappears when the computer is turned off. If you're working on a document, spreadsheet, or other type of file, you'll need to save it to avoid losing it. When you save a file, the data is written to the hard drive, which acts as long-term storage.
  4. Hard Drive: where your software, documents, and other files are stored. The hard drive is long-term storage, which means the data is still saved even if you turn the computer off or unplug it.
  5. Power Supply Unit: converts the power from the wall outlet to the type of power needed by the computer. It sends power through cables to the motherboard and other components.
  6. Expansion Cards: These are sometimes called PCI (peripheral component interconnect) cards. You may never need to add any PCI cards because most motherboards have built-in video, sound, network, and other capabilities. However, if you want to boost the performance of your computer or update the capabilities of an older computer, you can always add one or more cards.

PostgreSQL INSERT
  1. The most basic syntax of the INSERT statement: INSERT INTO table_name(column1, column2, …) VALUES (value1, value2, …);
  2. The INSERT statement also has an optional RETURNING clause that returns the information of the inserted row. If you want to return the entire inserted row, you use an asterisk (*) after the RETURNING keyword
  
PostgreSQL SELECT
  1. The SELECTstatement has the following clauses:
    1.a. Select distinct rows using DISTINCT operator.
    1.b. Sort rows usingORDER BY clause.
    1.c. Filter rows using WHERE clause.
    1.d. Select a subset of rows from a table using LIMIT or FETCH clause.
    1.e. Group rows into groups using GROUP BY clause.
    1.f. Filter groups using HAVING clause.
    1.g. Join with other tables using joins such as INNER JOIN, LEFT JOIN, FULL OUTER JOIN, CROSS JOIN clauses.
    1.h. Perform set operations using UNION, INTERSECT, and EXCEPT.
  2. The following illustrates the syntax of the SELECT statement: SELECT select_list FROM table_name;

PostgreSQL UPDATE
  1. The PostgreSQL UPDATE statement allows you to modify data in a table. The following illustrates the syntax of the UPDATE statement: UPDATE table_name SET column1 = value1, column2 = value2, ... WHERE condition;
    1.a. The WHERE clause is optional. If you omit the WHERE clause, the UPDATE statement will update all rows in the table.
    1.b. The UPDATE statement has an optional RETURNING clause that returns the updated rows.

PostgreSQL DELETE
  1. The PostgreSQL DELETE statement allows you to delete one or more rows from a table. The following shows basic syntax of the DELETE statement: DELETE FROM table_name WHERE condition;
    1.a. The WHERE clause is optional. If you omit the WHERE clause, the DELETE statement will delete all rows in the table.
    1.b. The DELETE statement returns the number of rows deleted. It returns zero if the DELETE statement did not delete any row.
