
# Taking input from user

**Data Types :**  Which type of Data are stored in variable .

```cpp
 int age; //declaration

 age = 30; //assign value

 age = 40; //assign value

 example : int age = 20;
```

## How to declared value in C programming and C++
```c
C programmimg : 

int age = 20;
printf("%d", age);

C++ : 

int age = 20;
cout<<age;
```

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int age = 20;

    cout<<"Age =";

    cout<<age; 

    return 0;
}
```
**⚙️ Output :**
>Age = 20


**💻 Example 2 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int age = 22;

    cout<<"My age is "<<age;

    return 0;
}
```
**⚙️ Output :**
>my age is 22

**💻 Example 3 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int age = 20;
    int weight = 50;

    cout<<"My age is"<<age<<"& Weight is"<<weight;
 
    return 0;
}
```
**⚙️ Output :**
>My age is 20 & weight is 50

### Console input

```cpp
console ----> input

cout<<"Enter age"
cin>>age;

>> ---> extraction operator 
```

**💻 Example 4 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int age;

    cout<<"Enter Age:";
    cin>>age;

    cout<<age;
 
    return 0;
}
```
**⚙️ Output :**
>Enter Age: 8<br>
8

## WAP to print sum of numbers by taking values from user

**💻 Example 5 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int num1;
    int num2;

    cout<<"Enter num1:";
    cin>>num1;

    cout<<"Enter num2:";
    cin>>num2;

    int sum = num1 + num2;

    cout<<"Sum ="<<sum;
 
    return 0;
}
```
**⚙️ Output :**
>Enter num1: 5<br>
Enter num2: 7<br>
Sum = 12

## Area of Reactangle

**💻 Example 6 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int l;
    int b;

    cout<<"Enter length:";
    cin>>l;

    cout<<"Enter breadth:";
    cin>>b;

    int area = l * b;

    cout<<"Area = "<<area;
    return 0;
}
```
**⚙️ Output :**
>Enter length: 8<br>
Enter breadth: 4<br>
Area = 32
 
## 🏠  HomeWork
>1️⃣ WAP to calculate Simple interest by taking values of P,R, & T from user<br>

>2️⃣ WAP to calculate area of triangle when base  & height is given by user

>3️⃣ WAP to calculate perimeter of circle when radius is given by user

## 🔗 Some Useful Links

## 📖 References
