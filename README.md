# DB Foundations Module 07 - SQL Functions

```markdown
This website is to display Assignment 07's written paper for the IT Foundations 130 course at University of Washington.
```

## Introduction
This week in IT Foundations of Database Management, I learned about SQL functions. This included what functionality SQL functions add to a database, the different types of functions, and how to utilize functions by storing them within databases. I will demonstrate what I have learned by using references from this week’s coding assignment.

## When to use a SQL User Defined Function (UDF)
UDFs can also be used to enhance the functionality of a SQL database. They resemble stored procedures, by allowing users to pull data from a data source but operate differently. Users should consider using User Defined Functions (UDFs) to avoid writing complex statements repetitively. These functions are customizable, allowing users to retrieve a single value or a table of values from a database. UDFs can be applied to data tables or views and can be stored within a database. This allows functions to be used multiple times without being recreated.

In the example below from Assignment 07, the view in Figure 01 is being referenced by the UDF in Figure 02. By referring to the data stored within the existing view, users do not have to repeatedly recreate statements to perform the same function. This makes UDFs a powerful tool because it saves times and allows users of differing skill levels to have the same level of access to the data within a SQL database. This promotes an environment where users with lesser knowledge of SQL statements can have the same level of access to complex statements as more advanced users. 

![image](https://user-images.githubusercontent.com/84411887/119762550-c5d3da00-be62-11eb-8343-3174fc204839.png)

_**Figure 01: View created within an SQL Database containing a function.**_

![image](https://user-images.githubusercontent.com/84411887/119762563-ce2c1500-be62-11eb-98e6-9e361fe471ca.png)

_**Figure 02: Function created within an SQL Database referencing view created in Figure 01.**_

## Differences between Scalar, Inline, and Multi-Statement Functions
Scalar, inline and multi-statement functions are all functions that can be utilized within an SQL database. They have some distinct differences, but all return results within a database.
- Scalar Functions: Uses a function to return one value as a result. Multiple parameters can be used in the statement.
- Inline Functions: Use a function to return a set of results in a table. While visually similar to scalar functions, both are fundamentally different due to inline functions allowing users to return more than one value. This allows data to be filtered and modified prior to results being generated.
- Multi-Statement Functions: Use one or more functions to return a set of results in a table-like view. The fields of data can be customized, allowing users to create a table of unique results.

## Summary
After this week’s assignment, I have a better understanding of SQL functions and how they can build upon one another within a database. By allowing users to view data in a consolidated view, users can utilize advanced reporting techniques and gain access to high level data with ease. SQL functions also allow users to store them within a database as views or as functions, which reduces how often a function must be re-written to be used. This greatly reduces the strain upon a SQL database by eliminating duplicate functions running to pull the same data.
