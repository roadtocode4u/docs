
# Assignment Operators & Relational Operators

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


## 2. Assignment Operator: (=, +=, -=,...)
ex : int a = 10;

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a=5; // assignment operator
    
    cout<<a;

    return 0;
}
```
**⚙️ Output :**
>5

**💻 Example 2 : Addition of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a=10;
    // num = num + 5;
   or
    a += 5;

    cout<<a;

    return 0;
}
```
**⚙️ Output :**
>15

**💻 Example 3 : Subtraction of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num=20;
   // num = num -5;
   or
   num -=5; 

    cout<<num;

    return 0;
}
```
**⚙️ Output :**
>15
 

**💻 Example 4 : Multiplication of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num=10;
   // num = num * 2;
   or
   num *=5; 

    cout<<num;

    return 0;
}
```
**⚙️ Output :**
>20
 

**💻 Example 5: Division of two numbers**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int num=10;
   // num = num /2;
   or
   num /=2; 

    cout<<num;

    return 0;
}
```
**⚙️ Output :**
>5

## % Modulus Operator : 

**💻 Example 6 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
     int num = 10;
   // num = num % 3;
   or
   num %=3; 

    cout<<num;
    
    return 0;
}
```
**⚙️ Output :**
>1

## Short hand : 
```cpp
num = num [] value //[+, -, *, /, %]

=> num[]=value;

ex: num[+]=5;
```

```cpp
* Boolean Value:

True  represent 1

False represent 0
```
## 3. Relational Operator : (>,<,>=,<=,==)
* comparision
* true / false value
```cpp
  1. == is equals to
ex : a == b // == comparision

a = b // value assign

two values are equal then result is true

two values are differebt then result is false
```


**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a = 5;

    int b = 5;

    int res = a==b;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1 

**💻 Example 2 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a = 15;

    int b = 5;

    int res = a==b;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>0

```
2. != Not equals to
ex : a !=b // result false
```
**💻 Example 3 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a = 15;

    int b = 5;

    int res = a!=b;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 4 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a = 15;

    int b = 15;

    int res = a!=b;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>0

```
3. < less than
ex : a < b (a is less than b)
a<b => true
```
**💻 Example 5 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a = 17;

    int b= 20;

    int res = a<b;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1


**💻 Example 6 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a = 17;

    int b= 20;

    int res = b<a;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>0

```
3. > greater than
ex : a > b (a is greater than b)
a>b => true
```

**💻 Example 7 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 170>20;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 8 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 20>170;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>0

```
4. >= greater than or equal to
ex : a >= b (a is greater than or equals to b)
a>=b => true
```
**💻 Example 9 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 5>=2;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 10 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 2>=2;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 11 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 1>=2;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>0

```
5. <= less than or equal to
ex : a <= b (a is less than or equals to b)
a<=b => true
```
**💻 Example 12 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 5<=10;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 13 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 10<=10;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 14 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int res = 15<=10;

    cout<<res;
 
    return 0;
}
```
**⚙️ Output :**
>0

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References
