### BookHaven

##### ***Objective:***
The aim of this assignment is to apply the concepts of relational database design, normalization, and entity-relationship modeling to create an efficient and structured database for a bookstore management system, **"BookHaven."**

##### ***Problem statement:***
**"BookHaven"** is facing challenges in managing its extensive collection of books, author information, customer data, and transaction records. The current system has issues with data redundancy, inconsistency, and inefficient data retrieval. Your task is to design a relational database that addresses these problems while ensuring data integrity and ease of access.

##### **Task 1:**
* Design a normalized database schema for "BookHaven."
* Identify and create tables such as Books, Authors, Customers, and Transactions.
* Define columns for each table with appropriate data types and constraints.


##### **Expected Outcome:**
A well-structured database schema diagram or document outlining tables, columns, data types, primary keys, foreign keys, and any relevant constraints.

#### ***Database Schema Design for BookHaven:***
CUSTOMERS:
|PK | customer_id | INT AUTO_INCREMENT |  
| -------- | -------- | -------- |
| | first_name |VARCHAR (50) NOT NULL 
| | last_name|VARCHAR (50) NOT NULL |
| | email |VARCHAR (255) UNIQUE, NOT NULL |  
| | phone |VARCHAR (15) NOT NULL |
| | address |TEXT NULL |

BOOKS:
|PK | book_id | INT AUTO_INCREMENT |  
| -------- | -------- | -------- |
| | title |VARCHAR (255) NOT NULL 
|FK | author_id | INT |  
| | publish_date|DATE NULL |
| | genre |VARCHAR (100) NULL |  
| | price |DECIMAL(10,2) NOT NULL |

AUTHORS:
|PK | author_id | INT AUTO_INCREMENT |  
| -------- | -------- | -------- |
| | first_name |VARCHAR (50) NOT NULL 
| | last_name|VARCHAR (50) NOT NULL |
| | bio |TEXT NULL |  

TRANSACTIONS:
|PK | transaction_id | INT AUTO_INCREMENT |  
| -------- | -------- | -------- |
|FK | customer_id | INT |
| | transaction_date |DATE NOT NULL   
| | payment_method |VARCHAR(50) NOT NULL |  
| | total |DECIMAL(10,2) NOT NULL |
|FK | book_id | INT |


##### **Task 2:**
* Develop an ERD to visually represent the relationships between the tables in your schema.
* Highlight key relationships such as the link between Books and Authors, and Customers and Transactions.
* Use standard ERD notation to illustrate one-to-many and many-to-one relationships.


##### **Expected Outcome:**
A clear and detailed ERD that accurately reflects the relationships within the "BookHaven" database.

##### *ERD:*
![image showing ERD](ERDSS.jpg)




#### ***Tools used:***
*vs code*
*markdown extension*
[freeCodeCamp](https://www.freecodecamp.org/news/how-to-use-markdown-in-vscode/)
[draw.io](https://app.diagrams.net/) - used to make ERD, saved to device
