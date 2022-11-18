## Special Operators : 
1. Ternary operator (? :)
```cpp
example :
condition ? true part : false part
```
**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int num = 10;

   num==10 ? cout<<"Equal" : cout<<"Not Equal";

   return 0;
}
```
**⚙️ Output :**
>Equal

**💻 Example 2 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int num = 15;

   num==10 ? cout<<"Equal" : cout<<"Not Equal";

   return 0;
}
```
**⚙️ Output :**
> Not Equal

**💻 Example 3 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int a = 5;
   int b = 8;

   int big =a>b ? a : b

   cout<<big;

   return 0;
}
```
**⚙️ Output :**
>8

**💻 Example 4 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int a = 50;
   int b = 8;

   int big =a>b ? a : b

   cout<<big;

   return 0;
}
```
**⚙️ Output :**
>50


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
 