# SQL Lesson 2 &amp; Mission 2

## What we have learned
### CRUD operations (Create, Read, Update &amp; Delete)
#### Create: Insert statement
```sql
INSERT INTO tbl_name (col1,col2) VALUES(15,20);
```

#### Read: Select statement
```sql
SELECT col1,col2 FROM tbl_name;
```

#### Update: Select statement
```sql
UPDATE t1 SET col1 = col1 + 1, col2 = col1;
```

#### Update: Select statement
```sql
DELETE FROM somelog WHERE user = 'jcole'
```

### Where clause
```sql
INSERT INTO t_copy SELECT * FROM t WHERE ... ;
DELETE FROM somelog WHERE user = 'jcole'
```

## Homework
Please save all the queries that you write in a file called `hw_queries.sql`
### Insert new data
#### `customers` table
```sql
(1, 'avner', 'gadasi', 'avner@exam    ple.com', 'tel aviv')
(2, 'kurt', 'cobain', 'moshe@example.com', 'aberdeen')
(3, 'rihanna', 'fenty', 'rihanna@example.com', 'saint michael')
(4, 'amy', 'winehouse', 'amy@example.com', 'london')
```

#### Salesmans table
```sql
(123, 'sman1', 'smanl_last', 'sman1@example.com', 'jerusalem', '2016-03-25')
(234, 'sman2', 'sman2_last', 'sman2@example.com', 'tel aviv', '2016-03-25')
(345, 'sman3', 'sman3_last', 'sman3@example.com', 'afula', '2016-03-25')
(456, 'sman4', 'sman4_last', 'sman4@example.com', 'haifa', '2016-03-25')
```

#### Purchases table

#### Products table
```sql 
('blank disc', 5)
('microphone', 599)
('laptop', 4999)
('alcohol', 59)
```

### Results expected
#### `customers` table
| social_security | first_name    | last_name | email               | city          |
| -------------   | ------------- |---------- | -------------       | ---------     |
| 1               | avner         | gadasi    | avner@example.com   | tel aviv      |
| 2               | kurt          | cobain    | kurt@example.com    | aberdeen      |
| 3               | rihanna       | fenty     | rihanna@example.com | saint michael |
| 4               | amy           | winehouse | amy@example.com     | london        |

#### Salesmans table
| social_security | first_name  | last_name  | email             | city       | start_of_work_date |
| -------------   | ----------- |----------  | -------------     | ---------  | ---------------    |
| 123             | sman1       | sman1_last | sman1@example.com | jerusalem  | 2016-03-25         |
| 234             | sman2       | sman2_last | sman2@example.com | tel aviv   | 2012-07-14         |
| 345             | sman3       | sman3_last | sman3@example.com | afula      | 2013-02-12         |
| 456             | sman4       | sman4_last | sman4@example.com | london     | 2012-08-29         |

#### Products table
| id  | name          | price  |
| --- | ------------- |------- |
| 1   | blank disc    | 5      |
| 2   | microphone    | 599    |
| 3   | laptop        | 4999   |
| 4   | alcohol       | 59     |

## Solution
Found in this repository at `northwind.sql` file.

## Materials
### Links
MySQL developers: insert
https://dev.mysql.com/doc/refman/5.7/en/insert.html

MySQL developers: update
https://dev.mysql.com/doc/refman/5.7/en/update.html

MySQL developers: select
https://dev.mysql.com/doc/refman/5.7/en/select.html

MySQL developers: delete
https://dev.mysql.com/doc/refman/5.7/en/delete.html