# Install PostgreSQL 12 on Amazon Linux 2
use thefollowing link to create upostgresql
```
https://techviewleo.com/install-postgresql-12-on-amazon-linux/
```

# Install postgresql using ansible
use the following link
```
https://middlewaretechnologies.in/2021/12/how-to-install-and-configure-postgresql-database-using-ansible-playbook.html
```
## write quries in postgresql
login into db
```
$ sudo su - postgres 
-bash-4.2$ psql 
```
Create database and connect
```
CREATE DATABASE students;
```
\c students 
```

Cretate table in students database
```
create table users (
  id serial primary key,
  name character varying not null,
  active boolean default true
);
```

SELECT * FROM users;
```
```
CREATE TABLE PASSENGERS(

"Id" INT PRIMARY KEY NOT NULL,

"Name" VARCHAR (100) NOT NULL,

"Email" VARCHAR (255) UNIQUE NOT NULL,

"Age" INTEGER NOT NULL,

"Travel_to" VARCHAR (255) NOT NULL,

"Payment" INTEGER,

"Travel_date" DATE

);
```
```
INSERT INTO "users" ("id", "name", "active")
VALUES (1, 'Jack', 'true') ;
```
inster query in postgresql
```
INSERT INTO "passengers" ("Id", "Name", "Email", "Age", "Travel_to", "Payment", "Travel_date")
VALUES (1, 'Jack', 'jack12@gmail.com', 20, 'Paris', 79000, '2018-1-1') ;
```
delete tables
```
DROP TABLE users; 
```
\dt ------------ list of tables

\dn ----------- list of schemas

create schemas
```
CREATE SCHEMA employees; create schemas
