# Data types and Sizeof Operator

## Data types

Data type is an inbuilt keyword that defines the type of a variable.

There are five data types : void, int, float, double, and char.

```cpp
   ________ bit                             
  |                          | | | |                        
 [1]                        [][][][]
                            |______|
                                |
                              nibble

int --> integer  (2 or 4 bytes)

```                          
```cpp
8 bit --> 1 byte
1024 bytes --> 1 kb => kilobyte
1024 kb --> 1 mb => megabyte
1024 mb --> 1 gb => gigabyte
1024 gb --> 1 tb
```
 
## unsigned int

*Unsigned int is used to store 32-bit integers. The keyword unsigned is a data type specifier, which only represents non-negative integers.*

```cpp
int --> 4 byte
short int --> 2 byte

limit of short int --> -32768 to +32767
```

WAP to find out maximum limit of float

**💻Example 1️:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    cout<<FLT_MAX;
    
    return 0;
}
    
```
**⚙️ Output :**
>3.40282e+38

WAP to find out minimum limit of float

**💻Example 2:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    cout<<FLT_MIN;
    
    return 0;
}
```
**⚙️ Output :**
>1.17549e-38

WAP to find out minimum limit of double


**💻Example 3:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    cout<<DBL_MAX;
    
    return 0;
}
```
**⚙️ Output :**
>1.79769e+308

WAP to find out minimum limit of double

**💻Example 4:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    cout<<DBL_MIN;
    
    return 0;
}
    
```
**⚙️ Output :**
>2.22507e-308


## Boolean

*The Boolean data type is used to declare a variable whose value will be set as true (1) or false (0).*

**💻Example 5:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    bool flag = true;
    
    cout<<flag;
    
    return 0;
}
```
**⚙️ Output :**
>1

**💻Example 6:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    bool flag = false;
    
    cout<<flag;
    
    return 0;
}   
```
**⚙️ Output :**
>0

WAP to check flag size in bool

**💻Example 7:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    bool flag = false;
    
    cout<<sizeof(flag);
    
    return 0;
}
```
**⚙️ Output :**
>1

WAP to check value of int

**💻Example 8:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    int num = 10;
    
    cout<<sizeof(num);
    
    return 0;
}
```
**⚙️ Output :**
>4

WAP to check value of char

**💻Example 9:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    char a;
    
    cout<<sizeof(a);
    
    return 0;
}
```
**⚙️ Output :**
>1

WAP to check value of float

**💻Example 10:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    float num;
    
    cout<<sizeof(num);
    
    return 0;
}
```
**⚙️ Output :**
>4

WAP to check value of double

**💻Example 11:**
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    
    double num;
    
    cout<<sizeof(num);
    
    return 0;
}
```
**⚙️ Output :**
>8

## Void

*The void keyword specifies that the function doesn't return a value.*

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References
