SQL Notes – Day 1 (Basics & Fundamentals)
🔹 What is SQL?

SQL (Structured Query Language) is used to interact with databases.

It allows you to create, read, update, and delete (CRUD) data.

Popular SQL databases: MySQL, PostgreSQL, Oracle, SQL Server, SQLite.

🔹 Key Concepts

Database → Collection of tables.

Table → Stores data in rows & columns.

Row (Record) → One entry in a table.

Column (Field) → Attribute/Property of the data.

🔹 Common Data Types
Data Type	Description
INT	Integer numbers
VARCHAR(n)	Variable-length string (up to n chars)
DATE	Stores date (YYYY-MM-DD)
BOOLEAN	True/False values
DECIMAL(p,s)	Numbers with precision (p) and scale (s)



🔹 Basic SQL Commands
1. Create Database
CREATE DATABASE school;

2. Use Database
USE school;

3. Create Table
CREATE TABLE students (
    student_id INT PRIMARY KEY,
    name VARCHAR(50),
    age INT,
    grade VARCHAR(10)
);

4. Insert Data
INSERT INTO students (student_id, name, age, grade)
VALUES (1, 'Vishnu', 21, 'A'),
       (2, 'Krishna', 22, 'B'),
       (3, 'Srikara', 20, 'A');

5. Select Data
SELECT * FROM students;


Fetches all rows & columns.

6. Update Data
UPDATE students
SET grade = 'A+'
WHERE student_id = 2;

7. Delete Data
DELETE FROM students
WHERE student_id = 3;
