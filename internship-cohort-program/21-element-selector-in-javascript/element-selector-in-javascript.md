## Element Selectors in Javascript

**Case**

1. Camel Case 
   
   ex: HelloWorldBye

   ex: helloWorldBye

2. Snake case 

    ex : hello_world

**Element Selectors in Javascript**

```html
1. getElementById()
2. getElementsByClassName()
3. getElementsByTagName()
````

**getElementById()**

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    <h1 id="heading1">This is Heading 1</h1>

    <h2 id="heading2">This is Heading 2</h2>

    <script>
      const tag = document.getElementById("heading1");
     console.log(tag);
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-1.png) 

**Properties**
1. innerHTML
2. innerText

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    <h1 id="heading1">This is Heading 1</h1>

    <h2 id="heading2">This is Heading 2</h2>


    <script>
      const tag = document.getElementById("heading1");
     console.log(tag.innerText);
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-2.png)  

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    <h1 id="heading1">This is Heading 1</h1>

    <h2 id="heading2">This is Heading 2 <b>Bold</b> </h2>


    <script>
      const tag = document.getElementById("heading2");
     console.log(tag.innerHTML);
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-3.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    <h1 id="heading1">This is Heading 1</h1>

    <h2 id="heading2">This is Heading 2 </h2>

    <script>
      const tag = document.getElementById("heading2");
      tag.innerHTML = "Modified Text"
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-4.png)

**getElementsByClassName()**

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    <h1 id="heading1" class="heading">This is Heading 1</h1>

    <h2 id="heading2" class="heading">This is Heading 2 </h2>

    <script>
      const tags = document.getElementsByClassName("heading");
      console.log(tags);
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-5.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    <h1 id="heading1" class="heading">This is Heading 1</h1>

    <h2 id="heading2" class="heading">This is Heading 2 </h2>

    <script>
      const tags = document.getElementsByClassName("heading");
      console.log(tags[1]);
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-6.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    <h1 id="heading1" class="heading">This is Heading 1</h1>

    <h2 id="heading2" class="heading">This is Heading 2 </h2>

    <script>
      const tags = document.getElementsByClassName("heading");
      tags[0].innerHTML = "First Element";
      tags[1].innerHTML = "Second Element";
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-7.png)

**getElementsByTagName()**

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    
    <b>One</b>
    <b>Two</b>
    <a>Anchor 1</a>
    <a>Anchor 2</a>

    <script>
      const tags = document.getElementsByTagName("b");
      console.log(tags);
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-8.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <title> Javscript </title>
</head>

<body>
    
    <b>One</b>
    <b>Two</b>
    <a>Anchor 1</a>
    <a>Anchor 2</a>

    <script>
      const tags = document.getElementsByTagName("a");
      console.log(tags[1]);
    </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-9.png)

**Query Selector**

```html
1. querySelector() 

👉(use=> For single element)

2. querySelectorAll() 

👉(use=> For multiple element)
```

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
  <title> Javscript </title>
</head>
<body>

  <b> This is bold element 1</b>
  <b> This is bold element 2</b>

  <script>
    const element = document.querySelector("b");
    console.log(element);
  </script>
</body>

</html>
```
**⚙️ Output :**

![Output](output-10.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>

<head>
  <title> Javscript </title>
</head>

<body>

  <b> This is bold element 1</b>
  <b> This is bold element 2</b>

  <script>
    const element = document.querySelectorAll("b");
    console.log(element);
  </script>
</body>

</html>
```
**⚙️ Output :**

![Output](output-11.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>

<head>
  <title> Javscript </title>
</head>

<body>

  <b> This is bold element 1</b>
  <b> This is bold element 2</b>

  <script>
    const element = document.querySelectorAll("b");
    console.log(element[1]);
  </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-12.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>

<head>
  <title> Javscript </title>
</head>

<body>

  <b id="xyz"> This is bold element 1</b>
  <b id="xyz"> This is bold element 2</b>

  <script>
    const element = document.querySelectorAll("#xyz");
    console.log(element);
  </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-13.png)


**💻Example :**
```html
<!DOCTYPE html>
<html>

<head>
  <title> Javscript </title>
</head>

<body>

  <b class="my-text"> This is bold element 1</b>
  <b class="my-text"> This is bold element 2</b>

  <script>
    const element = document.querySelectorAll(".my-text");
    console.log(element);
  </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-14.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
  <title> Javscript </title>
</head>
<style>
  .my-img{
    height: 100px;
  }
</style>
<body>

  <img src="sun.png" class="my-img" />

  <script>
    const imgElement = document.querySelector(".my-img");
    imgElement.src = "moon.png"
  </script>
</body>
</html>
```
**⚙️ Output :**

![Output](output-15.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>

<head>
  <title> Javscript </title>
</head>
<style>
  h1 {
    color: tomato;
  }
</style>

<body>

  <h1> Javascript </h1>

  <script>
    const heading = document.querySelector("h1");
    heading.style.color = "aqua"
  </script>
</body>

</html>
```
**⚙️ Output :**

![Output](output-16.png)

