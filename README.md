# The solution

mysql> create table Movie
    -> (
    -> moive_id INT,
    -> title VARCHAR(100),
    -> director VARCHAR(50),
    -> release_year INT,
    -> genre VARCHAR(50)
    -> );
Query OK, 0 rows affected (0.02 sec)

mysql> ALTER TABLE Movie ADD COLUMN rating DECIMAL(3, 1);
Query OK, 0 rows affected (0.02 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> create table Students
    -> (
    -> student_id INT,
    -> student_name VARCHAR(50),
    -> age INT,
    -> grade VARCHAR(2)
    -> );
Query OK, 0 rows affected (0.02 sec)

mysql> DROP TABLE Students;
Query OK, 0 rows affected (0.01 sec)

mysql> create table Events
    -> (
    -> event_id INT,
    -> event_name VARCHAR(100),
    -> date DATE,
    -> location VARCHAR(100)
    -> );
Query OK, 0 rows affected (0.03 sec)


mysql> show tables;
+---------------+
| Tables_in_db1 |
+---------------+
| events        |
| movie         |
| superuser     |
| users         |
+---------------+
4 rows in set (0.00 sec)

mysql> INSERT INTO Events VALUES(1, 'Java', '2032-12-13', 'Berlin');
Query OK, 1 row affected (0.01 sec)

mysql> INSERT INTO Events VALUES(1, 'Java', '2024-01-18', 'London');
Query OK, 1 row affected (0.00 sec)

mysql> INSERT INTO Events VALUES(2, 'Dance', '2024-01-18', 'London');
Query OK, 1 row affected (0.01 sec)

mysql> TRUNCATE TABLE Events;
Query OK, 0 rows affected (0.04 sec)

mysql> create table Restaurants
    -> (
    -> restaurant_id INT,
    -> name VARCHAR(50),
    -> cuisine VARCHAR(50),
    -> location VARCHAR(100)
    -> );
Query OK, 0 rows affected (0.03 sec)

mysql> RENAME TABLE Restaurants TO DiningSpots;
Query OK, 0 rows affected (0.01 sec)

mysql> show tables;
+---------------+
| Tables_in_db1 |
+---------------+
| diningspots   |
| events        |
| movie         |
| superuser     |
| users         |
+---------------+
5 rows in set (0.00 sec)