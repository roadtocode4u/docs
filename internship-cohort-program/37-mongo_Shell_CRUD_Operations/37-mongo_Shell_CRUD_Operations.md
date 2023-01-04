<!-- 37-mongo_Shell_CRUD_Operations -->
# MongoDB Shell CRUD Operations

## Show databases

To show all databases, use the `show dbs` command. This command will return a list of all databases in the MongoDB instance. There are two databases in the MongoDB instance: `admin` and `local`. The `admin` database is used to store administrative information. The `local` database is used to store replica set configuration information.

```js
show dbs
```

This will return the following output:

```js
admin   0.000GB
config  0.000GB
local   0.000GB
```

## Use database

To use a database, use the `use` command. This command will switch the current database to the specified database. Let's use the `test` database.

```js
use test
```

This will return the following output:

```js
switched to db test
```

## Show collections

To show all collections in the current database, use the `show collections` command. This command will return a list of all collections in the current database. There are two collections in the `test` database: `users` and `posts`.

```js
show collections
```

This will return the following output:

```js
posts
users
```

## CRUD Operations

CRUD stands for Create, Read, Update, and Delete. These are the four basic operations that we can perform on a database. In this lesson, we will learn how to perform these operations using the MongoDB shell. 

### Create

To create a new document in a collection, we use the `insertOne()` method. This method takes a single document as an argument. Let's create a new document in the `users` collection.

```js
db.users.insertOne({
  name: "John Doe",
  age: 25,
  favoriteFoods: ["pizza", "ice cream"]
})
```

This will create a new document in the `users` collection with the following properties:

```js
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9b"),
  name: "John Doe",
  age: 25,
  favoriteFoods: ["pizza", "ice cream"]
}
```

We can also create multiple documents at once using the `insertMany()` method. This method takes an array of documents as an argument. Let's create a few more documents in the `users` collection.

```js
db.users.insertMany([
  {
    name: "Jane Doe",
    age: 30,
    favoriteFoods: ["pizza", "ice cream"]
  },
  {
    name: "John Smith",
    age: 35,
    favoriteFoods: ["pizza", "ice cream"]
  },
  {
    name: "Jane Smith",
    age: 40,
    favoriteFoods: ["pizza", "ice cream"]
  }
])
```

This will create the following documents in the `users` collection:

```js
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9c"),
  name: "Jane Doe",
  age: 30,
  favoriteFoods: ["pizza", "ice cream"]
},
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9d"),
  name: "John Smith",
  age: 35,
  favoriteFoods: ["pizza", "ice cream"]
},
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9e"),
  name: "Jane Smith",
  age: 40,
  favoriteFoods: ["pizza", "ice cream"]
}
```

### Read

To read documents from a collection, we use the `find()` method. This method returns a cursor that we can use to iterate over the documents in the collection. Let's read all of the documents in the `users` collection.

```js
db.users.find()
```

This will return the following documents:

```js
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9b"),
  name: "John Doe",
  age: 25,
  favoriteFoods: ["pizza", "ice cream"]
},
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9c"),
  name: "Jane Doe",
  age: 30,
  favoriteFoods: ["pizza", "ice cream"]
},
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9d"),
  name: "John Smith",
  age: 35,
  favoriteFoods: ["pizza", "ice cream"]
},
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9e"),
  name: "Jane Smith",
  age: 40,
  favoriteFoods: ["pizza", "ice cream"]
}
```

We can also use the `findOne()` method to read a single document from a collection. This method returns the first document that matches the query. Let's read the first document in the `users` collection.

```js
db.users.findOne()
```

This will return the following document:

```js
{
  _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9b"),
  name: "John Doe",
  age: 25,
  favoriteFoods: ["pizza", "ice cream"]
}
```

### Update

To update a document in a collection, we use the `updateOne()` method. This method takes a filter and an update document as arguments. Let's update the `name` property of the first document in the `users` collection.

```js
db.users.updateOne(
  { _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9b") },
  { $set: { name: "John Doe Jr." } }
)
```

This will update the `name` property of the first document in the `users` collection to `John Doe Jr.`.

We can also use the `updateMany()` method to update multiple documents in a collection. This method takes a filter and an update document as arguments. Let's update the `name` property of all documents in the `users` collection.

```js
db.users.updateMany(
  {},
  { $set: { name: "John Doe Jr." } }
)
```

This will update the `name` property of all documents in the `users` collection to `John Doe Jr.`.

### Delete

To delete a document from a collection, we use the `deleteOne()` method. This method takes a filter as an argument. Let's delete the first document in the `users` collection.

```js
db.users.deleteOne({ _id: ObjectId("5b9b7b9b9b9b9b9b9b9b9b9b") })
```

This will delete the first document in the `users` collection.

We can also use the `deleteMany()` method to delete multiple documents from a collection. This method takes a filter as an argument. Let's delete all documents in the `users` collection.

```js
db.users.deleteMany({})
```

This will delete all documents in the `users` collection.

## Summary

In this lesson, we learned about MongoDB and how to use the MongoDB shell to perform CRUD operations on a MongoDB database. We also learned about the MongoDB data model and how to use the MongoDB shell to create, read, update, and delete documents in a collection.

## Resources

- [MongoDB Documentation](https://docs.mongodb.com/manual/)

- [MongoDB Shell Commands](https://docs.mongodb.com/manual/reference/mongo-shell/)

- [MongoDB CRUD Operations](https://docs.mongodb.com/manual/crud/)