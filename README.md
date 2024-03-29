# Oracle SQL Performance Tuning
## Coursera quiz answers - 100%

* [Understanding Necessity of SQL Tuning (100%)](https://github.com/CherpakAndrii/Oracle-SQL-Performance-Tuning--Quiz-Answers#understanding-necessity-of-sql-tuning)
* [Tracing Query Execution Techniques (100%)](https://github.com/CherpakAndrii/Oracle-SQL-Performance-Tuning--Quiz-Answers#tracing-query-execution-techniques)
* [Query Optimization - Indexes (100%)](https://github.com/CherpakAndrii/Oracle-SQL-Performance-Tuning--Quiz-Answers#query-optimization---indexes)
* [Performance Tuning Tools and Techniques (100%)](https://github.com/CherpakAndrii/Oracle-SQL-Performance-Tuning--Quiz-Answers#performance-tuning-tools-and-techniques)

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


# Performance Tuning Tools and Techniques
### 1. The temporary table gets auto refreshed if data from a table is copied into it, and the source table gets changed.
* True
* ***False***

### 2. Temporary table’s data by default get deleted on commit.
* ***True***
* False

### 3. We have redundant formula to be used in several new formula-based columns. What would be the best way of doing it?
* Use a temporary table
* ***Use an inline view***

### 4. Can we give multiple hints to the Oracle optimizer?
* ***Yes***
* No

### 5. In peak hours the records of the main tables get locked. What can be done to access those records even in the peak hours?
* Create Inline Views
* ***Add those records in a temporary table before peak hour***

### 6. An index is not getting used. What can we do so that the index gets used?
* Create a Temporary Table
* Create an Inline View
* ***Provide a hint***

### 7. We can drop the inline view.
* True
* ***False***

### 8. While creating the temporary table which keyword comes before the word temporary?
* Private
* ***Global***

### 9. Hints are not orders but directives
* ***True***
* False

### 10. Hints are provided in the ______
* Single quotes
* ***Comment formats***

### 11. Hints cannot be given by a Developer, but they can be given by a DBA only.
* True
* ***False***

### 12. In case of an inline view, we need to define a sub query after the from clause.
* ***True***
* False

### 13. CTE can be referred in the subsequent select statements in the from clause.
* ***True***
* False

### 14. Materialized View is a Virtual Table
* True
* ***False***

### 15. You need system level privilege to create and use a CTE
* True
* ***False***

### 16. MViews are inherently read only
* ***True***
* False

### 17. Any non-DBA user needs --- privilege to create a materialized view.
* Create materialized view
* ***Create any snapshot***
* Create View

### 18. Data within MView is session specific
* True
* ***False***

### 19. Which of the following will need disk space for storage.
* ***MView and Indexes***
* Inline Views and CTEs

### 20. The side-effect of MView is the additional disk space to store records in it.
* ***True***
* False
