# What is a Schema?
A **database schema** is considered the "blueprint" of a database, describing how the data may relate to other tables or data models. It provides a logical and structural representation of the database without actually containing the data itself.

## Why do we use them?
There are several reasons why we use database schemas:

1. **Access and security:** Database schema design helps in organizing data into separate entities, making it easier to share a single schema within another database. Administrators can control access through database permissions, adding a layer of security for proprietary data. For example, personally identifiable information (PII) can be stored in a separate schema and encrypted for privacy and security.

2. **Organization and communication:** Documentation of database schemas allows for better organization and communication among stakeholders. It provides a common source of truth, enabling users to understand the logical constraints and methods of aggregation across tables.

3. **Integrity:** Database schemas help ensure data validity. They assist administrators in managing normalization processes to avoid data duplication. Schemas also help monitor compliance with the constraints in the database design, ensuring adherence to ACID properties (atomicity, consistency, isolation, durability).

# What are the different types of Database Keys?

## Primary Key
A **primary key** is a column or set of columns that uniquely identifies each row in a table. Every database table must have a primary key for data manipulation operations. Optim, the database management system, uses primary keys defined in the database. However, additional primary keys can be defined to supplement those in the database.

## Foreign Key
A **foreign key** is a field or collection of fields in one table that refers to the primary key in another table. It establishes a relationship between the two tables. The table with the foreign key is called the child table, while the table with the primary key being referenced is called the referenced or parent table. The foreign key constraint prevents actions that would destroy the links between the tables.

## Composite Key
A **composite key** is a key in a database that consists of two or more attributes (columns) together. The combination of these attributes can uniquely identify a tuple (row) in a table. Each attribute forming the composite key can also be a foreign key in its own right. It is also known as a compound key.

# What are Relationships in a Relational Database?

## 1:1 Relationship
In a relational database, relationships represent associations between entities. A **one-to-one relationship** is a relationship between two entities where each instance of one entity is associated with exactly one instance of the other entity. For example, an employee being issued an employee ID card. Each individual employee is assigned a unique ID card in the company.

## Many:Many Relationship
A **many-to-many relationship** is a relationship between two entities where each instance of one entity can be associated with multiple instances of the other entity, and vice versa. Many-to-many relationships can create uncertainty and duplications in data, potentially leading to incorrect query results. For example, multiple persons can use many banks, and each bank can have multiple customers.


