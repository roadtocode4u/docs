## React 

React is a JavaScript library for building user interfaces. It is maintained by Facebook and a community of individual developers and companies. React can be used as a base in the development of single-page or mobile applications. 

## Folder Structure

The folder structure of a React project looks like this:

```bash
my-app/
  README.md
  node_modules/
  package.json
  public/
    index.html
    favicon.ico
  src/
    App.css
    App.js
    App.test.js
    index.css
    index.js
    logo.svg
```

For the project to build, **these files must exist with exact filenames**:

* `public/index.html` is the page template;
* `src/index.js` is the JavaScript entry point.

## Dom Manipulation

DOM manipulation is changing a document's structure, style, or content by using a scripting language such as JavaScript. 

## Cross Platform

Cross-platform is a term used to describe software that can use on more than one computer or operating system. For example, a cross-platform application can be used on Windows and Mac computers.

## 🤔 How to create a React App?

### npx

npx - node package executer

npx is a package runner tool. It allows you to run npm package binaries without installing them globally.

```bash
npx create-react-app my-app
```

## 🤔 How to start a React App?

npm - node package manager

npm is a package manager for the JavaScript programming language. It is the default package manager for the JavaScript runtime environment Node.js.

```bash
npm start
```

## 🤔 How to open a React App in the browser?

```bash
http://localhost:3000/
```

## SPA (Single Page Application)

A web application or web page interacts with the user by dynamically rewriting the current page instead of loading whole new pages from the server.

## React folder structures

### node_modules

This folder contains all the dependencies of the project. It is not recommended to modify the contents of this folder.

### package.json

package.json file contains the dependencies of the project. It is not recommended to modify the contents of this file.

### package-lock.json

package-lock.json file contains the exact version of the dependencies of the project. It is not recommended to modify the contents of this file.

### public

This folder contains the index.html file which is the entry point of the application. It is not recommended to modify the contents of this folder.

**robots.txt** file is used to tell search engines which pages or files the crawler can or can't request from your site.

**manifest.json** file is used to provide metadata associated with the web application.

**logo192.png** file is used to provide the logo of the web application.

**logo512.png** file is used to provide the logo of the web application.

**favicon.ico** file is used to provide the favicon of the web application.

**index.html** file is used to provide the entry point of the web application.

**%PUBLIC_URL%** This url points to the public folder.

**meta** tag is used to provide the metadata of the web application.

Note: Public folder is accessible everywhere in the application.

### src

It is the source folder of the application. It contains all the files related to the application.

**index.js** file is used to provide the entry point of the application.

**index.css** file is used to provide the styles of the entry point of the application.

**App.js** file is used to provide the root component of the application.

**App.css** file is used to provide the styles of the root component of the application.

**App.test.js** file is used to provide the test cases of the root component of the application.

### .gitignore

.gitignore file is used to tell git which files or folders to ignore in a project.
### React Components

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

There are two types of components in React:

* Class Components
* Functional Components

## Class Components

Class components are the ones which are defined as ES6 classes. They have a render method which returns a JSX. They also have a state object. They are also known as stateful or smart components.

## Functional Components

Functional components are the ones which are defined as functions. They have a return statement which returns a JSX. They do not have a state object. They are also known as stateless or dumb components.