# MongoDB

MongoDB is a document based database, which internally stores data in the form of
BSON, but we as normal developers can send or receive data in form of JSON,
internally mongodb manages the conversion of JSON-BSON and BSON-JSON
automatically.
Now when we used to store data in any RDBMS say MySQL, data was stored in tables.
Tables used to represent real life entity. Inside a table, we had many rows. Rows used
to represent one data record. Columns inside table used to represent properties of the
entity.
Now in mongodb, we store data in form of documents (JSON like).
So here, a real life entity is represented by Collections. What table is for RDBMS is
collections for mongodb. In simple terms, collections are group of JSON documents.
One record in a collection is called as Document. What row is for RDBMS is document
for mongodb.
A document is nothing but a JSON (internally BSON), a JSON has multiple key-value
pairs. The key of JSON represent the property of the entity. So what column is for
RDBMS, key (from key-value pair) is for mongodb .

# Installing MongoDB
To install mongoDb your system need to download
```
Link: https://medium.com/@LondonAppBrewery/how-to-download-install-mongodb-on-
windows-4ee4b3493514
```
# Using MongoDB

Open MongoDB in terminal:
Write  ``mongosh``  in your terminal, and it will open the mongodb console.

`![Alt Text] (Image/Screenshot from 2024-04-09 15-11-03.png)`

# List all databases in mongodb

To list all the databases stored in your mongodb we can use the below commands:

```
show database;
```
or

```
show dbs;
```
`![Alt Text] (Image/Screenshot from 2024-04-09 15-19-27.png)`

# How to select a particular DB to work on?

To select a particular db and start querying on it we can use
```
use name_of_database;
```

`![Alt Text] (Image/Screenshot from 2024-04-09 17-29-15.png)`

# How to print all the collections stored in a database ?

To print all the collections we can use:
```
show collections;
```

`[Alt Text] (Image/Screenshot from 2024-04-09 17-33-15.png)`

# How to print all the documents of a collection ?

To print all the documents of a collection we can use:
```
db.collectionname.find();
```
`[Alt Text] (Image/Screenshot from 2024-04-09 17-41-43.png)`

# How to create a new database ?
To create a new database we can do:
```
use new_database_name;
```
The ```use``` command creates a new database if there is no already present db with the
same name, otherwise if there is a db with the same name, it just selects it.