# if and if-else

### Comments in C++ : 
```
* compiler ---> ignore

* programmer ---> redability
```
 **Two Types of Comments :**
1. single line comments <br>
// comment text

2. multiple text <br>
/* ------- */

```
1. Single Line Comment : 
// this is single line Comment

2. Multiple Line Comment : 
/*
function to calculate simple interest
int cal_si(p,r,t)
{
 ----
 ----
 ----
} 
*/
```

**💻 Example 1 : example of ternary operator**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    cout<<"Enter Number : ";
    cin>>num;

    num%2==1 ? cout<<"Number is Odd" : cout<<"Number is Even";

    return 0
}
```
**⚙️ Output :**
>Enter Number : 10<br>
Number is Even

## Conditional Statements : 
There are Four Types : 
1. if 
2. if-else
3. if-else-ladder
4. nested-if

```cpp
1. if
syntax : 

if (condition)
{
    //-----
    //-----
}
```

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    cout<<"Enter Number : ";
    cin>>num;

    if(num>0){
        cout<<"Positive Number";
    }

    return 0
}
```
**⚙️ Output :**
>Enter Number : 5<br>
Positive Number

```cpp
2. if-else
syntax : 
 if (condition)
{
    // True
}
else
{
    //----
    //----
}
```

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    cout<<"Enter Number : ";
    cin>>num;

    if(num%2==0){
        cout<<"Number is Even";
    }
    else{
        cout<<"Number is Odd";
    }

    return 0
}
```
**⚙️ Output :**
>Enter Number : 5 <br>
Number is odd

**💻 Example 2 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    cout<<"Enter Number : ";
    cin>>num;

    if(num%2==0){
        cout<<"Number is Even";
    }
    else{
        cout<<"Number is Odd";
    }

    return 0
}
```
**⚙️ Output :**
>Enter Number : 4 <br>
Number is Even

**💻 Example 3 :** 
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    cout<<"Enter Number : ";
    cin>>num;

    if(num%3==0 && num%5==0){
        cout<<"Number is divisible by 5 & 3";
    }
    else{
        cout<<"Number is NOT divisible by 5 & 3";
    }

    return 0
}
```
**⚙️ Output :**
>Enter Number : 15<br>
Number is divisible by 5 & 3


**💻 Example 4 :** 
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    cout<<"Enter Number : ";
    cin>>num;

    if(num%3==0 && num%5==0){
        cout<<"Number is divisible by 5 & 3";
    }
    else{
        cout<<"Number is NOT divisible by 5 & 3";
    }

    return 0
}
```
**⚙️ Output :**
>Enter Number : 3<br>
Number is NOT divisible by 5 & 3

**💻 Example 5 :** 
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;

    cout<<"Enter Number : ";
    cin>>num;

    if(num%3==0 || num%5==0){
        cout<<"Number is divisible by 5 or 3";
    }
    else{
        cout<<"Number is NOT divisible by 5 or 3";
    }

    return 0
}
```
**⚙️ Output :**
>Enter Number : 15<br>
Number is divisible by 5 or 3

**💻 Example 3 :** 
```cpp
#include <iostream>
using namespace std;

int main() {
    int rate,quantity;

    cout<<"Enter rate & Quantity : ";
    cin>>rate>>quantity;

    int bill = rate * quantity

     cout<<"Bill: "<<bill;
    
    return 0
}
```

**⚙️ Output :**
>Enter Rate & Quantity : 5  3<br>
Bill 15

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References



