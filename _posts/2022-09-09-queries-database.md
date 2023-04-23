---
title: Database Query 
author: Nikky Leone
date: 2022-08-09 20:55:00 +0800
categories: [Year 7, Database]
tags: [queries]
---

**In standard English, a query means a request for information. In computer programming, it refers to the same thing, except the information is retrieved from a database.**

**However, writing a query requires a set of pre-defined code to make the database understand the instruction. This concept is also known as the query language.**

While the standard language for database management is **Structured Query Language (SQL)**, other query languages to make database communication easy include **AQL**, **Datalog**, and **DMX**.

> **Important!** Note that `SQL` is different from `MySQL` – the former is the query language, while the latter is the **software that uses** the language.
{: .prompt-warning }

This article will explain how a query works, examples of queries, and cover the **steps of writing them in the database. (Optional)**

# What Is a Query?

**A database query is a request for data from a database. The request should come in a database table or a combination of tables using a code known as the query language. This way, the system can understand and process the query accordingly.**

# How Does Query Work?

**Let’s say that you want to order an Americano at a coffee shop. You make a request by saying, “Can I have an Americano?”. The barista will understand the meaning of your request and give you the ordered item.**

**A query works the same way – it adds meaning to the code, allowing the system to understand and execute actions accordingly.** Be it `SQL` or any other query language, **both the user and the database can exchange information as long as they use the same language.**

Meanwhile, **a well-designed database stores data in multiple tables. They consist of columns that hold the data’s attributes, along with rows or records of information. A query then helps retrieve data from different tables, arrange them, and display them according to the commands.**

**A query can either be a select, an action, or a combination of both. Select queries can retrieve information from data sources, and action queries work for data manipulation, for example, to add, change or delete data.**

**Advanced users can also use query commands to perform various programming tasks**, from creating MySQL users and granting permissions to changing WordPress URLs in `MySQL` databases.

*Below are some of the most common query commands along with their functions:*


SELECT 
: fetch data from the database. It’s one of the most popular commands, as every request begins with a select query.

AND
: combine data from one or more tables.

CREATE TABLE
: build different tables and specify the name of each column within.

ORDER BY
: sort data results either numerically or alphabetically.

SUM
: summarize data from a specific column.

UPDATE
: modify existing rows in a table.

INSERT
: add new data or rows to an existing table.

WHERE
: filter data and get its value based on a set condition.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

For more variations, combine some of the commands above. For example, pair the `SELECT` query with other commands like `AND` or `SUM` to aggregate data or combine results.

Besides using query language to request information from a database, other methods include:

- **Using available parameters. By default, the database software has lists of parameters that users can define as they need. These parameters deal with exchanging information between user-defined functions (UDF) and stored procedures (SP).**
- **Query by example (QBE). Relational databases use a graphical query language. The system will show a code template in which you can write and specify the fields and values of your data. So instead of writing complete SQL statements, a user can fill the blank areas.**
- **Installing database plugins. An ideal solution for beginners – the plugins let users perform various database tasks, including queries, with only a few clicks. Additionally, some plugins come with optimization features to ensure the best performance.**

**In addition to databases, search engines can also query and retrieve information. However, the term query in these two technologies differs.**

**Web search query refers to keywords that users type in the search engine**, while database query is a particular action to make a request for information.

Now that you understand the basic fundamentals of queries, **let’s study several standard terms you might come across when querying a database:**

Query string
: a portion of URL to pass requests from the web to the database.

Query parameters
: elements attached to the end of an URL to specify a particular query on the database.

Query folding
: refers to a process where the Power Query is enabled to transform complex calculations for query optimization.

Query containment
: happens when one query is contained in another, if it is independent of the stored data values.

# Query Languages

As mentioned before, **choosing the database and its language is crucial when working with queries.** In addition to `SQL`, there is another type of database called `NoSQL` (Not Only Structured Query Language). The main difference between the two is the data structure.

**`SQL` databases are relational and use predefined schemas that require you to specify your data structure.** On the other hand, `NoSQL` databases are non-relational and have dynamic schemas for unstructured data.

**Regardless, both `SQL` and `NoSQL` provide applicable options. An `SQL` database is a great choice for an ACID-compliant data structure. Conversely, if you have unstructured documents, key-values, or graphs, a `NoSQL` database might be an ideal choice.**

# Query Examples

Before we delve into the examples, below are the main benefits of using a query:

- Review data from multiple tables simultaneously.
- Filter records containing only certain fields and of certain criteria.
- Automate data management tasks and perform calculations.

**, let’s suppose you have collected some data from a survey. Below is a snippet of your data. Note that for this example, we will use an `SQL` database.**


![Table1](https://raw.githubusercontent.com/ConyersSchool/ConyersSchool.github.io/master/assets/img/table1.png){: width="712" height="239" }


## **Selecting Only the “Name” and “Occupation” Columns From the “Participant” Table**

**This example shows you how to create a select query that only returns the value for Name and Occupation. The `SQL` statement should look something like this:**

```sql
SELECT Name, Occupation FROM Participant 
```

The statement above filters specific data from the table. It will generate the following result table:


![Table2](https://raw.githubusercontent.com/ConyersSchool/ConyersSchool.github.io/master/assets/img/table2.png){: width="712" height="239" }



To select other types of data from the table, change the variables accordingly.

## **Deleting Data From the Unemployed Respondents**

**The `DELETE` query works to remove existing records from particular tables. In this example, we are going to delete the Unemployed records using the following statement:**

`DELETE FROM Participant WHERE Occupation = ‘Unemployed’`

Hit enter, and this will remove the respective records and return this output:


![Table3](https://raw.githubusercontent.com/ConyersSchool/ConyersSchool.github.io/master/assets/img/table3.png){: width="712" height="239" }



## **Inserting a New Row Containing a Participant Called Mario**

**In a broader scene, the `INSERT INTO` query inserts data into the `MySQL` database via `MySQLi` and `PHP` Data Object. However, this example will show how to use the query to add a new row to a database table.**

There are two different ways to incorporate this `SQL` statement:

**If you’re adding new values and fields, specify all the elements. Hence, the statement will look like this:**

```sql
INSERT INTO <em>table_name</em> (<em>column1</em>,<em> column2</em>,<em> column3</em>, ...)
VALUES (<em>value1</em>,<em> value2</em>,<em> value3</em>, ...);
```

**If you’re only adding new values to all existing columns, use the statement below:**

```sql
INSERT INTO <em>table_name</em>
VALUES (<em>value1</em>,<em> value2</em>,<em> value3</em>, ...);
```

## **Changing Margareth’s Occupation to “Headmaster”**

**To modify existing records in a table, use the `UPDATE` query. Meanwhile, to specify which rows to update, use the `WHERE` query. **

In this case, we’re going to edit Margareth’s occupation to Headmaster. Thus, the SQL statement will be:

```sql
UPDATE Participant SET Occupation = ‘Headmaster’ WHERE ID = ‘3’
```

The query runs to update row 3 into the specified value and shows the following output:


![Table4](https://raw.githubusercontent.com/ConyersSchool/ConyersSchool.github.io/master/assets/img/table4.png){: width="712" height="239" }



## Wrapping Up

**A query can either be a select or action query – select queries pick parts of your data, while action queries manipulate retrieved data. **

**A query can also work with the combination of both actions to perform more varied tasks, for example, to review, insert, modify, or delete data, as well as calculate and combine data from multiple tables.**

**Database queries show that manipulating data doesn’t have to be complicated. Most query languages are intuitive and are easy to learn once you understand some basic rules.** For those who don’t feel comfortable coding, you can use database plugins or Query by example as alternatives.
 

> **Important!** Note that you don't have to learn SQL or undertand it fully, I used it to showcase a few examples. Try to look back at this post if you are in year 10.
{: .prompt-tip }

