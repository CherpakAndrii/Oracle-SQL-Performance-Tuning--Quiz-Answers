# Oracle SQL Performance Tuning
## Coursera quiz answers

* [Understanding Necessity of SQL Tuning (100%)](https://github.com/CherpakAndrii/Oracle-SQL-Performance-Tuning--Quiz-Answers#understanding-necessity-of-sql-tuning)
* [Tracing Query Execution Techniques (100%)](https://github.com/CherpakAndrii/Oracle-SQL-Performance-Tuning--Quiz-Answers#tracing-query-execution-techniques)
* [Query Optimization - Indexes (100%)](https://github.com/CherpakAndrii/Oracle-SQL-Performance-Tuning--Quiz-Answers#query-optimization-indexes)

# Understanding Necessity of SQL Tuning
### 1. Char data type will take more disk space than Varchar data type.
* ***True***
* False

### 2. Internally From clause gets executed first in the select statement execution.
* ***True***
* False

### 3. For counting rows of table Select Count(*) is faster than select count(1)
* True
* ***False***

### 4. Having filters actuals rows of the table.
* True
* ***False***

### 5. The child table or transaction table has a high volume of records. This statement is true or false.
* ***True***
* False

### 6. Varchar data type is suitable for fixed length values. This statement is true or false.
* True
* ***False***

### 7. Having clause gets executed before the where clause. This statement is true or false.
* True
* ***False***

### 8. Which clause eliminates duplicates?
* Select Column List
* ***Group By***
* Having
* Order By

### 9. What happens if a numeric value is given as a parameter to the count function?
* ***It will show the count of rows***
* The select statement fails to execute

### 10. The Exists operator will understand____ type of value
* ***Boolean***
* Integer

### 11. The user does not have the privilege of select on a table. The user issues a select statement on that table. Which clause will throw error?
* Where
* Having
* ***From***
* Order By

### 12. The column alias can be used in_____
* ***Order By***
* Where
* Having
* Group By


# Tracing Query Execution Techniques
### 1. The output of Explain is stored in a table known as Plan_Table
* ***True***
* False

### 2. Explain Plan output may not practically be correct always.
* ***True***
* False

### 3. Checking SQL statement syntax is done while executing and not while compiling.
* True
* ***False***

### 4. Bind variable is session specific
* ***True***
* False

### 5. The sql statements Select * from Emp; and select * from emp; are same for hard parsing?
* Yes
* ***No***

### 6. To eliminate the hard parsing again what is used.
* Substitution Variable
* ***Bind Variable***
* PLSQL Package variable
* A Local PLSQL variable

### 7. -- The --- dynamic view is used to see the parsing details
* V$parse
* ***V$sql***

### 8. In which parsing the syntax of a sql statement is checked?
* Soft parse
* ***Hard Parse***

### 9. The____needs DBA privilege.
* ***AutoTrace***
* Explain Plan

### 10. Explain plan neither executes the query nor automatically queries the plan table.
* ***True***
* False

### 11. The heavy data loading has not happened. Some small volume of data is dumped in the tables. Only the indexing and structure is ready. Which is a good way to know the execution?
* AutoTrace
* ***Explain Plan***

### 12. For knowing the execution details Explain Plan is an initial activity to be done whereas AutoTrace is the activity to be done later
* ***True***
* False


# Query Optimization - Indexes
### 1. Bitmap index is the default type of index in Oracle
* True
* ***False***

### 2. A function-based index stores actual values of the column
* True
* ***False***

### 3. The composite index Is made up of more than one column.
* ***True***
* False

### 4. Indexing is done to avoid a Full Table Scan.
* ***True***
* False

### 5. Index is not required if the query is going to access 95% rows of the table.
* ***True***
* False

### 6. In the Auto trace output if Oracle shows that index is used then which keyword comes for the where clause column condition?
* ***Access***
* Filter

### 7. Which is the correct command to create a composite index?
* ***Create Index My_Index on T1(A, B);***
* Create Composite Index My_Index on T1(A, B);

### 8. In a Function-Based index_______can be called.
* Procedure
* ***Function***

### 9. If there is no where clause in the select statement, then a full table scan happens.
* ***True***
* False

### 10. In Oracle composite index can be created of how many columns?
* 8
* 16
* 64
* ***32***

### 11. If a column has foreign key, then which type of index is ideal for that column?
* B-Tree
* ***Bitmap***

### 12. If a column has a primary key, then which type of index is there for that column?
* B-Tree
* ***Bitmap***
