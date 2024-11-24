# Ex.No.4. Implement NoSQL Database Operations: CRUD operations using MongoDB
## Aim
To perform Create, Read, Update, and Delete (CRUD) operations using MongoDB.

## Procedure

1.Install MongoDB and start the MongoDB service.
2.Connect to MongoDB using a client like MongoDB Compass or the mongo shell.
3.Execute CRUD operations on a sample database and collection.
## Code/Steps

1.Insert a single document:
```
db.students.insertOne({"name": "John", "age": 22, "course": "CSE"})
```
2.Insert multiple documents:
```
db.students.insertMany([
    {"name": "Anna", "age": 23, "course": "ECE"},
    {"name": "Mike", "age": 21, "course": "ME"}
])
```
3.Read documents:
```
db.students.find().pretty()
```
4.Update documents
```
db.students.updateOne({"name": "John"}, {$set: {"age": 23}})
```
5.Delete documents
```
db.students.deleteOne({"name": "Mike"})
```
## Result
Successfully implemented CRUD operations in MongoDB.

