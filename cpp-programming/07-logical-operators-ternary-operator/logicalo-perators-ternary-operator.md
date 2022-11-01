
# Logical Operators & Ternary Operator 

## 4. Logical Operator : (&&,||, !)
```cpp
 1. Logical AND  => &&
 2. Logical OR =>  ||
 3. Logical NOT(Negation) => !
```
```cpp
1. Logical AND (&&) 

**Truth Table**
(condition 1 && condition 2)
 T   T => T
 T   F => F
 F   T => F
 F   F => F
 ```

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int a = 5;

   int b = 8;
   
   int res =  a==5 &&b==a;

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
   
   int a = 5;
   
   int res =  a>5 &&a<20;

   cout<<res;

   return 0;
}
```
**⚙️ Output :**
>0

**💻 Example 3 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int a = 5;
   
   int res =  a==5 &&a<20;

   cout<<res;

   return 0;
}
```
**⚙️ Output :**
>0

**💻 Example 4 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int a = 5;
   
   int res =  a==8 &&a==10;

   cout<<res;

   return 0;
}
```
**⚙️ Output :**
>0

```cpp
2. Logical OR (||) 

**Truth Table**
(condition 1 || condition 2)
 T   T => T
 T   F => T
 F   T => T
 F   F => F
 ```

 **💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int jee = 130;

   int cet = 20;

   int res = jee >= 120 || cet >= 200;

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
   
   int jee = 0;

   int cet = 220;

   int res = jee >= 120 || cet >= 200;

   cout<<res;

   return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 3 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int jee = 125;

   int cet = 220;

   int res = jee >= 120 || cet >= 200;

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
   
   int jee = 0;

   int cet = 0;

   int res = jee >= 120 || cet >= 200;

   cout<<res;

   return 0;
}
```
**⚙️ Output :**
>0

```cpp
3. Logical NOT/ NEGATION  (!) 
 ```

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int jee = 0;

   int res = jee >= 120;

   cout<<res;

   return 0;
}
```
**⚙️ Output :**
>0

**💻 Example 2 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int jee = 0;

   int res = !(jee >= 120);

   cout<<res;

   return 0;
}
```
**⚙️ Output :**
>1

**💻 Example 3 :**
```cpp
#include <iostream>
using namespace std;

int main() {
   
   int jee = 125;

   int res = (jee >= 120);

   cout<<!res;

   return 0;
}
```
**⚙️ Output :**
>0

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

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References



