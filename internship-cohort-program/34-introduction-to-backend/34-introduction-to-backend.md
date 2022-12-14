# Introduction to Backend

```html
Client => Server
Frontend => Backend
```

**MVC**

**Model view Controller**

```
View => Visibile Things => Frontend

Model => Backend

Controller => Control The things

```

## APIs

 **Application Program Interface**

**Frontend**

<img height="250px" src="./frontend.png" />

**API**

 <img height="250px" src="./api.png" />
    
**Backend**

<img height="250px" src="./backend.png" />

```
 API are acts as an intermediary between frontend and backend.
```

**Steps of Create simple Node App**

**Step 1** => Create Node

```
npm init -y
```
   
   i) Create File **index.js**

   ii) Add Start Command in package.json file

```
"start": "node index.js"
```

**Step 2** => Create Express server

```
npm install express
```

**Add ECMAScript modules in package.json file**
```
 "type": "module"
```

**Step 3** => import express

```
import express from "express";
```

**Step 4** => Create instance of express

```
const app = express();
```

**Step 5** => Create middleware function for Express

```
app.use(express.json());
```

**Step 6** => Port 
```
app.listen(5000, ()=>{
    console.log("server is runnig on port 5000");
})
```
**Step 7**=> Start your server using following command 

```
npm start
```

**💻 Simple Server Started example**

**filename = index.js**

```html
import express from "express";

const app = express();
app.use(express.json());

app.listen(5000, ()=>{
    console.log("server is runnig on port 5000");
})
```

<img src="./output-1.png" />

**Simple API**

```
app.get('/ping', (req,res)=>{
    res.send("pong");
})
```

**filename = index.js**
```html
import express from "express";

const app = express();
app.use(express.json());

app.get('/ping', (req,res)=>{
    res.send("pong");
})

app.listen(5000, ()=>{
    console.log("server is runnig on port 5000");
})
```
<img src="./output-2.png" />


**filename = index.js**
```html
import express from "express";

const app = express();
app.use(express.json());

app.get('/ping', (req,res)=>{
    res.send("pong");
})

app.get('/coffee', (req,res)=>{
    res.send("Coffee is ready..☕ ")
})

app.get('/pizza', (req,res)=>{
    res.send("pizza is ready..🍕 ")
})

app.listen(5000, ()=>{
    console.log("server is runnig on port 5000");
})
```

<img src="./output-3.png" />
<img src="./output-4.png" />


## Nodemon

Nodemon is a dependency for keeping track of server changes and automatically restarts our app.

**Command to install Nodemon dependency**

```html
npm i nodemon
```

**Send route response in JSON Format**

```
app.get('/coffee', (req,res)=>{
    res.send({
        message: "Coffee is Good"
    });
})
```

 **💻 Example :**
```html
import express from "express";

const app = express();
app.use(express.json());

app.get('/coffee', (req,res)=>{
    res.send({
        name: "cooffe",
        price: 2.5
    });
})

app.listen(5000, ()=>{
    console.log("server is runnig on port 5000");
})

```

<img src="./output-5.png" />

## Get and Post Method


**Get Method** 

To read Resources 

**Post Method**

To create Resources


```html
app.post('/coffee', (req,res)=>{
    res.send({
        name: 'coffee is being made'
    });
})
```

## Reading parameter from request body

```html
app.post('/coffee', (req,res)=>{

    // console.log(req.body);

    const tableNumber  = req.body.tableNumber;
    const coffeeType = req.body.coffeeType

    res.send({
        orderDetails: `Table ${tableNumber} ordered a ${coffeeType}
    }); 
})
```

<img src="./output-7.png" />
<img src="./output-6.png" />

## Query Params






