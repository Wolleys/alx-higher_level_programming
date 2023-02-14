# MySQL - Introduction

# Resources
1. [What is Database & SQL?](https://www.youtube.com/watch?v=FR4QIeZaPeM)
2. [A Basic MySQL Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-20-04)
3. [Basic SQL statements: DDL and DML](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/ddldml.php) (*no need to read the chapter “Privileges”*)
4. [Basic queries: SQL and RA](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/queries.php)
5. [SQL technique: functions](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/functions.php)
6. [SQL technique: subqueries](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/subqueries.php)
7. [What makes the big difference between a backtick and an apostrophe?](https://stackoverflow.com/questions/29402361/what-makes-the-big-difference-between-a-backtick-and-an-apostrophe/29402458)
8. [MySQL Cheat Sheet](https://intellipaat.com/mediaFiles/2019/02/SQL-Commands-Cheat-Sheet.pdf?US)
9. [MySQL 8.0 SQL Statement Syntax](https://dev.mysql.com/doc/refman/8.0/en/sql-statements.html)
10. [installing MySQL in Ubuntu 20.04](https://phoenixnap.com/kb/install-mysql-ubuntu-20-04)

# Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg), **without the help of Google:**

## General
* What’s a database
* What’s a relational database
* What does SQL stand for
* What’s MySQL
* How to create a database in MySQL
* What does `DDL` and `DML` stand for
* How to `CREATE` or `ALTER` a table
* How to `SELECT` data from a table
* How to `INSERT`, `UPDATE` or `DELETE` data
* What are `subqueries`
* How to use MySQL functions

# Requirements
## General
* Allowed editors: `vi`, `vim`, `emacs`
* All your files will be executed on `Ubuntu 20.04 LTS` using `MySQL 8.0` (version 8.0.25)
* All your files should end with a new line
* All your SQL queries should have a comment just before (i.e. syntax above)
* All your files should start by a comment describing the task
* All SQL keywords should be in uppercase (`SELECT`, `WHERE`…)
* A `README.md` file, at the root of the folder of the project, is mandatory
* The length of your files will be tested using `wc`

# More Info
## Comments for your SQL file:

```
$ cat my_script.sql
-- 3 first students in the Batch ID=3
-- because Batch 3 is the best!
SELECT id, name FROM students WHERE batch_id = 3 ORDER BY created_at DESC LIMIT 3;
$
```

## Install MySQL 8.0 on Ubuntu 20.04 LTS

```
$ sudo apt update
$ sudo apt install mysql-server
...
$ mysql --version
mysql  Ver 8.0.25-0ubuntu0.20.04.1 for Linux on x86_64 ((Ubuntu))
$
```

Connect to your MySQL server:
```
$ sudo mysql
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 11
Server version: 8.0.25-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql>
mysql> quit
Bye
$
```

## Use “container-on-demand” to run MySQL
**In the container, credentials are** `root/root`
* Ask for container `Ubuntu 20.04`
* Connect via SSH
* OR connect via the Web terminal
* In the container, you should start MySQL before playing with it:
```
$ service mysql start                                                   
 * Starting MySQL database server mysqld 
$
$ cat 0-list_databases.sql | mysql -uroot -p                               
Database                                                                                   
information_schema                                                                         
mysql                                                                                      
performance_schema                                                                         
sys                      
$
```
**In the container, credentials are** `root/root`

# Tasks
Tasks table

| Task Name  | File Name | Description |
| --------------- | ------------------------------ |---------------------------------------------------------------|
| 0. List databases | `0-list_databases.sql` | Add: List all databases of your MySQL server |
| 1. Create a database | `1-create_database_if_missing.sql` | Create the database `hbtn_0c_0` in your MySQL server |
| 2. Delete a database | `2-remove_database.sql` | Delete the database `hbtn_0c_0` in your MySQL server |
| 3. List tables | `3-list_tables.sql` | List all the tables of a database in your MySQL server |
| 4. First table | `4-first_table.sql` | Create a table called `first_table` |
| 5. Full description | `5-full_table.sql` | Print the full description of the table `first_table` |
| 6. List all in table | `6-list_values.sql` | List all rows of the table `first_table` from the database `hbtn_0c_0` |
| 7. First add | `7-insert_value.sql` | Insert a new row in the table `first_table` |
| 8. Count 89 | `8-count_89.sql` | Display the number of records with `id = 89` in the table `first_table` |
| 9. Full creation | `9-full_creation.sql` | Create a table `second_table` and add multiples rows |
| 10. List by best | `10-top_score.sql` | List all records of the table `second_table` |
| 11. Select the best | `11-best_score.sql` | List all records with a `score >= 10` in the table `second_table` |
| 12. Cheating is bad | `12-no_cheating.sql` | Update the score of Bob to `10` in the table `second_table` |
| 13. Score too low | `13-change_class.sql` | Remove all records with a `score <= 5` in the table `second_table` |
| 14. Average | `14-average.sql` | The score average of all records in the table `second_table` |
| 15. Number by score | `15-groups.sql` | List the number of records with the same score in the table `second_table` |
| 16. Say my name | `16-no_link.sql` | List all records of the table `second_table` |
| 17. Go to UTF8 | `100-move_to_utf8.sql` | Convert `hbtn_0c_0` database to UTF8 (`utf8mb4`, collate `utf8mb4_unicode_ci`) |
| 18. Temperatures #0 | `101-avg_temperatures.sql` | Display the average temperature by city ordered by temperature |
| 19. Temperatures #1 | `102-top_city.sql` | Display the top 3 of cities temperature during |
| 20. Temperatures #2 | `103-max_state.sql` | Display the max temperature of each state (ordered by State name) |
