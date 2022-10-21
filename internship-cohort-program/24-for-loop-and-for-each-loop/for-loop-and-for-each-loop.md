## For loop and for each loop

## 🤔How to iterate over array elements?

### For loop

**💻Example :**

```js
const arr = ["A", "B", "C", "D", "E"];

for (let i = 0; i <= arr.length; i++) {
  console.log(arr[i]);
}
```

**⚙️ Output :**

>A<br>
B<br>
C<br>
D<br>
E<br>
F<br>

**💻Example :**
```js
const arr = ["A", "B", "C", "D", "E", "F"];

for (let i = 0; i < arr.length; i++) {
  console.log("Prasad for =>" + arr[i]);
}
```
**⚙️ Output :**

>Prasad for =>A<br>
Prasad for =>B<br>
Prasad for =>C<br>
Prasad for =>D<br>
Prasad for =>E<br>
Prasad for =>F<br>

**💻Example :**
```js
const arr = [1, 2, 3, 4];

for (let i = 0; i < arr.length; i++) {
    console.log(arr[i]*arr[i]);
}
```

**⚙️ Output :**

>1<br>
4<br>
9<br>
16<br>

**💻Example :**
```js
const arr = ["Aniket", "Pradnya", "Sakshi", "Mukesh", "Rohit"];

for (let i = 0; i < arr.length; i++) {
    console.log("Sending email to " + arr[i]);
}
```

**⚙️ Output :**

>Sending email to Aniket<br>
Sending email to Pradnya<br>
Sending email to Sakshi<br>
Sending email to Mukesh<br>
Sending email to Rohit<br>

### For each loop

arror function

**syntax :**

```js
() =>{
    //code
}
```

**💻Example :**
```js
const arr = ["Aniket", "Pradnya", "Sakshi", "Mukesh", "Rohit"];

arr.forEach(() => {
    console.log("A")
})
```

**⚙️ Output :**

>A<br>
A<br>
A<br>
A<br>
A<br>

**💻Example :**
```js
const students = ["Aniket", "Pradnya", "Sakshi", "Mukesh", "Rohit"];

students.forEach((item, index) => {
    console.log(item, index)
})
```

**⚙️ Output :**

>Aniket 0<br>
Pradnya 1<br>
Sakshi 2<br>
Mukesh 3<br>
Rohit 4<br>


**💻Example :**
```js
const students = ["Aniket", "Pradnya", "Sakshi", "Mukesh", "Rohit"];

students.forEach((item, index) => {
    console.log("Sending email to ", item)
})
```

**⚙️ Output :**

>Sending email to  Aniket<br>
Sending email to  Pradnya<br>
Sending email to  Sakshi<br>
Sending email to  Mukesh<br>
Sending email to  Rohit<br>

**💻Example :**
```js
const students = ["Aniket", "Pradnya", "Sakshi", "Mukesh", "Rohit"];

function sendEmail(student, index){
    console.log("Sending email to " + student)
}

students.forEach(sendEmail)
```

**⚙️ Output :**

>Sending email to Aniket<br>
Sending email to Pradnya<br>
Sending email to Sakshi<br>
Sending email to Mukesh<br>
Sending email to Rohit<br>

**💻Example :**
```js
const students = ["Aniket", "Pradnya", "Sakshi", "Mukesh", "Rohit"];

students.forEach((student, index) => {
    console.log("Sending email to " + student)
})

sendEmail("Sayali", -1)
```

**⚙️ Output :**

>Sending email to Aniket<br>
Sending email to Pradnya<br>
Sending email to Sakshi<br>
Sending email to Mukesh<br>
Sending email to Rohit<br>
sendEmail("Sayali", -1)<br>
^
<br>
ReferenceError: sendEmail is not defined

