# SQL vs NoSQL

https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool

- SQL are primarily referred to as RDBMS - Relational Databases. SQL are table based. Scaled by increasing the power of hardware.

- NoSQL are non-relational. These are document based, key, value pairs, graph DBs, or wide column stores. Scaled my amount of DBs. Good fit for complex queries and hierarchical data storage.

- Mongo is a NoSQL DB. Stores data in documents similar to JSON. Non-relational and has dynamic schema. Written in C++.

- Mongo is good for Speed - handles simple queries well, gives data in a single doc. **A document DB**

- Scalability - Horizontally scalable.

- Manageable - Easy to use.

- Dynamic schema - Flexibility to change your data schema without impacting your previously existing data in storage.

# NoSQL modeling

https://highlyscalable.wordpress.com/

- Key-Value storage - simple yet powerful. Poor applicabilty in cases of key ranges. Ordered kay value pair takes care of this. 

- Ordered Key Value - powerful - 

- Big-Table - maps out your data. Columns, column families, timestamps, etc.

- Graph DBs - originated from the Ordered K/V pairs - 

- NoSQL requires a good understanding of data structures and algorithms. 

- MongoDB - document based.

- Denormalization - copying the same data in multiple docs. (MongoDB)

- Schema-less in doc-based DBs. Aggregation is more flexible and better performance.

- Joins - usually hinders query times by aggegation, embedding nested entries.

- Geohash is reducing a size of a large file by flattening it into a list of entries.

- Index table - big table - very simple index table containing the information. Can retireve information with a single specified query.

- Composite key index - beneficial when used with ordered keys. Multidimensional index. Allows us to iterate through the data by a search.

- Aggregation with composite keys - also by used for grouping as well as indexes. The information will return collocated, that is the idea behind this.

- Inverted search - Direct aggregation - data processing pattern, less of data modeling. Use of a index to find data that meets a certain criteria.

- Hierarchical Techniques - Tree Aggregation - Your typical tree structure. Searching maybe a little more difficult. 

- Adjacency lists - each node is an independent record and contains arrays of parents and children.

- Materialized Paths - A parent/child structure. Able to list all parents and children.

- Nested Sets - used in modeling a tree-like structures. Store leafes of the tree into an array an map the non-leaf nodes and putting them in an index showing start and end.

- Nested Documents Flattening - Basically indexing everything to avoid errors in search queries. Be more specific with naming. Good for search engines.

- Batch graph processing - Storing large maops is inefficent since large maps do not scale well. Reducing them allows for more efficiency. 

[code301 Reading Notes](/301/code301Table.md)