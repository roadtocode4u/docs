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

**Promise**

Promise is an object that represents the eventual completion or failure of an asynchronous operation. 

**resolve and reject**

resolve and reject are functions that can be used to resolve or reject a promise.

**resolve**

resolve() is a function that is used to resolve a promise. It takes a single argument which is the value that the promise will be resolved with.

**reject**

reject() is a function that is used to reject a promise. It takes a single argument which is the value that the promise will be rejected with.

**💻Example :**

```js
async function main(){
  setTimeout(() => {
    console.log("Sentence A");
  }, 3000);
  console.log("Sentence B");
}
main();
```

**⚙️ Output :**

> Sentence B<br>
> Sentence A

**💻Example :**

```js
async function calBill(){
  const bill = 100;
  return 100;
}

async function calTax(bill){
  const tax = bill + 18;
  return tax;
}

const bill = calBill();
console.log('Bill', bill);

const tax = calTax(bill);
console.log('Tax', tax);
```

**⚙️ Output :**

> Bill Promise { 100 }<br>
> Tax Promise { '[object Promise]18' }

**💻Example :**

```js
async function calBill(){
  const bill = 100;
  return 100;
}

async function calTax(bill){
  const tax = bill + 18;
  return tax;
}

async function main(){
  const bill = await calBill();
  console.log('Bill', bill);

  const tax = await calTax(bill);
  console.log('Tax', tax);
}

main();
```

**⚙️ Output :**

> Bill 100<br>
> Tax 118

**💻Example :**

```js
async function calBill(){
  return new Promise((resolve, reject)=>{
  })
}

const bill = calBill();
console.log('Bill', bill);
```

**⚙️ Output :**

> Bill Promise { \<pending\> }

**💻Example :**

```js
async function calBill(){
    return new Promise((resolve, reject)=>{
      const bill = 100;
      resolve(bill);
    })
  }
  
  async function main() {
    const bill = await calBill();
    console.log(bill);
  }
main();
```

**⚙️ Output :**

> 100

**💻Example :**

```js
async function calBill(){
    return new Promise((resolve, reject)=>{
      reject("Bill not found");
    })
    }

async function main() {
    const bill = await calBill();
    console.log(bill);
}
main();

```

**⚙️ Output :**

> Uncaught (in promise) Bill not found

**💻Example :**

```js
async function calBill(){
    return new Promise((resolve, reject)=>{
      reject(new Error("Bill not found"));
    })
    }

async function main() {
    const bill = await calBill();
    console.log(bill);
}
main();
  
```

**⚙️ Output :**

> Error: Bill not found

**💻Example :**

```js
async function calBill(bill){
    return new Promise((resolve, reject)=>{
      if(bill%2 === 0){
        resolve(bill);
      }
        else{
            reject(new Error("Invalid bill"));
        }
    })
    }

async function main() {
    const bill = await calBill(100);
    console.log(bill);
}
main();

```

**⚙️ Output :**

> 100

**💻Example :**

```js
async function calBill(bill){
    return new Promise((resolve, reject)=>{
      if(bill%2 === 0){
        resolve(bill);
      }
        else{
            reject(new Error("Invalid bill"));
        }
    })
    }

async function main() {
    const bill = await calBill(101);
    console.log(bill);
}
main();

```

**⚙️ Output :**

> Uncaught (in promise) Error: Invalid bill

**💻Example :**

```js
async function calBill(bill){
    return new Promise((resolve, reject)=>{
      if(bill%2 === 0){
        resolve(bill);
      }
        else{
            reject(new Error("Invalid bill"));
        }
    })
    }

async function main() {
    const bill = calBill(100);
    console.log(bill);
}
main();

```

**⚙️ Output :**

> Promise { <pending> }

**Date**

Date is a built-in object that provides functionality to work with dates and times.

**💻Example :**

```js
const date = new Date();
console.log(date);
```

**⚙️ Output :**

> 2022-11-04T14:39:57.380Z

**🤔 How to convert date to string?**

**💻Example :**

```js
const date = new Date();
console.log(date.toDateString());
```

**⚙️ Output :**

> Fri Nov 04 2022

**💻Example :**

```js
const date = new Date();
console.log(date.toString());
```

**⚙️ Output :**

> Fri Nov 04 2022 20:16:09 GMT+0530 (India Standard Time)

**💻Example :**

```js
const date = new Date();
console.log(date.toUTCString());
```

**⚙️ Output :**

> Fri, 04 Nov 2022 14:47:35 GMT

**💻Example :**

```js
const date = new Date();
console.log(date.toISOString());
```

**⚙️ Output :**

> 2022-11-04T14:48:49.995Z

**💻Example :**

```js
const date = new Date();
console.log(date.getFullYear());
```

**⚙️ Output :**

> 2022

**💻Example :**

```js
const date = new Date();
console.log(date.getHours());
```

**⚙️ Output :**

> 20

**💻Example :**

```js
const date = new Date();
console.log(date.geTDates());
```

**⚙️ Output :**

> 4

**💻Example :**

```js
const date = new Date();
console.log(date.getMonth());
```

**⚙️ Output :**

> 10
