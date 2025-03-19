# Introduction to MongoDB

MongoDB is a NoSQL database that stores data in a flexible, JSON-like format called BSON (Binary JSON).

Unlike traditional relational databases, it does not use tables, rows, or a fixed schema. Instead, it stores data as 
**documents** inside **collections**, making it highly scalable and adaptable to various applications.

An example of a document:

```JavaScript
{
  "_id": "65a3c1d2e9b21",
  "name": "Dennis",
  "age": 25,
  "email": "dennis@example.com",
  "skills": ["JavaScript", "React", "MongoDB"]
}
```

## SQL vs NoSQL Databases

Databases can be categorized into two: **relational/SQL databases** and **non-relational/NoSQL databases**.

<note>
SQL databases are relational databases (RDBMS) that use Structured Query Language (SQL) for defining and manipulating 
data.

They require predefined schemas to determine the structure of the data before working with it. This makes SQL databases
suitable for structured data and complex queries
</note>

<note>
NoSQL databases on the other hand don't use Structured Query Language for defining and manipulating data.

They can be document-oriented, column-oriented, graph-based, or organized as key-value stores. This flexibility 
allows for the creation of documents without a defined structure, making NoSQL databases suitable for handling 
large amounts of unstructured data
</note>

## Installing MongoDB
You need to install MongoDB and the Mongo shell.

Mongo shell is a mongo client that will allow you to interact with the mongodb server.

You also need to install the mongodb compass, which is the GUI of mongodb.

[Follow the steps outlined in this video](https://www.youtube.com/watch?v=gB6WLkSrtJk)

## MongoDB Terminologies
- **Database**: A MongoDB database is used to store and manage a set of collections. It consists of various collections, 
indexes, and other essential data structures required to store the data efficiently.
- **Collection**: A collection in MongoDB is a group of documents. The name of a collection must be unique within its 
database. Collections can be viewed as the table equivalencies in a relational database.
- **Document**: A document is a record in a MongoDB collection. It is comprised of a set of fields, similar to a row in 
a relational database. However, unlike tables in a relational database, no schema or specific structure is enforced 
on the documents within a collection.
- **Field**: A field in MongoDB is a key-value pair inside a document. It can store various types of data, including 
strings, numbers, arrays, and other documents. Fields in MongoDB can be seen as columns in a relational database.
- **Index**: Indexes in MongoDB are data structures that improve the speed of common search operations. They store 
a small portion of the dataset in a well-organized structure. This structure allows MongoDB to search and sort 
documents faster by reducing the number of documents it has to scan.
- **Query**: A query in MongoDB is used to retrieve data from the database. It retrieves specific documents or subsets 
of documents from a collection based on a given condition.
- **Cursor**: A cursor is a pointer to the result set of a query. It allows developers to process individual documents 
from the result set in an efficient manner.
- **Aggregation**: Aggregation in MongoDB is the process of summarizing and transforming the data stored in collections. 
It is used to run complex analytical operations on the dataset or create summary reports.
- **Replica Set**: A replica set in MongoDB is a group of mongodb instances that maintain the same data set. It provides 
redundancy, high availability, and automatic failover in case the primary node becomes unreachable.
- **Sharding**: Sharding is a method of distributing data across multiple machines. It is used in MongoDB to
horizontally scale the database by partitioning the dataset into smaller, more manageable chunks called shards.