# Data-analytics-week-2

COMMON DATA STRUCTURE

Monday, 15 April 2024
09:27

STRUCTURED DATA
-Tabled
-stored in consistent, defined manner.
-organized into rows and columns.
All entries in a column contain the same type of value

UNSTRUCTURED DATA
-Qualitative, describes the characteristics of an event or an object.
-images, phrases, audio, video recordings and descriptive texts are examples of unstructured data.

SEMI STRUCTURED DATA
-It has a structure but it is not tabular. An example of a semi structured data is an email.

COMMON FILE FORMATS
TEXT FILE

Text files are widely used due to their ability to be opened on any platform without needing proprietary software. They are also known as flat files and are commonly used for storing machine-generated data like log entries. Delimiters, such as commas and tabs, separate data fields in structured text files. CSV files use commas as delimiters, while TSV files use tabs. Many software packages and coding languages support reading and writing delimited files, making it easy to work with structured data. Overall, text files are versatile and essential for storing and transmitting alphanumeric data in a variety of computing environments.

![image](https://github.com/NdiiLe/Data-analytics-week-2/assets/131252498/c2aeb8a4-8b39-4fff-9350-343deac77c3b)




DATABASES & DATA ACQUISITION
RELATIONAL DATABASE
Relational databases are pieces of software that let you make an operational system out of an ERD. You start with a relational model and create a physical design. Relational entities correspond to database tables, and entity attributes correspond to table columns. 
When creating a database table, the ordering of columns does not matter because you can specify the column order when retrieving data from a table. When an attribute becomes a column, you assign it a data type. Completing all of this work results in a diagram known as a schema. You can think of a schema as an ERD with the additional details needed to create a database.

NON RELATIONAL DATABASE
A nonrelational database does not have a predefined structure based on tabular data. The result is a highly flexible approach to storing data. However, the data types available in relational databases are absent. As a result, you need to know more about the data itself to interact with it. Data validation happens in code, as opposed to being done in the database. 
![image](https://github.com/NdiiLe/Data-analytics-week-2/assets/131252498/3f211695-b774-4a91-8425-0adc8103b7ce)

Examples of a none relational database are:

Key-Value
Document
Column-Family
Graph
![image](https://github.com/NdiiLe/Data-analytics-week-2/assets/131252498/d9e4ec12-75aa-443d-8a48-67133e29b181)


ONLINE TRANSACTIONAL PROCESSING

Wednesday, 17 April 2024
09:52


OLTP systems manage everyday transactions like flight reservations, online orders, and stock trades. They can handle high volumes of transactions, each involving small amounts of data, while efficiently reading and writing data.

NORMALIZATION

First normal form
-every row in a table is unique and every column contains a unique value

Second normal form
-takes from 1NF
-all nonprimary key values must depend on the entire primary key

Third normal form
-builds from 2NF
-adds a rule stating all columns must depend on only the primary key

ONLINE ANALYTICAL PROCESSING
OLAP systems focus on the ability of organizations to analyze data. While OLAP and OLTP databases can both use relational database technology, their structures are fundamentally different. OLTP databases need to balance transactional read and write performance, resulting in a highly normalized design. Typically, OLTP databases are in 3NF.
On the other hand, databases that power OLAP systems have a denormalized design. Instead of having data distributed across multiple tables, denormalization results in wider tables than those found in an OLTP database. It is more efficient for analytical queries to read large amounts of data for a single table instead of incurring the cost of joining multiple tables together.

SCHEMA CONCEPTS
The design of a database schema depends on its purpose, with normalized databases suitable for transactional systems and denormalized designs for analytical systems. Data warehouses aggregate data from various systems for analytics across an entire organization, while data marts focus on specific departmental needs. Data lakes store raw data in native formats, demanding additional knowledge for analytical utility. Relational databases enforce structure and business rules absent in data lakes. Design patterns for data warehouses and marts impact analytical efficiency, especially as data volume grows. Considerations like data source, frequency of changes, and persistence duration are vital in database schema life cycles. Creating a data mart within a data warehouse can cater to specific departmental analytics needs, such as analyzing employee trends in human resources.


![image](https://github.com/NdiiLe/Data-analytics-week-2/assets/131252498/cc203b61-9b8a-49bf-b086-a1bafe99bf29)



