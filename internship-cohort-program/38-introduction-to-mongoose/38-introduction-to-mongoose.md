# Introduction to Mongoose

## What is Mongoose?

Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

## Why Mongoose?

Mongoose provides a straight-forward, schema-based solution to modeling your application data and includes built-in type casting, validation, query building, business logic hooks and more, out of the box.

## Installation

```bash
npm install mongoose
```

## Connecting to MongoDB
### Syntax
```js
import mongoose from 'mongoose';

mongoose.connect('URL', 'CALLBACK FUNCTION');
```

### Example
```js
import mongoose from 'mongoose';

mongoose.connect('mongodb+srv://<username>:<password>@cluster0-<cluster>.mongodb.net/<dbname>?retryWrites=true&w=majority', {

    console.log('Connected to MongoDB');
});
```
## Creating a Schema

Schema is a blueprint of how the data should look like. It defines the structure of the document, default values, validators, etc. 

```js
import mongoose, {model, Schema} from 'mongoose';

const studentSchema = new Schema({
  name: String,
  age: Number,
  email: String,
});

const Student = mongoose.model('Student', studentSchema);

export default Student;
```
Here, we have created a schema for a student. The schema defines the structure of the document. The first argument of the `mongoose.model()` function is the name of the collection in the database. The second argument is the schema.

## Creating a Document

A document is an instance of the model. It is a single record in the database. 

```js
import Student from './studentModel.js';

const student = new Student({
  name: 'CM GoGo',
  age: 21,
  email: 'cmgogo@rtc.com',
});

student.save();
```
Here, we have created a document for a student. The first argument of the `new Student()` function is the data that we want to store in the database. The `save()` function saves the document to the database.

### Example

```js
import mongoose, {model, Schema} from 'mongoose';
import Student from './studentModel.js';

mongoose.connect('mongodb+srv://<username>:<password>@cluster0-<cluster>.mongodb.net/<dbname>?retryWrites=true&w=majority', {

    console.log('Connected to MongoDB');
});

const student = new Student({
  name: 'CM GoGo',
  age: 21,
  email: '
});

student.save();
```

## Finding Documents

### Syntax
```js
Model.find(QUERY, CALLBACK FUNCTION);
```

### Example
```js

Student.find({name: 'CM GoGo'}, (err, students) => {
  console.log(students);
});
```
Here, we have found all the documents in the `Student` collection where the `name` is `CM GoGo`. The first argument of the `find()` function is the query. The second argument is the callback function. The callback function takes two arguments. The first argument is the error. The second argument is the documents that match the query.