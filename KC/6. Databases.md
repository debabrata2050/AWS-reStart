# Databases

## KC - Introduction to Databases

#### 1. What is a database?
- [ ] A collection of data that is organized into files called rows
- [x] A collection of data that is organized into tables ✅
- [ ] A collection of data that organized into files called datasets.
- [ ] A collection of data that is organized into files called columns

#### 2. Which database attributes accurately represent elements of a relational database? (Select TWO.)
- [ ] Forms
- [ ] Key-value pairs
- [x] Columns ✅
- [x] Tables ✅
- [ ] Horizontal scaling

#### 3. What are the primary features of a NoSQL database? (Select TWO.)
- [ ] NoSQL databases work well for customer relation management (CRM) applications or enterprise resource planning (ERP) applications.
- [x] NoSQL databases have a flexible schema. ✅
- [ ] NoSQL databases use vertical scaling.
- [x] NoSQL databases use data models that are not based on relational tables ✅
- [ ] NoSQL databases can run transactional or analytical queries.

#### 4. Which of the following is not a type of anomaly?
- [ ] Deletion anomaly
- [ ] Insertion anomaly
- [ ] Update anomaly
- [x] Structure anomaly ✅

#### 5. What is the primary benefit of using database as a service (DBaaS)?
- [ ] These databases increase the cost of installing and maintaining the servers.
- [ ] These databases are used for processing only small datasets.
- [x] These databases reduce the cost of installing and maintaining the servers. ✅
- [ ] These databases can be modified so that administrators can perform management tasks, such as server provisioning, patching, setup, configuration, backups, or recovery.

***

## KC - Data Interaction and Database Transaction

#### 1. A customer is ordering a product from an online retailer. If the payment for the transaction is successful, the Orders table must be updated so that a new order row is inserted. The stockTable table must also be updated so that product rows are removed for the purchased products. If one step fails, then all steps fail.

Which type of database transaction property does this scenario represent?
- [ ] Consistency
- [x] Atomicity ✅
- [ ] Durability
- [ ] Isolation

#### 2. The daily duties of database administrators include all of the following except which option?
- [x] Create different applications that can receive data ✅
- [ ] Use different SQL commands to interact with tables in databases
- [ ] Design, implement, administer, and monitor data in database systems
- [ ] Ensure consistency, quality, and security of the database

#### 3. What is a database transaction?
- [x] A transaction is the reproduction of one or more changes that are performed on a database. ✅
- [ ] A transaction is a web server running a webpage that gathers information from the server.
- [ ] A transaction is an application that is installed on the user computer or the application server.
- [ ] A transaction is an application written with Java that is used to embed SQL statements in the application code.

#### 4. What does the I in the term ACID compliance represent?
- [ ] The ability to ensure that any change will not violate the integrity of the database
- [ ] The ability to ensure that as soon as a transaction is committed, any interruption to database availability does not affect data consistency
- [x] The ability to concurrently process multiple transactions so that one transaction does not affect other transactions ✅
- [ ] The ability to ensure that all changes are successfully completed

#### 5. Which of the following options describes a successful transaction on a database?
- [x] A transaction on a database is successful if the transaction is committed. ✅
- [ ] A transaction on a database is successful if the transaction is active.
- [ ] A transaction on a database is successful if the transaction is partially committed.
- [ ] A transaction on a database is successful if the transaction is ended.

***

## KC - Creating Tables and Learning Different Data Types

#### 1. What is the purpose of data definition language (DDL) statements in structured query language (SQL)?
- [ ] They are used to view, change, and manipulate data in a table.
- [ ] They are used to control access to the data in a database.
- [ ] They are used to perform queries on the data in schema objects.
- [x] They are used to create and modify the structure of a database. ✅

#### 2. What is the function of the SELECT statement in structured query language (SQL)?
- [ ] Modify rows in a table
- [ ] Add or delete columns in a table
- [x] Retrieve data from a table ✅
- [ ] Revoke permissions from a user

#### 3. Which statement describes a foreign key?
- [x] It is a reference to a column in another table. ✅
- [ ] It enforces limits on the types of data that can go in a table.
- [ ] It includes words that structured query language (SQL) reserves and have predefined data types.
- [ ] It is a purposeful way to name objects or items in a database.

#### 4. Which statement defines referential integrity?
- [ ] Columns automatically have foreign key and primary key constraints.
- [ ] Rules and limitations are imposed by the database management system (DBMS).
- [x] Foreign key values must match an existing primary key value. ✅
- [ ] The primary key value matches an existing foreign key.

#### 5. What is the purpose of data manipulation language (DML) statements in structured query language (SQL)?
- [ ] They control access to the data in a database.
- [ ] They create and modify the structure of a database.
- [x] They are used to view, add, change, or delete data in a table. ✅
- [ ] They perform queries on the data within schema objects.

***

## KC - Inserting Data into a Database

#### 1. What is the most common use of a comma-separated values (CSV) file?
- [ ] To create and modify the structure of a database
- [x] To import data into or export data out of databases and spreadsheets ✅
- [ ] To remove a table definition and all the table data
- [ ] To delete records in an existing table

#### 2. What is the function of a NULL value in structured query language (SQL)?
- [ ] It is used to provide a description of the specified table or view.
- [ ] It is a constraint that forces a column to not accept NULL values.
- [x] It is used to represent a missing value. ✅
- [ ] It is a NULL value that represents a Boolean value.

#### 3. How is a comma-separated values (CSV) file validated before it is imported into a database?
- [ ] Confirm that values are enclosed with single quotation marks (' ') for character values or date values.
- [x] Confirm that the structure of the data in the file matches the number of columns in the table and the type of data in each column. ✅
- [ ] Verify that the information in the file is formatted in several columns.
- [ ] Confirm that each piece of information in the file is placed in a new row. Change every character in a string to lowercase.

#### 4. What is the purpose of the CONCAT function in structured query language (SQL)?
- [ ] It creates a substring with a specified length.
- [ ] It returns the number of rows in a table.
- [x] It combines strings from several columns and puts them together in one line. ✅
- [ ] It removes characters from the beginning and end of a string.

#### 5. What are two ways to use the INSERT INTO statement? (Select TWO.)
- [x] To add a new record to a table ✅
- [ ] To create a new table
- [x] To add new data to a database ✅
- [ ] To add new data to a table with a different number of headers
- [ ] To clean the data in a comma-separated values (CSV) file

***

## KC - Selecting Data from a Database

#### 1. Which statement describes the purpose of a WHERE clause in a SELECT statement?
- [ ] The WHERE clause uses a column identifier to organize the result-set data into groups.
- [ ] The WHERE clause sorts query results by one or more columns in either ascending or descending order.
- [x] The WHERE clause requests only specific rows from a table. ✅
- [ ] The WHERE clause provides an alias for each column or expression.

#### 2. Which clause is required to complete a SELECT statement?
- [ ] ORDER BY
- [x] FROM ✅
- [ ] HAVING
- [ ] GROUP BY

#### 3. Which term describes what the WHERE clause represents in the SELECT-FROM-WHERE statement?
- [ ] Operator
- [ ] Constraint
- [ ] Query
- [x] Condition ✅

#### 4. What does an asterisk (*) do in a structured query language (SQL) query?
- [ ] Select all keys
- [ ] Select all rows
- [ ] Select all tables
- [x] Select all columns ✅

#### 5. A database developer created a complex SELECT query. They want to ensure that other developers can understand each line in this query.
What is the correct way for the developer to create a single-line comment within the query?
- [ ] !--- comment ---
- [x] -- comment ✅
- [ ] /* comment */
- [ ] ## comment

***

## KC - Performing a Conditional Search

#### 1. Which logical operator selects values in a given range?
- [ ] AND
- [ ] LIKE
- [x] BETWEEN ✅
- [ ] SOME

#### 2. Which logical operator determines whether a specific character string matches a specified pattern?
- [ ] IN
- [ ] SOME
- [ ] WHERE
- [x] LIKE ✅

#### 3. What is the purpose of using aliases in structured query language (SQL) statements?
- [ ] Aliases create temporary names for constraints.
- [x] Aliases create temporary names for columns. ✅
- [ ] Aliases create temporary names for rows.
- [ ] Aliases create temporary names for queries.

#### 4. Consider the following structured query language (SQL) statement:
```sql
{
SELECT ID, Name, CountryCode
FROM city
WHERE Name SQL_OPERATOR 'c%'
}
```
Which structured query language (SQL) operator compares a value to similar values by using the wildcard operators?
- [ ] OR
- [ ] NOT
- [ ] IN
- [x] LIKE ✅

#### 5. Which value is tested for by the IS NULL condition in structured query language (SQL)?
- [ ] INT value
- [ ] Boolean value
- [ ] NOT NULL value
- [x] NULL value ✅

***

## KC - Working with Functions

#### 1. Which function calculates the number of rows in a table?
- [ ] MAX()
- [x] COUNT() ✅
- [ ] MOD()
- [ ] SUM()

#### 2. Which SELECT statement displays only the unique combinations of values of district and countrycode?
- [ ] SELECT ORDER BY district, countrycode FROM city;
- [x] SELECT DISTINCT district, countrycode FROM city; ✅
- [ ] SELECT UNIQUE district, countrycode FROM city;
- [ ] SELECT DIFFERENCE district, countrycode FROM city;

#### 3. Which string function removes the leading space on entries in a column?
- [x] LTRIM() ✅
- [ ] MOD()
- [ ] RTRIM()
- [ ] MIN()

#### 4. Which structured query language (SQL) function calculates the sum of a set of values or the sum of an expression?
- [ ] MAX
- [ ] COUNT
- [x] SUM ✅
- [ ] DIFFERENCE

#### 5. Which keyword is commonly used with individual columns to ensure that the retrieved column has unique values?
- [ ] UNIQUE
- [ ] ORDER BY
- [x] DISTINCT ✅
- [ ] DIFFERENCE

***

## KC - Organizing Data

#### 1. A database manager must sometimes aggregate data from different rows in a table. They must correlate the data into specified columns. Which clause should the manager use?
- [ ] ORDER BY
- [ ] HAVING
- [x] GROUP BY ✅
- [ ] WHERE

#### 2. Which operator can be used to filter query results after applying a GROUP BY clause?
- [x] HAVING ✅
- [ ] WHERE
- [ ] ORDER BY
- [ ] BETWEEN

#### 3. A database administrator must query a column that contains sequential dates. They want to see the output from their query in descending order. Which clause should the manager use with GROUP BY so that they can get results in descending order?
- [ ] ORDER BY column_name HAVING
- [x] ORDER BY column_name DESC ✅
- [ ] ORDER BY column_name ASC
- [ ] ORDER BY column_name WHERE

#### 4. A database developer wrote a query which includes the clause ORDER BY 3. What effect will this ORDER BY clause have on the structured query language (SQL) query?
- [ ] The query output will exclude data having a value of 3 for the third column in the SELECT clause of the SQL statement.
- [ ] The query output will be sorted by the third table in the FROM clause of the SQL statement.
- [ ] The query output will only include data having a value of 3 for the third column in the SELECT clause of the SQL statement.
- [x] The query output will be sorted by the third column in the SELECT clause of the SQL statement. ✅
 
#### 5. If a database developer wants to limit the output of a query to only those customers with sales that are more than 5,000 units, which structure query language (SQL) clause should they use?
- [ ] HAVING sales < 5000
- [ ] WHERE SUM(sales) > 5000
- [x] HAVING SUM(sales) > 5000 ✅
- [ ] GROUP BY SUM(sales) > 5000

***

## KC - Retrieving Data from Multiple Tables

#### 1. Which operator can be used to combine the results of two or more SELECT statements into a single set?
- [ ] HAVING
- [x] UNION ✅
- [ ] COUNT
- [ ] AVG

#### 2. Which structured query language (SQL) statement represents the correct way to create a qualified column name?
- [ ] table_name_column_name.
- [ ] .table_name_column_name
- [ ] column_name.table_name
- [x] table_name.column_name ✅

#### 3. A database administrator is working on a database. Two tables in the database contain important information that the administrator wants to query against. They want to display the matching values from both tables only if there are matching columns between the tables. Which clause should the administrator use?
- [ ] OUTER JOIN
- [ ] CROSS JOIN
- [ ] RIGHT JOIN
- [x] INNER JOIN ✅

#### 4. A database administrator is working on a database. Two tables in the database contain important information that the administrator wants to query against. They want to use a JOIN clause to retrieve all rows from the first table and all matching rows from the second table. Which clause should the administrator use?
- [ ] FULL OUTER JOIN
- [ ] OUTER JOIN
- [x] LEFT JOIN ✅
- [ ] RIGHT JOIN

#### 5. Which statement is used to create an alias so that the table name is not repeated twice in a self JOIN query?
- [x] AS ✅
- [ ] WITH
- [ ] ALIAS
- [ ] JOIN

***

## KC - Amazon RDS

#### 1. Which task can be automatically performed by Amazon Relational Database Service (Amazon RDS) or manually performed by a user?
- [ ] Hardware provisioning
- [ ] Database setup
- [ ] Operating system (OS) patching
- [x] Periodic backups ✅
 
#### 2. Which option must be specified first when creating a database (DB) instance in Amazon Relational Database Service (Amazon RDS)?
- [x] Choose the DB engine ✅
- [ ] Choose a DB instance identifier
- [ ] Connect to the DB instance
- [ ] Choose an Amazon Web Services (AWS) Region

#### 3. Which task is a best practice for high availability in an Amazon Relational Database Service (Amazon RDS) database (DB) instance?
- [ ] Creating a deployment within the same Amazon Web Services (AWS) Region
- [x] Deploying the DB instance in multiple Availability Zones (multi-AZ deployment) ✅
- [ ] Replicating the data six ways across three Availability Zones
- [ ] Deploying the DB instance in a single Availability Zone (single-AZ deployment)

#### 4. Which use case represents a reason for using Amazon Relational Database Service (Amazon RDS) instead of other database solutions?
- [ ] Simple GET or PUT requests and queries
- [ ] Relational database management system (RDBMS) customization
- [ ] Support for key-value and document data models
- [x] Complex transactions or complex queries ✅

#### 5. What is an Amazon Aurora database (DB) cluster?
- [x] An Aurora DB cluster consists of one or more DB instances and a cluster volume that manages the data for those DB instances. ✅
- [ ] An Aurora DB cluster consists of an Amazon Web Services (AWS) Region and two or one Availability Zones.
- [ ] An Aurora DB cluster consists of an instance endpoint and an one Amazon Web Services (AWS) Region.
- [ ] An Aurora DB cluster consists of a virtual private cloud (VPC), subnet, and security group.

***

## KC - Amazon DynamoDB

#### 1. Which type of database is Amazon DynamoDB?
- [ ] Hierarchical database
- [ ] Relational database
- [x] NoSQL database ✅
- [ ] In-memory database

#### 2. How does Amazon DynamoDB achieve high availability and scalability across Regions?
- [ ] By using a collection of multiple partition keys
- [ ] By using a collection of one or more attributes
- [x] By using a collection of multiple replica tables ✅
- [ ] By using a collection of multiple items

#### 3. Which statement describes the concept of partitioning in Amazon DynamoDB?
- [x] Partitioning is the allocation of storage for a table. ✅
- [ ] Each partition has a maximum size of about 10MB
- [ ] Partitioning is the manual replication of table across multiple Availability Zones within an AWS Region.
- [ ] As data grows, table data is partitioned and indexed by a composite key.

#### 4. Which statement about Amazon DynamoDB partition keys is true?
- [ ] A primary key is composed of two partition keys
- [x] Partition keys uniquely identify each item in the table. ✅
- [ ] No two items in a table can use the same partition keys.
- [ ] A table can have two partition keys.

#### 5. How many ways can Amazon DynamoDB retrieve data from a DynamoDB table?
- [ ] Three ways
- [ ] One way
- [x] Two ways ✅
- [ ] Four ways

***
