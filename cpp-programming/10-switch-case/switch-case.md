
# Switch Case

 ## Homeworks Examples :

**💻 Example 1️⃣ :  WAP to calculate largrst number among 3 using if-else-ladder ?**
```cpp
#include <iostream>
using namespace std;

int main() {

    int a,b,c;
    cout<<"Enter 3 Numbers:";
    cin>>a>>b>>c;

    if(a>b && a>c)
    {
        cout<<"A is largest";
    } 
    else if(b>a && b>c)
    {
        cout<<"B is largest";
    }
    else if(c>a && c>b)
    {
        cout<<"C is largest";
    } 
    else
    {
        cout<<"All are equal";
    }  
     return 0;
}
```
**⚙️ Output :**
>Enter 3 Numbers 5 80 7<br>
B is largest

**💻 Example 2️⃣: WAP to calculate largest number among 3 using nested-if ?**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    int a,b,c;
    cout<<"Enter 3 Numbers:";
    cin>>a>>b>>c;

    if(a>b)
    {
         if(a>c)
         {
             cout<<"A is largest";
         }
         else
         {
             cout<<"C is largest";
         }
    }
    else
    {
        if(b>c)
        {
            cout<<"B is largest";
        }
        else
        {
            cout<<"C is largest";
        }
    }
     return 0;
}
```
**⚙️ Output :**
>Enter 3 Numbers 2 70 6<br>
B is largest

## 💕Switch case  : 
```cpp
1 ----> "One"

2 ----> "Two"

3 ----> "Three"

syntax of switch case : 
switch(value)
{
    case 1 : 
    // case 1 operations
    break;

    case 2 : 
    // case 2 operations
    break;

    case 3 : 
    // case 3 operations
    break;
}
```
**💻 Example 1️⃣ :**
```cpp
#include <iostream>
using namespace std;

int main() {

    int value;
    cout<<"Enter Value:";
    cin>>value;

    switch(value)
    {
        case 1 : 
        cout<<"One";
        break;

        case 2 : 
        cout<<"Two";
        break;

        case 3 : 
        cout<<"Three";
        break;
    }
   
     return 0;
}
```
**⚙️ Output :**
>Enter Value: 1<br>
One

**💻 Example 2️⃣ :**
```cpp
#include <iostream>
using namespace std;

int main() {

    int value;
    cout<<"Enter Value:";
    cin>>value;

    switch(value)
    {
        case 1 : 
        cout<<"One";
        break;

        case 2 : 
        cout<<"Two";
        break;

        case 3 : 
        cout<<"Three";
        break;
    }
   
     return 0;
}
```
**⚙️ Output :**
>Enter Value: 3<br>
Three

**💻 Example 3️⃣ :**
```cpp
#include <iostream>
using namespace std;

int main() {

    int value;
    cout<<"Enter Value:";
    cin>>value;

    switch(value)
    {
        case 1 : 
        cout<<"One";
        break;

        case 2 : 
        cout<<"Two";
        break;

        case 3 : 
        cout<<"Three";
        break;

        default:
        cout<<"Not Matched";
    }
   
     return 0;
}
```
**⚙️ Output :**
>Enter Value: 5<br>
Not Matched

**💻 Example 4️⃣ :**
```cpp
#include <iostream>
using namespace std;

int main() {

    int a,b;
    cout<<"Enter Two Values:";
    cin>>a>>b;

    char op;

    cout<<"Which operations do you want to perform:(+, -, /, *): ";
    cin>>op;

    switch(op)
    {
        case "-";
        cout<<"a-b = "<<(a-b);
        break;

        case "+";
        cout<<"a+b = "<<(a+b);
        break;

        case "*";
        cout<<"a*b = "<<(a*b);
        break;

        case "/";
        cout<<"a/b = "<<(a/b);
        break;

        default : 
        cout<<"Operation is not valid";
    }  
     return 0;
}
```
**⚙️ Output :**
>Enter Two Values: 6,5<br>
Which operations do you want to perform :(+, -, /, *): - <br>
a-b = 1


**💻 Example 5️⃣ :**
```cpp
#include <iostream>
using namespace std;

int main() {

    int a,b;
    cout<<"Enter Two Values:";
    cin>>a>>b;

    char op;

    cout<<"Which operations do you want to perform:(+, -, /, *): ";
    cin>>op;

    switch(op)
    {
        case "-";
        cout<<"a-b = "<<(a-b);
        break;

        case "+";
        cout<<"a+b = "<<(a+b);
        break;

        case "*";
        cout<<"a*b = "<<(a*b);
        break;

        case "/";
        cout<<"a/b = "<<(a/b);
        break;

        default : 
        cout<<"Operation is not valid";
    }  
     return 0;
}
```
**⚙️ Output :**
>Enter Two Values: 9 9<br>
Which operations do you want to perform :(+, -, /, *): #  <br>
Operation is not valid


## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References



