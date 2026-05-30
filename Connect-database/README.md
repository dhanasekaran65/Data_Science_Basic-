# Python — Connect Database using Python

A hands-on Jupyter Notebook demonstrating how to connect Python to both MySQL and MongoDB databases and perform full CRUD operations.

## Databases covered

| Database | Library | Connection |
|---|---|---|
| MySQL | mysql-connector-python | localhost:3306 |
| MongoDB | pymongo | localhost:27017 |

## MySQL operations

| Operation | Code used |
|---|---|
| Connect | `mysql.connector.connect()` |
| Create DB | `CREATE DATABASE student_data` |
| Create Table | `CREATE TABLE student(...)` |
| Insert | `INSERT INTO student VALUES(%s,...)` |
| Fetch all | `cursor.fetchall()` |
| Update | `UPDATE student SET col=%s WHERE...` |
| Delete | `DELETE FROM student WHERE...` |
| Close | `connection.close()` |

## MongoDB operations

| Operation | Method |
|---|---|
| Connect | `MongoClient("mongodb://localhost:27017")` |
| Insert one | `collection.insert_one(doc)` |
| Insert many | `collection.insert_many([...])` |
| Find all | `collection.find()` |
| Find one | `collection.find_one({"key":"val"})` |
| Update one | `collection.update_one({},{"$set":{}})` |
| Update many | `collection.update_many({},{"$set":{}})` |
| Delete one | `collection.delete_one({"key":"val"})` |
| Delete many | `collection.delete_many({})` |
| Count docs | `collection.count_documents({})` |

## How to run

```bash
pip install mysql-connector-python pymongo
jupyter notebook Connect_Database_using_python.ipynb
```

> Make sure MySQL server and MongoDB are running locally before executing cells.
