# Environment Variables and Dotenv

## What are Environment Variables?

Environment variables are variables that are set outside of the application. They are used to store configuration data that is used by the application. Environment variables are used to store sensitive data such as API keys, passwords, etc. that should not be stored in the code.

## Why Environment Variables?

Environment variables are used to store sensitive data that should not be stored in the code. They are also used to store configuration data that is used by the application.

## Dotenv

Dotenv is a zero-dependency module that loads environment variables from a `.env` file into `process.env`. Storing configuration in the environment separate from code is based on The Twelve-Factor App methodology.

## Installation

```bash
npm install dotenv
```

## Usage

Create a `.env` file in the root directory of your project. Add environment-specific variables on new lines in the form of `NAME=VALUE`. For example:

```bash
PORT=3000
MONGODB_URL=mongodb://localhost:27017
```
Also remember to add `.env` to `.gitignore` file.

```bash
.gitignore
node_modules
.env
```

Add the following code to the file:

```js
import dotenv from 'dotenv';

dotenv.config();
```
This will import the `dotenv` module and call the `config()` function. This will read the `.env` file and add the variables to `process.env`.

Now, you can access the environment variables anywhere in your application. For example:

```js
const port = process.env.PORT;

mongoose.connect(process.env.MONGODB_URL, ()=>
    console.log('Connected to MongoDB')
);
```

## Resources

- [Environment Variables](https://www.twilio.com/blog/2017/08/working-with-environment-variables-in-node-js.html)
