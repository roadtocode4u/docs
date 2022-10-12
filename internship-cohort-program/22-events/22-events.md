## Events in Javascript

JavaScript interacts with HTML through events when the browser manipulates the page. When a page loads, it's called an event. When user clicks on a button, that click is also an event.

**Types of events in javascript**

* onClick
* onChange
* onmouseover
* onmouseout
* onkeydown
* onload

**onClick**

The onClick event occurs when the user clicks on an element.

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <script>

    </script>
</head>
<body>
    <button onClick="console.log('Button is clicked..')">Click Me</button>
</body>
</html>
```
**⚙️ Output :**

![Output](output-1.png)


**function**

The function is a block of code that is executed when the event occurs.

**Syntax :**

```javascript

function functionName() {
    // code to be executed
}

```

**💻Example :**
```javascript
function clickMe()
{
    console.log('Clicked..')
}

clickMe()
clickMe()
clickMe()
```

**⚙️ Output :**

> Clicked..<br>
Clicked..<br>
Clicked..

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <script>
        function clickMe() 
        {
            console.log('Clicked..');
        }
    </script>
</head>
<body>
    <button onClick="clickMe()">Click here</button>
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
    <script>
        let count = 0;
        function clickMe() 
        {
            count++;
            console.log('Clicked '+count+' times...')
        }
    </script>
</head>
<body>
    <button onClick="clickMe()">Click here</button>
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
    <script>
        let count = 0;
        function clickMe() 
        {
            count++;
            document.getElementById('counter').innerHTML = count;
        }
    </script>
</head>
<body>
    <h1 id="counter">0</h1>

    <button onClick="clickMe()">Tap Me</button>
</body>
</html>
```

**⚙️ Output :**

![Output](output-4.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <script>
        let count = 0;
        function clickMe() 
        {
            count++;
            document.getElementById('counter').innerHTML = count;
        }

        function reset() 
        {
            count = 0;
            document.getElementById('counter').innerHTML = count;
        }
    </script>
</head>
<body>
    <h1 id="counter">0</h1>

    <button onClick="clickMe()">Tap Me</button>
    <button onClick="reset()">Reset to Zero</button>
</body>
</html>
```

**⚙️ Output :**

![Output](output-5.png)

![Output](output-6.png)

**💻Example :**
```html
<!DOCTYPE html>
<html>
<head>
    <script>
        let count = 0;
        function inc()
        {
            count++;
            document.getElementById('counter').innerHTML = count;
        }

        function reset() 
        {
            count = 0;
            document.getElementById('counter').innerHTML = count;
        }

        function dec()
        {
            count--;
            document.getElementById('counter').innerHTML = count;
        }
    </script>
</head>
<body>
    <h1 id="counter">0</h1>

    <button onClick="inc()">+</button>
    <button onClick="reset()">Reset to Zero</button>
    <button onClick="dec()">-</button>
</body>
</html>
```

**⚙️ Output :**

![Output](output-7.png)

![Output](output-8.png)

![Output](output-9.png)
