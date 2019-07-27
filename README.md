# Cassandra Summary

By: Mostafa Ghadimi
At: WizeAnalytics @ SUT

## NoSQL Database types(Not Only Structured Query Language) 

- Key/value pair store
- Column-family store
- Document-based repository
- Graph database

### Key/value pair store Database

Each data item is represented as an attribute name, also a key, together with its value.

Internally, key/value pairs are stored in a data structure called hashmap. **Hashmap** is popular because it provides very good performance on accessing data.

Popular Examples: **Amazon Dynamo, Redis, Riak**

### Column-family store Database

A column in this context is __not equal__ to a column in a relational table. In the NoSQL world, a column is a data structure that contains a **key**, **value**, and **timestamp**. Because of timestamps they provide
optimized performance for queries over very large datasets.

Popular Examples: **Google BigTable, Apache Cassandra, HBase**

### Document-Based repository Databse

Document-based repository is designed for documents or semi-structured data. The basic unit of a document-based repository associates each key, a primary identifier, with a complex data structure called a document. A document can contain many different key-value pairs, or key-array pairs, or even nested documents.

Popular Examples: **MongoDB, CouchDB**

### Graph Database

Graph databases are designed for storing information about networks, such as a social network. A graph is used to represent the highly connected network that is composed of nodes and their relationships. The nodes and relationships can have individual properties.

Graph databases are particularly difficult to be scaled out with sharding because traversing a graph of the nodes on different machine does not provide a very good performance. It is also not a straightforward operation to update all or a subset of the nodes at the same time.

Popular Examples: **Neo4j, FlockDB**

