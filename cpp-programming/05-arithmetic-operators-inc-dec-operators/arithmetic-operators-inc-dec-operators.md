
# Arithmetic Operators, Inc/Dec Operators

**Operators :**  

```cpp
Doctor ---> Operator

patients ---> Operand

ex : a+b
 + ---> operator
 a,b ---> operand
```

## Types of Operator
1. Arithmetic Operator :  (-, +, /, *, %)
2. Assignment Operator : (=, +=, -=,...)
3. Relational Operator : (>,<,>=,<=,==)
4. Logical Operator: (&&,||, !)
5. Bitwise Operator


## 1.Arithmetic Operator:

```
+ ---> Addition
- ---> Subtraction
* ---> Multiplication
/ ---> Division
% ---> Modules
```

**💻 Example 1 : Addition of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a=5;
    int b=10;

    int result = a + b;
    cout<<result;

    return 0;
}
```
**⚙️ Output :**
>15


**💻 Example 2 : Subtraction of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a=20;
    int b=10;

    int result = a - b;
    cout<<result;

    return 0;
}
```
**⚙️ Output :**
>10

**💻 Example 3 : Multiplication of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a=55;
    int b=2;

    int result = a * b;
    cout<<result;

    return 0;
}
```
**⚙️ Output :**
>110

**💻 Example 4: Division of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a=55;
    int b=2;

    int result = a / b;
    cout<<result;

    return 0;
}
```
**⚙️ Output :**
>27

## % Modulus Operator : 
* It calculates reminder after the integer division

**💻 Example 5 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int result = 22 % 5;
    cout<<result;

    return 0;
}
```
**⚙️ Output :**
>2


```cpp
odd number : 3,7,9
odd % 2 = 1
ex:
3 % 2 = 1
7 % 2 = 1
9 % 2 = 1

even number:4,8,10
even % 2 = 0
ex :
4 % 2 = 0
8 % 2 = 0
10 % 2 = 0
```
 ## Increment Operator & Decrement Operator

 ```cpp
* Inc Operator : 
1. Pre-Increment
ex : ++num; 
(first increase then use)
2. Post-Increment
ex : num++;
(first use then increase)

* Dec Operator : 
1. Pre-Decrement
ex : --num;
(first decrease then use)
2. Post-Decrement
ex : num--;
(first use then decrease)
 ```

**💻 Example 6 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int count=0;

    count = count + 1;
    cout<<count;
 
    return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 7 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int count=0;

    count = count + 1;

    count = count + 1;
    cout<<count;
 
    return 0;
}
```
**⚙️ Output :**
>2

**💻 Example 8 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int count=5;

    count++;
    count++;

    cout<<count;
 
    return 0;
}
```
**⚙️ Output :**
>7

**💻 Example 9 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int count=5;

    int res = ++count;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>6

**💻 Example 10 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int count=5;

    int res = count++;

    cout<<res<<endl;
    cout<<"Count: "<<count;
 
    return 0;
}
```
**⚙️ Output :**
>5 <br>
Count : 6

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References



