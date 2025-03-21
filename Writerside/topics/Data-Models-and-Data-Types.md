# Data Models and Data Types

In MongoDB, data is stored in BSON format, which supports various data types.

Understanding these data types is essential as they play a crucial role in schema design and query performance.

## BSON vs JSON
In MongoDB, data is stored in a binary format called BSON (Binary JSON), which is a superset of JSON 
(JavaScript Object Notation).

While both BSON and JSON are used to represent data in MongoDB, they have some key differences.

### JSON
JSON is a lightweight and human-readable data representation format that can be easily parsed and generated by many 
programming languages.

It is used widely as a medium for transmitting data over the web. Some features of JSON include:
- **Human readable**: JSON is textual with a simple structure, making it easy for humans to read and write.
- **Interoperable**: JSON can be easily parsed and generated by many different programming languages, making it 
a popular choice for data interchange between applications.
- **Limited Data Types**: JSON supports fewer data types compared to BSON, such as strings, numbers, booleans, and null. 
This means that some data, like dates or binary data, must be represented as strings or custom objects in JSON.

### BSON
BSON is a binary-encoded serialization of JSON-like documents.

<note>
When we say that BSON is binary encoded, we mean that data is stored in a format that computers can process more 
efficiently than plain text. Instead of being stored as human-readable text (like JSON), BSON converts the data into 
a series of bytes (binary format), which makes storage and retrieval faster.
</note>

It is designed to be efficient in storage, traversability, and encoding/decoding.

Some of its key features include:

- **Binary Encoding**: BSON encodes data in a binary format, which offers better performance and allows the storage 
of data types not supported by JSON.
- **Support for Additional Data Types**: BSON supports more data types compared to JSON, such as `Date`, `Binary`, 
`ObjectId`, and `Decimal128`. This makes it possible to represent diverse data more accurately in MongoDB documents.