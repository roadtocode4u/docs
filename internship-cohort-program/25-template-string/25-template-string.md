## Template Strings

**💻Example :**
```js
const studentName = "Aniket"
const studentAge = 21

console.log(studentName, " is ", studentAge, " years old")
```

**⚙️ Output :**

>Aniket  is  21  years old

**💻Example :**
```js
const studentName = "Rupal"
const studentAge = 21

const message = studentName + " is " + studentAge + " years old"

console.log(message)
```

**⚙️ Output :**

>Rupal is 21 years old

**💻Example :**
```js
const studentName = "Jagruti"
const studentAge = 22

const message = `${studentName} is ${studentAge} years old`

console.log(message)
```

**⚙️ Output :**

>Jagruti is 22 years old

**💻Example :**
```js
const studentName = "Pradnya"

const message = `Hello ${studentName}, Happy Diwali`

console.log(message)
```

**⚙️ Output :**

>Hello Pradnya, Happy Diwali
