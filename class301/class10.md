
Fill in the chart below with five differences between SQL and NoSQL databases:

# [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
SQL                                                                            NoSQL
1. Relational Databases                                                        1. non-Relational or distributed database
2. Table based databases                                                       2. document based, key-value pairs, graph databases wide-column stores.
3. predefined schema                                                           3. dynamic schema for unstructured data.
4. vertically scalable, scaled by increasing the horse-power of the hardware   4. horizontally scalable are scaled by increasing the databases servers in the pool of resources
5. structured query language                                                   5. ocused on collection of documents.
 	 
 	 
 	 
1. What kind of data is a good fit for an SQL database?
      * complex query intensive environment
2. Give a real world example.
      * netflix uses SQL
3. What kind of data is a good fit a NoSQL database?
      * hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data
4. Give a real world example.
      * storing large data files, real time anaytics and various web applications
5. Which type of database is best for hierarchical data storage?
      * NOSQL
6. Which type of database is best for scalability?
      * SQL 

## Videos
[ql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

1. What does SQL stand for?
      * Structured query language
2. What is a relational database?
      * A relational database is a type of database that organizes data into one or more tables, each consisting of a set of columns and rows. The columns represent the attributes or properties of the data, while the rows represent the individual instances or records of the data.
3. What type of structure does a relational database work with?
      * A relational database works with a structured data model in which data is organized into tables, also known as relations.

Each table in a relational database has a predefined set of columns or fields, which define the attributes or properties of the data, and a set of rows or records, which represent the individual instances of the data. The columns in one table can be linked or related to columns in another table through the use of primary and foreign keys.

This structure allows for efficient querying and manipulation of data, as well as the ability to ensure data integrity through the use of constraints such as unique, not null, and foreign key constraints.

The relational model has been widely adopted and is used in many popular database management systems, including MySQL, Oracle, Microsoft SQL Server, and PostgreSQL.
4. What is a ‘schema’?
        * In a relational database, a schema is a blueprint or plan that describes the structure of the database. It defines the tables, columns, relationships, and constraints that make up the database, as well as the rules and procedures for managing and manipulating the data.

A database schema is usually created by a database administrator or a developer and serves as a guide for other users who need to access or work with the database. It provides a clear understanding of the data model, which makes it easier to develop, test, and maintain the database.

In addition to defining the structure of the database, a schema can also include information about access control and security, such as user roles and permissions. Some database management systems also support multiple schemas, which allow different groups of users to work with different parts of the database.

5. What is a NoSQL database?
      * A NoSQL database is a non-relational database that uses a document-based or key-value data model instead of the traditional table-based structure used in relational databases.

Unlike relational databases, NoSQL databases do not use SQL for querying data and do not enforce the same level of data consistency and integrity as relational databases. This allows for more flexibility and scalability, as well as better performance when working with large volumes of data.

NoSQL databases are often used in web and mobile applications, where large amounts of unstructured data need to be stored and accessed quickly. They are also commonly used in big data and real-time data processing applications, where the speed of data processing is more important than data consistency.

Examples of popular NoSQL databases include MongoDB, Cassandra, Couchbase, and Redis.

6. How does it work?
      * NoSQL databases work by storing and retrieving data using a document-based or key-value data model, rather than the table-based structure used in relational databases.

In a document-based NoSQL database, data is stored in collections, which are similar to tables in a relational database. Each collection contains one or more documents, which are similar to records in a table. However, unlike relational databases, the structure of each document in a collection can be different, allowing for greater flexibility and scalability. Documents can be nested and contain arrays, making it easy to store complex data structures.

In a key-value NoSQL database, data is stored and retrieved using a unique key that identifies each piece of data. Each key-value pair is stored independently of other data, allowing for fast retrieval and storage of data.

NoSQL databases also typically provide features such as automatic sharding, which allows the database to scale horizontally across multiple servers, and eventual consistency, which allows for faster writes by not enforcing immediate consistency across all nodes in the database.

NoSQL databases are often used in applications where large amounts of unstructured or semi-structured data need to be stored and accessed quickly, such as web and mobile applications, big data processing, and real-time data analysis.
7. What is inside of a MongoDB database?
      * In a MongoDB database, data is stored in collections, which are analogous to tables in a relational database. Each collection can contain multiple documents, which are the equivalent of rows or records in a relational database.

MongoDB documents are JSON-like objects, which consist of key-value pairs and can be nested. The keys represent the field names or attributes of the data, while the values represent the data itself.

MongoDB also includes the concept of a "database," which is a logical container for collections. Each database can contain multiple collections, and each collection can have its own set of indexes and options.
8. Which is more flexible - SQL or MongoDB? and why.
      * In terms of flexibility, MongoDB is generally considered more flexible than SQL. This is because MongoDB uses a document-based data model that allows for more flexible and dynamic schemas compared to the rigid, tabular structure of SQL.

In a MongoDB database, documents can have different fields and structures, and there is no need to define a fixed schema before storing data. This allows for more agility and faster development, as changes to the data model can be made more easily without requiring changes to the database schema or application code.

In contrast, SQL databases enforce a rigid structure, requiring the definition of a fixed schema before data can be stored. While this can provide more data consistency and integrity, it can also be more difficult to change the schema once data has been stored, requiring migrations and updates to application code.
9. What is the disadvantage of a NoSQL database?
      * Limited query functionality: NoSQL databases generally do not support the full range of SQL queries, which can make it more difficult to analyze data and perform complex joins across different collections.

      * Limited transaction support: NoSQL databases typically do not support transactions with the same level of data consistency and isolation as relational databases, which can lead to data inconsistencies and conflicts in some use cases.

      * Lack of standardization: Unlike SQL databases, which have a well-established standard for querying and managing data, NoSQL databases have a more fragmented landscape with different data models and APIs, which can make it harder to switch between databases or integrate with other systems.

      * Limited tooling and community support: NoSQL databases often have less mature tooling and a smaller community of developers compared to SQL databases, which can make it harder to find resources and support for development and maintenance.
