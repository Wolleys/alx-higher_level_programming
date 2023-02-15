# SQL - More queries

# Resources
1. [How To Create a New User and Grant Permissions in MySQL](https://www.digitalocean.com/community/tutorials/how-to-create-a-new-user-and-grant-permissions-in-mysql)
2. [How To Use MySQL GRANT Statement To Grant Privileges To a User](https://www.mysqltutorial.org/mysql-grant.aspx)
3. [MySQL constraints](https://zetcode.com/mysql/constraints/)
4. [SQL technique: subqueries](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/subqueries.php)
5. [Basic query operation: the join](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/join.php)
6. [SQL technique: multiple joins and the distinct keyword](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/multijoin.php)
7. [SQL technique: join types](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/jointypes.php)
8. [SQL technique: union and minus](https://web.csulb.edu/colleges/coe/cecs/dbdesign/dbdesign.php?page=sql/setops.php)
9. [MySQL Cheat Sheet](https://intellipaat.com/mediaFiles/2019/02/SQL-Commands-Cheat-Sheet.pdf?US)
10. [The Seven Types of SQL Joins](https://tableplus.com/blog/2018/09/a-beginners-guide-to-seven-types-of-sql-joins.html)
11. [MySQL Tutorial](https://www.youtube.com/watch?v=yPu6qV5byu4)
12. [SQL Style Guide](https://www.sqlstyle.guide)
13. [MySQL 8.0 SQL Statement Syntax](https://dev.mysql.com/doc/refman/8.0/en/sql-statements.html)

Extra resources around relational database model design:
1. [Design](https://www.guru99.com/database-design.html)
2. [Normalization](https://www.guru99.com/database-normalization.html)
3. [ER Modeling](https://www.guru99.com/er-modeling.html)

# Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg), **without the help of Google:**

## General
* How to create a new MySQL user
* How to manage privileges for a user to a database or table
* What’s a `PRIMARY KEY`
* What’s a `FOREIGN KEY`
* How to use `NOT NULL` and `UNIQUE` constraints
* How to retrieve datas from multiple tables in one request
* What are subqueries
* What are `JOIN` and `UNION`

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

## How to import a SQL dump

```
$ echo "CREATE DATABASE hbtn_0d_tvshows;" | mysql -uroot -p
Enter password: 
$ curl "https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/274/hbtn_0d_tvshows.sql" -s | mysql -uroot -p hbtn_0d_tvshows
Enter password: 
$ echo "SELECT * FROM tv_genres" | mysql -uroot -p hbtn_0d_tvshows
Enter password: 
id  name
1   Drama
2   Mystery
3   Adventure
4   Fantasy
5   Comedy
6   Crime
7   Suspense
8   Thriller
$
```

# Tasks
Tasks table

| Task Name  | File Name | Description |
| --------------- | ------------------------------ |---------------------------------------------------------------|
| 0. My privileges! | `0-privileges.sql` | List all privileges of the MySQL users `user_0d_1` and `user_0d_2` |
| 1. Root user | `1-create_user.sql` | Create the MySQL server user `user_0d_1` |
| 2. Read user | `2-create_read_user.sql` | Create the database `hbtn_0d_2` and the user `user_0d_2` |
| 3. Always a name | `3-force_name.sql` | Create the table `force_name` on your MySQL server |
| 4. ID can't be null | `4-never_empty.sql` | Create the table `id_not_null` on your MySQL server |
| 5. Unique ID | `5-unique_id.sql` | Create the table `unique_id` on your MySQL server |
| 6. States table | `6-states.sql` | Create the database `hbtn_0d_usa` and the table `states` |
| 7. Cities table | `7-cities.sql` | Create the database `hbtn_0d_usa` and the table `cities` |
| 8. Cities of California | `8-cities_of_california_subquery.sql` | List all the cities of California |
| 9. Cities by States | `9-cities_by_state_join.sql` | List all cities contained in the database `hbtn_0d_usa` |
| 10. Genre ID by show | `10-genre_id_by_show.sql` | List all shows contained in `hbtn_0d_tvshows` |
| 11. Genre ID for all shows | `11-genre_id_all_shows.sql` | List all shows contained in the database `hbtn_0d_tvshows` |
| 12. No genre | `12-no_genre.sql` | List all shows contained in `hbtn_0d_tvshows` without a genre linked |
| 13. Number of shows by genre | `13-count_shows_by_genre.sql` | List all genres from `hbtn_0d_tvshows` |
| 14. My genres | `14-my_genres.sql` | List all genres of the show `Dexter` from `hbtn_0d_tvshows` db |
| 15. Only Comedy | `15-comedy_only.sql` | List all Comedy shows in the database `hbtn_0d_tvshows` |
| 16. List shows and genres | `16-shows_by_genre.sql` | List all shows, and all genres linked to that show |
| 17. Not my genre | `100-not_my_genres.sql` | List all genres not linked to the show `Dexter` |
| 18. No Comedy tonight! | `101-not_a_comedy.sql` | List all shows without the genre Comedy |
| 19. Rotten tomatoes | `102-rating_shows.sql` | List all shows by their rating |
| 20. Best genre | `103-rating_genres.sql` | List all genres by their rating |
