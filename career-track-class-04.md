PostgreSQL Joins
  1. PostgreSQL join is used to combine columns from one (self-join) or more tables based on the values of the common columns between related tables. The common columns are typically the primary key columns of the first table and foreign key columns of the second table. 
  2. PostgreSQL supports inner join, left join, right join, full outer join, cross join, natural join, and a special kind of join called self-join.
  
One-to-One:
  1. In systems analysis, a one-to-one relationship is a type of cardinality that refers to the relationship between two entities (see also entity–relationship model) A and B in which one element of A may only be linked to one element of B, and vice versa. In mathematical terms, there exists a bijective function from A to B. For instance, think of A as the set of all human beings, and B as the set of all their brains. Any person from A can and must have only one brain from B, and any human brain in B can and must belong to only one person that is contained in A.
  2. In a relational database, a one-to-one relationship exists when one row in a table may be linked with only one row in another table and vice versa. It is important to note that a one-to-one relationship is not a property of the data, but rather of the relationship itself.

One-to-Many:
  1. In systems analysis, a one-to-many relationship is a type of cardinality that refers to the relationship between two entities (see also entity–relationship model) A and B in which an element of A may be linked to many elements of B, but a member of B is linked to only one element of A. For instance, think of A as books, and B as pages. A book can have many pages, but a page can only be in one book.
  2. In a relational database, a one-to-many relationship exists when one row in table A may be linked with many rows in table B, but one row in table B is linked to only one row in table A. It is important to note that a one-to-many relationship is not a property of the data, but rather of the relationship itself.

Many-to-Many:
  1. In systems analysis, a many-to-many relationship is a type of cardinality that refers to the relationship between two entities[1] A and B in which A may contain a parent instance for which there are many children in B and vice versa. For example, think of A as Authors, and B as Books. An Author can write several Books, and a Book can be written by several Authors.
  2. In a relational database management system, such relationships are usually implemented by means of an associative table (also known as join table, junction table or cross-reference table), say, AB with two one-to-many relationships A -> AB and B -> AB. In this case the logical primary key for AB is formed from the two foreign keys (i.e. copies of the primary keys of A and B).
  3. In web application frameworks such as CakePHP and Ruby on Rails, a many-to-many relationship between entity types represented by logical model database tables is sometimes referred to as a HasAndBelongsToMany (HABTM) relationship.
  
