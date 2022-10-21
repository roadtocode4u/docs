
## Function Overloading and Default Arguments

 ### Function overloading :
 Function Overloading is defined as the process of having two or more function with the same name, but different in parameters is known as function overloading.

  ```cpp
  Trianble 🔼 ->        f1(base , height)
  Reactangle [rect] ->  f2(length , breadth)
  square ⬜ ->          f3 (side)


  Overloading:
  1. No. of parameters
  2. Types of parameters

  cal_area(int a)   cal_area(float b)
  cal_area(5)      cal_area(10.5)
  ```

**💻 Example 1️⃣ :**
```cpp
#include <iostream>
using namespace std;

void show(int num)
{
    cout<<"int value is"<<num<<endl;
}
void show(float num)
{
    cout<<"float value is"<<num<<endl;
}
int main() {
    show(10);
    show(15.3f)
    
    return 0;
}
```
**⚙️ Output :**
>int value is: 10<br>
float value is: 15.3

**💻 Example 2️⃣ :**
```cpp
    cal_area(int r)   cal_area(int a , int b)
    cal_area(10)      cal_area(5,10)
```
```cpp
#include <iostream>
using namespace std;

void cal_area(int r)
{
    cout<<"Radius of circle is:"<<r<<endl;
}
void cal_area(int l,int b)
{
    cout<<"Length: "<l<<"Breadth: "<<b<<endl;
}
int main() {
   
    cal_area(10)
    cal_area(5,10)
    return 0;
}
```
**⚙️ Output :**
>Radius of circle is: 10<br>
Length: 5 Breadth:10

## Default Argument :
* The values passed in the default arguments are not constant. These values can be overwritten if the value is passed to the function. If not, the previously declared value retains.
* During the calling of function, the values are copied from left to right
* All the values that will be given default value will be on the right.
```cpp
default argument :

void fun(int num=10) //bydefault value is 10
{

}
fun(20)

void fun(int num) //argument
{

}
fun(10) // parameter
```

**💻 Example 3️⃣ : bydeafult value**
```cpp
#include <iostream>
using namespace std;

void show_value(int num=10)
{
    cout<<"value  of num is:"<<num<<endl;
}
int main() {
    show_value();
    
    return 0;
}
```
**⚙️ Output :**
>value  of num is: 10

**💻 Example 4️⃣ :**
```cpp
#include <iostream>
using namespace std;

void show_value(int num=10)
{
    cout<<"value  of num is:"<<num<<endl;
}
int main() {
    show_value(5);
    
    return 0;
}
```
**⚙️ Output :**
>value  of num is: 5

**💻 Example 5️⃣ :**
```cpp
#include <iostream>
using namespace std;

void show_value(int x, int y)
{
    cout<<"X: "<<x<<"Y: "<<y<<endl;
}
int main() {
    show_value(8,4);
    
    return 0;
}
```
**⚙️ Output :**
>X: 8 Y: 4


**💻 Example 6️⃣ : bydefault value**
```cpp
#include <iostream>
using namespace std;

void show_value(int x, int y=8)
{
    cout<<"X: "<<x<<"Y: "<<y<<endl;
}
int main() {
    show_value(4);
    
    return 0;
}
```
**⚙️ Output :**
>X=4 Y=8

**💻 Example 7️⃣ :**
```cpp
#include <iostream>
using namespace std;

void show_value(int x, int y=8)
{
    cout<<"X: "<<x<<"Y: "<<y<<endl;
}
int main() {
    show_value(4, 12);
    
    return 0;
}
```
**⚙️ Output :**
>X=4 Y=12

## 🏠  HomeWork
\
## 🔗 Some Useful Links

## 📖 References