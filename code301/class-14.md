# Database Normalization 

Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included. By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.

Having the table serve many purposes introduces many of the challenges:
1. data duplication
1. data update issues
1. increased effort to query data

There are three main reasons to normalize a database:
1. to minimize duplicate data
1. to minimize or avoid data modification issues
1. to simplify queries

There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form.

- First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.


- Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.


- Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key


[Database Normalization Explained in Simple English](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)



[<----Back Home](../README.md)