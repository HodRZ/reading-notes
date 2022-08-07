# Mongo and Mongoose

**SQL** databases or *Relational Databases*, are databases that uses *Structured Query Language* and have a *predefined schema (the blueprint of how the data will look)*, they're *vertically* scalable, and are *table* based.

**NoSQL** databases or *Non-Relational*, are databases that have a *dynamic schema*, they're *horizontally scalable*, and based on documents, key-value pairs, graphs,or wide column stors.

![sql vs nosql](https://phoenixnap.com/kb/wp-content/uploads/2021/04/database-types.jpg)

---

SQL databases uses 2d tables to store data, so for example it  might have a table for users and another table for contact info, so to connect the data it might use a third column with foreign/primary keys and this creates a *relation* betweed the stored data.

SQL databases are known for *Simplicity*, *Data Security*, *Accessibility*, and *Data accuracy and integrity (ACID)*. BUT they're *Expensive*, *Doesn't perform better when grow*, and *Doesn't Scale well*.

![relational database](https://www.pragimtech.com/blog/contribute/article_images/2220211210231003/what-is-a-relational-database.jpg)

![relational databse](https://www.pragimtech.com/blog/contribute/article_images/2220211210231003/what-is-a-database.jpg)

---
NoSQL databases doesn't rely on tables, lets take MongoDB for example, it relies on collections that store multiple documents.

NoSQL databases have a *Great Performance*, they *Scale well*, and they're *Flexible* since they doesn't require a predefined schema, and they're also *Cost Effective*. BUT being a new technology it *Lacks the Support* that the SQL has, it has some *Consistency Issues (BASE)*, and it proves challenging for data analysis applications.

![mongoDB](https://www.pragimtech.com/blog/contribute/article_images/2220211210231003/what-is-mongodb.jpg)

![mongo hirarchy](https://www.pragimtech.com/blog/contribute/article_images/2220211210231003/mongodb-collection-vs-document.jpg)
