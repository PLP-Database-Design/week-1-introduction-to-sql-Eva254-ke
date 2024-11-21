# SQL Assignment Week 1


## *What You'll Need*
- A computer with internet access.
- A code editor (e.g., Visual Studio Code).
- MySQL Workbench or another SQL database environment.

---



## *Submission Instructions*
1. Answer every question below and put your responses in a file named `answers.md`
2. Push your completed `answers.md` file to your GitHub repository.
3. Submit the GitHub link for review.

---

## **Assignment Questions**

## 1. State and Explain the components of a DBMS(Database Management System)
A Database Management System (DBMS) is a software system that enables efficient management, storage, retrieval and organization of data in a database. It consists of several core components that work together to facilitate database operations.

The database itself is the structured collection of data organized into tables, records and fields for instance, a database may store information about employees, including their IDs, names and salaries. The DBMS software manages these databases and provides an interface for users or applications to interact with the data examples of such software include MySQL, PostgreSQL, Oracle DB and SQLite.

The query processor is an integral part of the DBMS, responsible for interpreting user queries is usually written in SQL and converting them into low-level instructions that the database engine can execute. For example, a query like `SELECT * FROM Employees WHERE Salary > 50000;` is processed by this component. Meanwhile, the storage manager handles the physical storage of data on disk ensuring data integrity and optimizing space through efficient file and buffer management techniques.

To ensure reliable and consistent operations, the transaction manager oversees transactions enforcing the ACID properties (Atomicity, Consistency, Isolation and Durability). This ensures that even if multiple users access the database simultaneously or a process is interrupted, data remains accurate and secure. Supporting this is the metadata which provides detailed information about the database's structure such as the schema of tables, data types and constraints.

Data access languages, primarily SQL, allow users to interact with the database. They include DML (Data Manipulation Language) for operations like `INSERT` and `UPDATE`, DDL (Data Definition Language) for schema related commands like `CREATE TABLE`, and DCL (Data Control Language) for managing permissions through commands like `GRANT` and `REVOKE`. These interactions are made user-friendly through a variety of interfaces, ranging from command-line tools for developers to graphical interfaces like MySQL Workbench or Oracle SQL Developer for non-technical users.

At the heart of the DBMS is the database engine which performs the actual work of executing queries, managing indexing and handling data consistency. Complementing this is the security manager which enforces authentication and authorization rules to control user access and protect sensitive data. For example, it ensures that only authorized personnel can modify critical records such as payroll information.

In summary, a DBMS integrates multiple components, including the database, query processor, storage and transaction managers, metadata, database engine and security mechanisms all working together to ensure data is effectively managed, accessible, and secure.
## 2. What is a relational database? Give 4 examples.
A relational database is a type of database that organizes data into tables consisting of rows and columns. Each table represents a specific entity such as customers or products with rows holding individual records and columns representing the attributes of those records. The structure is highly organized allowing data to be related across different tables through the use of primary keys and foreign keys. This approach ensures data integrity and allows for powerful data querying and manipulation using Structured Query Language (SQL).

Examples of relational databases include MySQL, an open-source system widely used in web development and PostgreSQL a feature-rich open-source database known for its extensibility. Oracle Database is another example, designed for large-scale enterprise applications offering robust performance and scalability. Microsoft SQL Server is also a popular choice, providing comprehensive solutions for data management and business intelligence. Relational databases are used in various fields to manage and retrieve structured data efficiently.

## 3. State and Explain three classifications of SQL?

   SQL (Structured Query Language) can be classified into three main types based on the operations it performs: Data Definition Language (DDL), Data Manipulation Language (DML) and Data Control Language (DCL). DDL focuses on defining and modifying the structure of a database such as creating, altering or deleting tables and other database objects. For example, the `CREATE TABLE` statement defines a new table while `ALTER` modifies an existing table structure.

DML is used to interact with and manipulate the data within the database. It includes operations such as inserting new records, updating existing data, deleting records and retrieving data. Commands like `INSERT`, `UPDATE`, `DELETE` and `SELECT` fall under this category. For instance, a query like `SELECT * FROM Employees WHERE Salary > 50000;` retrieves all employees earning more than 50,000.

DCL deals with access control and permissions in the database, ensuring data security by granting or revoking user privileges. Commands like `GRANT` and `REVOKE` are used to manage user access. For example, the command `GRANT SELECT ON Employees TO user1;` allows user1 to view data from the Employees table. These classifications provide a structured and comprehensive way to manage database operations effectively.

## 4. What is the difference between a Primary Key and a Foreign Key?
   
A Primary Key is a unique identifier for each record in a table. It ensures that every row in the table is distinct and its values cannot be NULL or duplicate for example, in an `Employees` table, `EmployeeID` might be the primary key because it uniquely identifies each employee. Each table can have only one primary key although it can consist of a single column or a combination of columns (a composite key).

A Foreign Key, on the other hand, is a field or combination of fields in one table that refers to the Primary Key in another table. It is used to establish a relationship between two tables, ensuring referential integrity by linking the data in the related tables. For example, a `DepartmentID` in the `Employees` table might be a foreign key referencing the `DepartmentID` primary key in the `Departments` table. This connection ensures that each employee is assigned to a valid department.


## 5. What is an Entity-Relationship Diagram?
   An Entity-Relationship Diagram (ERD) is a visual representation of the data and relationships within a database. It is a tool used in database design to model the structure of data and the connections between different entities making it easier to understand the organization and flow of information.

In an ERD, entities represent the real-world objects or concepts e.g., `Customer`, `Order` and `Product` that need to be stored in the database. Each entity is depicted as a rectangle and contains attributes which are the specific details or properties of that entity e.g., `CustomerName`, `OrderDate`, `ProductPrice).

Relationships define how entities are connected to one another and are represented by diamonds or lines. For example, a `Customer` entity may have a "places" relationship with an `Order` entity, indicating that customers place orders. The relationships can also describe the cardinality e.g., one-to-one, one-to-many or many-to-many, specifying how many instances of one entity are associated with instances of another.

Attributes are often shown as ovals connected to their corresponding entities and key attributes such as primary keys are typically underlined to distinguish them. ERDs are essential for designing a clear, logical database schema and ensuring that relationships between data are correctly modeled before actual implementation.

## 6. What are the advantages of relational databases?
    Relational databases offer several advantages. They ensure data integrity through features like ACID compliance and data normalization. They are highly flexible and scalable allowing for easy modifications and handling large amounts of data. Security is a key strength, with robust features like user authentication, access controls and encryption. Relational databases also excel in data retrieval and analysis, thanks to powerful SQL queries and the ability to handle complex data relationships. Finally, they are user-friendly and well-established making them easy to manage and widely supported.

## 7. State four types of data type used to store data in tables?
    Integer: Stores whole numbers e.g., 1, 2, -5, 100.
Float or Real: Stores decimal numbers e.g., 3.14, 2.718, -0.5.
String or Text: Stores textual data e.g., "Hello, world!", "This is a string".
Boolean or Logical: Stores true or false values e.g., True, Fals).
   
## 8. What is the purpose of a database management system (DBMS)?
    A Database Management System (DBMS) is a software application that interacts with end-users, other applications and the database itself to capture and analyze data.

 Its primary purpose is to efficiently store, manage and retrieve data. It ensures data integrity, security and provides a user-friendly interface for data interaction.   









*How to edit a [markdownfile](https://www.markdownguide.org/basic-syntax/#headings)*

###  NOTE: You should not fork the repository
