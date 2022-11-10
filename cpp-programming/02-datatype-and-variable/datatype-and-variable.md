# Datatypes & Variables

## variables & constants
* variables : it changes<br> (in programing language data stored in variable)<br>

* constant : it does not change

## DataTypes : which type of data to be stored in variable

 **Example 1 :** 1 , 2 , 3 , 4 ---> integer , int <br>
  **Example 2 :** 7.2 , 8.4 , 3.5 , 4.3 ---> floating , float  <br>
**Example 3 :** 'a' , 'z' , 'v' , 'b' ---> charecter  , char  <br>

`char int and float` that is data types stored in variable

## How to define variable 
```
<datatype> <variable_name>;
int          age;
```
```
<char> <variable_name>;
char          gender;
```
```
<float> <variable_name>;
float          weight;
```
**💻 Example 3 :**
```cpp

#include <iostream>
using namespace std;

int main() {
    
    int age; //declaration
    
    age = 22; //assign value

    cout<<age; 

    return 0;
}
```
**⚙️ Output :**
>22
 

**💻 Addition of  Two Number :**
```cpp

#include <iostream>
using namespace std;

int main() {
    
    int val1 = 10; //declaration

    int val2 = 20; // declaration

    int sum = val1 + val2; 

    cout<<sum; 

    return 0;
}
```
**⚙️ Output :**
>30


**💻 program to illustrate used of \n (new line):**
```c

#include <iostream>

int main() {
    
    std::cout << "Hello World";
    
    std::cout << "\n Hello ABC!";

    return 0;
}
```
**⚙️ Output :**
>Hello World<br>
Hello ABC!

## Rules to declared Variable

1. Variable name should be  meaningful
2. Variable name may contain (a-z,A-Z,0-9,_)
3. Variable name cannot start with number
4. It should not be reserved keyword
5. There should not be any special charecter

## 🔗 Some Useful Links

## 📖 References
