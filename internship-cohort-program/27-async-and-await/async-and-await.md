## Set Timeout

setTimeout() is a function that takes two arguments: a callback function and a time in milliseconds. The callback function will be called after the time has passed.

**💻Example :**

```js
setTimeout(() => {
  console.log("Hello World");
}, 2000);
```

**⚙️ Output :**

> Hello World

**💻Example :**

```js
setTimeout(() => {
  console.log("Printing after 3 seconds");
}, 3000);
```

**Output:**

> Printing after 3 seconds

The above code will print "Hello World" after 2 seconds.

**sync and async**

Sync and async are keywords that can be used with a function to specify whether the process should be executed synchronously or asynchronously.

**sync** 

Synchronous functions are executed one after the other. The next function will not be executed until the previous function has finished executing.

**💻Example :**

```js
console.log("Person 1");
console.log("Person 2");
console.log("Person 3");
console.log("Person 4");
```

**⚙️ Output :**

> Person 1<br>
> Person 2<br>
> Person 3<br>
> Person 4

**💻Example :**

```js
function fun1() {
  console.log("Func 1");
}
function fun2() {
  console.log("Func 2");
}

fun1();
fun2();
```

**⚙️ Output :**

> Func 1<br>
> Func 2

**💻Example :**

```js
function fetchExamSchedule() {
  console.log("Fetching exam schedule");
}

function fetchPaymentInformation() {
  console.log("Fetching payment information");
}

fetchExamSchedule();
fetchPaymentInformation();
```

**⚙️ Output :**

> Fetching exam schedule<br>
> Fetching payment information

**async**

Asynchronous functions are executed at the same time. The next function will be executed even if the previous function has not finished executing.

**💻Example :**

```js
console.log("Person 1");

setTimeout(() => {
  console.log("Person 2");
}, 3000);

console.log("Person 3");
```

**⚙️ Output :**

> Person 1<br>
> Person 3<br>
> Person 2

**💻Example :**

```js
async function fun1() {
  console.log("Func 1");
}
async function fun2() {
  console.log("Func 2");
}

fun1();
fun2();
```

**⚙️ Output :**

> Func 1<br>
> Func 2

**💻Example :**

```js
async function fetchExamSchedule() {
  console.log("Fetching exam schedule");
}

async function fetchPaymentInformation() {
  console.log("Fetching payment information");
}

fetchPaymentInformation();
fetchExamSchedule();
```

**⚙️ Output :**

> Fetching payment information<br>
> Fetching exam schedule

**💻Example :**

```js
async function fetchExamSchedule() {
  return "Fetching exam schedule";
}

async function fetchPaymentInformation() {
  return "Fetching payment information";
}

const examSchedule = fetchExamSchedule();
console.log(examSchedule);

const paymentInformation = fetchPaymentInformation();
console.log(paymentInformation);
```

**⚙️ Output :**

> Promise { 'Fetching exam schedule' }<br>
> Promise { 'Fetching payment information' }

**💻Example :**

```js
async function fetchExamSchedule() {
  for (let i = 0; i < 1000000000; i++) {}
  return "Fetching exam schedule";
}

async function fetchPaymentInformation() {
  return "Fetching payment information";
}

const examSchedule = fetchExamSchedule();
console.log(examSchedule);

const paymentInformation = fetchPaymentInformation();
console.log(paymentInformation);
```

**⚙️ Output :**

> Promise { 'Fetching exam schedule' }<br>
> Fetching payment information

**💻Example :**

```js
async function fetchExamSchedule() {
  return "Fetching exam schedule";
}

async function fetchPaymentInformation() {
  return "Fetching payment information";
}

async function main() {
  const examSchedule = await fetchExamSchedule();
  console.log(examSchedule);

  const paymentInformation = await fetchPaymentInformation();
  console.log(paymentInformation);
}

main();
```

**⚙️ Output :**

> Fetching exam schedule<br>
> Fetching payment information
