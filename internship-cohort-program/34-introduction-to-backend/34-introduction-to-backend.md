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

````

## APIs

 **Application Program Interface**

**Frontend**
 ![frontend](frontend.png)

**API**
 ![api](api.png) 
    
**Backend**
 ![backend](backend.png)

```
 API are acts as an intermediary between frontend and backend.
 
  
```

**Create Node App Step**

**Step 1** => npm init -y

   i) Create File **index.js**

   ii) Add Start Command in package.json file

**Step 2** => npm install express

    i) "type": "module"

**Create API Step**

Step 1 => import express

Step 2 => Create instance of express


**filename = index.js**

```html
import express from "express";

const app = express();
app.use(express.json());

app.listen(5000, ()=>{
    console.log("server is runnig on port 5000");
})
```

![output](output-1.png)

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
![output](output-2.png)


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

![output](output-3.png)

