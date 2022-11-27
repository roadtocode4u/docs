## JSON 

```html
Javascript Object Notations
```
Use of json => Data Protability

## object => 

```html
{
    <key1>:<value>,
    <key2>:<value>
}
```
key is always in string formate. 
value are number, string, boolean, array formate.

**💻Example :**
```html
const colors = {
    red: '#ff0000',
    green: '#00ff00',
    blue: '#0000ff'
}

console.log(colors);
```
**⚙️ Output :**

![Output](output-1.png)  

**💻Example :**
```html
const colors = {
    red: '#ff0000',
    green: '#00ff00',
    blue: '#0000ff'
}

console.log(colors['red']);
```
**⚙️ Output :**

![Output](output-2.png)

**💻Example :**
```html
const students = {
    "Amit": 123,
    "Dikshita": 456,
    "Jayashri": 789,
    "Shubham":211
}

console.log(students["Amit"]);
```
**⚙️ Output :**

![Output](output-3.png)

```html
const students = {
    name: 'John',
    age: 25,
    isActive: true,
    courses: ['html','css','js']
}

console.log(students['age']);
```
**⚙️ Output :**

![Output](output-4.png)

```html
const students = {
    name: 'John',
    age: 25,
    isActive: true,
    courses: ['html','css','js']
}

console.log(students['courses'][0]);
```

**⚙️ Output :**

![Output](output-5.png)

**💻Example :**
```html
const student = {
    name: 'John',
    age: 25,
    isActive: true,
    courses: ['html','css','js']
}

const studentCourses = student["courses"]
studentCourses.push("icp")
console.log(studentCourses);
```
**⚙️ Output :**

![Output](output-6.png)

**💻Example :**
```html
const students = [{
    name: "Chandrabhan",
    age: 23,
    courses: ["React","Node","Mongodb"]
},
{
    name: "Mukesh",
    age: 25,
    courses: ["C","C++","Java"]
},
{
    name: "Punam",
    age: 25,
    courses: ["Python","Django","flask"]
}
]
console.log(students[0]);
```
**⚙️ Output :**

![Output](output-7.png)

**💻Example :**

```html
const students = [{
    name: "Chandrabhan",
    age: 23,
    courses: ["React","Node","Mongodb"]
},
{
    name: "Mukesh",
    age: 25,
    courses: ["C","C++","Java"]
},
{
    name: "Punam",
    age: 25,
    courses: ["Python","Django","flask"]
}
]
console.log(students[0]["courses"]);
```

**⚙️ Output :**

![Output](output-8.png)

**💻Example :**

```html
const students = [{
    name: "Chandrabhan",
    age: 23,
    courses: ["React","Node","Mongodb"]
},
{
    name: "Mukesh",
    age: 25,
    courses: ["C","C++","Java"]
},
{
    name: "Punam",
    age: 25,
    courses: ["Python","Django","flask"]
}
]

students.forEach((students) =>{
    console.log(`Hello ${students['name']}`);
})
```

**⚙️ Output :**

![Output](output-9.png)

**💻Example :**
 
```html
const courses = [{
    title: "Javascript",
    price: 100,
    instructor: "Suraj",
    duration: "2 Month",
    timing: "7 PM",
    isStarted: true
},
{
    title: "React",
    price: 100,
    instructor: "Anand",
    duration: "2 Month",
    timing: "8 PM",
    isStarted: true
},
{
    title: "MongoDB",
    price: 100,
    instructor: "Pinki",
    duration: "2 Month",
    timing: "9 PM",
    isStarted: true
}
]

courses.map((element)=>{
    console.log(element);
})
```
**⚙️ Output :**

![Output](output-10.png)

**💻Example :**

```html
const courses = [{
    title: "Javascript",
    price: 100,
    instructor: "Suraj",
    duration: "2 Month",
    timing: "7 PM",
    isStarted: true
},
{
    title: "React",
    price: 100,
    instructor: "Anand",
    duration: "2 Month",
    timing: "8 PM",
    isStarted: true
},
{
    title: "MongoDB",
    price: 100,
    instructor: "Pinki",
    duration: "2 Month",
    timing: "9 PM",
    isStarted: true
}
]

courses.map((courses)=>{
    console.log(courses['instructor']);
})
```

**⚙️ Output :**

![Output](output-11.png)

**💻Example :**

```html
const courses = [{
    title: "Javascript",
    price: 100,
    instructor: "Suraj",
    duration: "2 Month",
    timing: "7 PM",
    isStarted: true
},
{
    title: "React",
    price: 100,
    instructor: "Anand",
    duration: "2 Month",
    timing: "8 PM",
    isStarted: false
},
{
    title: "MongoDB",
    price: 100,
    instructor: "Pinki",
    duration: "2 Month",
    timing: "9 PM",
    isStarted: false
}
]

courses.map((course) => {
    if (course['isStarted'] == true) {
        console.log(`${course['title']} is live`);
    }
    else {
        console.log(`${course['title']} not live`);
    }
})
```

**⚙️ Output :**

![Output](output-12.png)

