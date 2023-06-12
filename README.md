# EXP 01 - CREATE A SQL QUERY PROGRAM TO FETCH THE "FIRST_NAME".

## AIM:

To create a sql query program yo fetch the "FIRST_NAME" from the worker table using alias name.

## SOFTWARE:

MYSQL PLATFORM.

## ALGORITHM:

1) Start by connecting to your database.
2) Formulate the SQL query:
      * Begin with the "SELECT" statement.
      * Specify the column you want to retrieve, in this case, "FIRST_NAME".
      * Specify the table from which you want to fetch the data.
3) Execute the SQL query.
4) Fetch the result set returned by the query.
5) Process the result set:
      * Iterate over the rows of the result set.
      * Access the value of the "FIRST_NAME" column for each row.
      * Perform any required operations on the fetched data.
6) Close the database connection

## PROGRAM:

```java

CREATE TABLE Worker (
  WORKER_ID INT NOT NULL PRIMARY KEY,
  FIRST_NAME CHAR(25),
  LAST_NAME CHAR(25),
  SALARY INT(15),
  JOINING_DATE DATETIME,
  DEPARTMENT CHAR(25)
);

INSERT INTO Worker(WORKER_ID, FIRST_NAME, LAST_NAME, SALARY, JOINING_DATE,DEPARTMENT) VALUES
  (001, 'Monika', 'Arora', 100000, '14-02-2009.00.00', 'HR'),
  (002, 'Niharika', 'Verma', 80000, '14-06-1109.00.00', 'Admin'),
  (003, 'Vishal', 'Singhal', 300000, '14-02-2009.00.00', 'HR'),
  (004, 'Amitabh', 'Singh', 500000, '14-02-2009.00.00', 'Admin'),
  (005, 'Vivek', 'Bhati', 500000, '14-06-11 09.00.00','Admin'),
  (006, 'Vipul', 'Diwan', 200000, '14-06-11 09.00.00','Account'),
  (007, 'Satish', 'Kumar', 75000, '14-01-20 09.00.00','Account'),
  (008, 'Geetika', 'Chauhan', 90000, '14-04-1109.00.00', 'Admin');

SELECT FIRST_NAME AS WORKER_NAME from Worker;

```
## OUTPUT:
<img width="174" alt="sql e1 " src="https://github.com/divvisha/FETCH-FIRST-NAME-EXP1/assets/127508123/13a4e483-adbe-4767-9736-6b03706e3310">

## RESULT:

Thus a SQL query is created to fetch data from table using alias name.
