# Hash Table

A **hash table** is a data structure which stores data in an associative manner. In a hash table, data is stored in an array format, where each data value has its own unique index value. Access of data becomes very fast if we know the index of the desired data.
Thus, it becomes a data structure in which insertion and search operations are very fast irrespective of the size of the data. Hash Table uses an array as a storage medium and uses hash technique to generate an index where an element is to be inserted or is to be located from.

The **Hash table** data structure stores elements in key-value pairs where:

- **Key**: A unique integer that is used for indexing the values.
- **Value**: Data that is associated with keys.

## Hashing

**Hashing** is a technique to convert a range of key values into a range of indexes of an array. We're going to use modulo operator to get a range of key values. Consider an example of hash table of size 20, and the following items are to be stored. Items are in the (key,value) format.

# Hash Collision

When the hash function generates the same index for multiple keys, there will be a conflict (what value to be stored in that index). This is called a **hash collision**.

We can resolve the hash collision using one of the following techniques:

## 1. Collision Resolution by Chaining

## 2. Open Addressing
   - Linear Probing
   - Quadratic Probing
   - Double Hashing

## Why Hash Tables
Hash tables are a fundamental data structure used in computer science and programming. They operate by storing data in key-value pairs, where each key serves as a unique integer used for indexing associated values. Hash tables offer several advantages:

- **Fast Retrieval:** Hash tables provide fast data retrieval, thanks to their ability to quickly locate values based on keys.

- **Efficient Insertion and Deletion:** They efficiently handle insertion and deletion operations, typically performing them in constant time when given the key.

- **Flexibility:** Hash tables can store various data types as values, making them adaptable for diverse applications.

- **Memory Efficiency:** They dynamically adjust their size, minimizing memory wastage.

- **Useful for Frequent Element Checks:** They are particularly valuable for applications that involve frequent element existence checks.

