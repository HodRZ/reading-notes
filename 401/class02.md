# SQL database, ORM, Sequelize

In a previous readings (*[Mongo](./../301/class11.md)*) we touched on the topic of databases and the difference between SQL and NoSQL databases, this time we'll focus on the SQL part.
___

## ORM

ORM stands for *Object–relational mapping*, it's a technique used to work with SQL databases, it allows an object code (OOP) to connect with a relational database. It also simplifies development by using the same code used in development instead of pure SQL queries.

![ORM](https://miro.medium.com/max/950/1*0STzo-DcWTZL90RkL0tSwQ.png)

An *ORM library* is any library that adds the ORM capabilities to the your App, one of the most used with the **PERN stack** is **Sequelize**

## [Sequelize](https://sequelize.org/)

___

### What and Why Sequelize

> Sequelize is a modern TypeScript and Node.js ORM for Postgres, MySQL, MariaDB, SQLite and SQL Server, and more. Featuring solid transaction support, relations, eager and lazy loading, read replication and more.

Sequelize handles the translation from JavaScript to SQL statements, allowing us to interact with a Postgres database using JavaScript instead of SQL.

![Sequelize](https://res.cloudinary.com/practicaldev/image/fetch/s--KsAKfY6F--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://loizenai.com/wp-content/uploads/2020/08/Nodejs-PostgreSQL-CRUD-Example-Architecture-Overview.png)

___

### How to Sequelize

to start using Sequelize, we follow the steps in the official docs:

1- install Sequelize using npm

>`npm install --save sequelize`

2- install a driver for the database, in this case Postgres

>`npm install --save pg pg-hstore`

3- configure the environment variables in the `.env`

>`DB_HOST=127.0.0.1`
>`DB_USERNAME=username`
>`DB_PASSWORD=password`

4- connect to the database

>`const { Sequelize } = require('sequelize');`
>`const sequelize = new Sequelize('postgres://user:pass@example.com:5432/dbname')`

5- define a model to use
>A model is an abstraction that represents a table in your database
