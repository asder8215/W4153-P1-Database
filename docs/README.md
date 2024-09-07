# W4153-P1-Database

The link to the repository is: https://github.com/donald-f-ferguson/W4153-P1-Database

## Overview

Project 1 in W4153 - Cloud Computing is to build a simple [fullstack web application.](https://medium.com/@p.reaboi.frontend/understanding-full-stack-development-architecture-a-comprehensive-guide-548f8cba6d91)

This project is the database project. 

|   <img src="fullstack.jpg">   |
|:-----------------------------:|
| __Fulltsack Web Application__ |


## Installation

You must have installed [MySQL Community Edition](https://dev.mysql.com/downloads/mysql/8.0.html). During the
installation,
- You will be asked to choose an authentication method. Choose the ```Legacy``` authentication.
- You will be asked to set a root password. I __strongly suggest__ you use ```dbuserdbuser```. Please write
down you password in a place where you can find it again. In general, writing down passwords _is a really
bad idea._ It is not a problem in this situation.

MySQL should startup automatically.

I __strongly recommend__ that you use [DataGrip](https://www.jetbrains.com/datagrip/) for your database
development environment. Follow the [instructions](https://www.jetbrains.com/help/datagrip/mysql.html) for creating a
data source to your local MySQL Server. You may see a link to install necessary driver files.

Once you have established a successful data source, create a new __database schema.__ Name the database schema
```pi_database.``` Open a query console on the ```p1_database.``` Enter the following (you can cut and paste)
into the query console.

```
use p1_database;

create table if not exists course_sections
(
    course_id     bigint null,
    course_name   text   null,
    uuid          text   null,
    created_at    text   null,
    course_code   text   null,
    sis_course_id text   null,
    course_no     text   null,
    section       text   null,
    course_year   text   null,
    semester      text   null
);

insert into p1_database.course_sections
value (204283,
       "COMSW4153_001_2024_3 - Cloud Computing",
       "3jHCxUV0ck9Z8TF1sZeI8WTx47olDGkX1YPL3USM",
       "024-04-05T00:58:50Z",
       "COMSW4153_001_2024_3 - Cloud Computing",
       "COMSW4153_001_2024_3",
       "COMSW4153",
       "001",
       "2024",
       "3")
```

You will see a lot of information messages. You completed your task if the last informational message
is something like.

```[2024-09-07 08:04:37] 1 row affected in 3 ms```



