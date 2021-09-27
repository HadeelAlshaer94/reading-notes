# Code 301 - Intermediate Software Development
# Mongo and Mongoose

## five differences between SQL and NoSQL databases:

SQL | NoSQL
----|-----
SQL databases are primarily called as Relational Databases (RDBMS) |NoSQL database are primarily called as non-relational or distributed database
SQL databases are table based databases |NoSQL databases are document based, key-value pairs, graph databases or wide-column stores
SQL databases have predefined schema |NoSQL databases have dynamic schema for unstructured data
SQL databases are vertically scalable |NoSQL databases are horizontally scalable
SQL databases uses SQL ( structured query language ) for defining and manipulating the data |NoSQL database, queries are focused on collection of documents

### What kind of data is a good fit for an SQL database?
- SQL databases are not best fit for hierarchical data storage.

### Give a real world example.
- SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL

### What kind of data is a good fit a NoSQL database?
- NoSQL database fits better for the hierarchical data storage

### Give a real world example.
- database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb

### Which type of database is best for hierarchical data storage?
- NoSQL database

### Which type of database is best for scalability?
- SQL databases

![nosql](https://cdn.educba.com/academy/wp-content/uploads/2019/05/what-is-Nosql-database1.png)

## sql vs nosql 

### What does SQL stand for?
- SQL stands for Structured Query Language, and is a ubiquitous language used to interact with structured data in databases. It is a language most data practitioners—data engineers, data analysts, business analysts, and data scientists—use in their everyday work to converse with databases in a scalable and efficient manner.

### What is a realational database?
- A relational database is a type of database that stores and provides access to data points that are related to one another.

### What type of structure does a relational database work with?
- SQL
### What is a ‘schema’?
- The database schema is its structure described in a formal language supported by the database management system (DBMS). The term "schema" refers to the organization of data as a blueprint of how the database is constructed (divided into database tables in the case of relational databases).

### What is a NoSQL database?
- “NoSQL database”, they typically use it to refer to any non-relational database.
- NoSQL databases are databases that store data in a format other than relational tables.

### How does it work?
-  NoSQL databases can store relationship data—they just store it differently than relational databases do.
- NoSQL data models allow related data to be nested within a single data structure.
- related data doesn’t have to be split between tables.

![nosql](https://www.improgrammer.net/wp-content/uploads/2020/04/NoSQL-Database-Types.jpg)

### What is inside of a Mongo database?
- stores data in JSON like documents

### Which is more flexible - SQL or MongoDB? and why.
- MongoDB
- Its gives you the flexibility to evolve your data schema without modifying the existing data

### What is the disadvantage of a NoSQL database?
- 1- NoSQL databases are not good fit for complex queries
- 2- You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.
- 3- still not comparable and sable enough in high load and for complex transactional applications.
- 4- For some NoSQL database you still have to rely on community support,and only limited outside experts are available for you to setup and deploy your large scale NoSQL deployments. 