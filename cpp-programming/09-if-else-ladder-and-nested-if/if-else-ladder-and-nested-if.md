# if-else-ladder and nested-if

## Conditional Statements : 
There are Four Types : 
1. if 
2. if-else
3. if-else-ladder
4. nested-if

```cpp
3. if-else-ladder

syntax : 
if (condition 1)
{
    //-----
    //-----
}
else if(condition 2)
{
    //----
    //----
}
else if(condition 3)
{
    //----
    //----
}
else if(condition 4)
{
    //----
    //----
}
else
{
  //----
}
```

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;
    cout<<"Enter Number: ";
    cin>>num;

    if(num==1){
        cout<<"One";
    }
    else if(num==2){
        cout<<"Two"; 
    }
    else if(num==3){
        cout<<"Three"; 
    }
    else if(num==4){
        cout<<"Four"; 
    }
    else
    {
        cout<<"Not Matched :";
    }  
     return 0;
}
```
**⚙️ Output :**
>Enter Number : 3<br>
Three

**💻 Example 2 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int num;
    cout<<"Enter Number: ";
    cin>>num;

    if(num==1){
        cout<<"One";
    }
    else if(num==2){
        cout<<"Two"; 
    }
    else if(num==3){
        cout<<"Three"; 
    }
    else if(num==4){
        cout<<"Four"; 
    }
    else
    {
        cout<<"Not Matched...";
    } 
     return 0; 
}
```
**⚙️ Output :**
>Enter Number : 8<br>
Not Matched...

**💻 Example 3 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int marks;

    cout<<"Enter Marks:";
    cin>>marks;

    if(marks>90){
        cout<<" Grade A";
    }
    else if(marks>80){
        cout<<"Grade B"; 
    }
    else if(marks>70){
        cout<<" Grade C"; 
    }
    else
    {
        cout<<"Fail";
    }  
     return 0;
}
```
**⚙️ Output :**
>Enter Marks : 85<br>
Grade B

**💻 Example 4 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int marks;

    cout<<"Enter Marks:";
    cin>>marks;

    if(marks>90){
        cout<<" Grade A";
    }
    else if(marks>80){
        cout<<"Grade B"; 
    }
    else if(marks>70){
        cout<<"Grade C"; 
    }
    else if(marks>60){
        cout<<"Grade D"; 
    }
    else
    {
        cout<<"Fail";
    }  
     return 0;
}
```
**⚙️ Output :**
>Enter Marks : 25<br>
Fail

**💻 Example 5 : Boundry Condition**
```cpp
#include <iostream>
using namespace std;

int main() {
    int marks;

    cout<<"Enter Marks:";
    cin>>marks;

    if(marks>=70 && marks<=80>){
        cout<<"Grade C";
    }
    else if(marks>=80 && marks<=90){
        cout<<"Grade B"; 
    }
    else if(marks>=90 && marks <=100){
        cout<<"Grade A"; 
    }
    else
    {
        cout<<"Invalid Number";
    }  

    return 0;
}
```
**⚙️ Output :**
>Enter Marks : 100<br>
A

**💻 Example 6 : Boundry Condition**
```cpp
#include <iostream>
using namespace std;

int main() {
    int marks;

    cout<<"Enter Marks:";
    cin>>marks;

    if(marks>=70 && marks<=80>){
        cout<<"Grade C";
    }
    else if(marks>=80 && marks<=90){
        cout<<"Grade B"; 
    }
    else if(marks>=90 && marks <=100){
        cout<<"Grade A"; 
    }
    else
    {
        cout<<"Invalid Number";
    }  

    return 0;
}
```
**⚙️ Output :**
>Enter Marks : 880<br>
Invalid Number

```cpp
4. nested-if
syntax : 

if (condition)
{
    if
    {
        //-----
    }
    else
    {
        //----
    }
}
else
{
    //----
}
```

**💻 Example 1 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int maths=30;
    int marathi=36;

    if(marks>=35 && marathi>=35>){
        cout<<"Pass";
    }
    else
    {
        cout<<"Fail";
    }  

    return 0;
}
```
**⚙️ Output :**
>Fail

**💻 Example 2 :**
```cpp
#include <iostream>
using namespace std;

int main() {
    int maths=40;
    int marathi=16;

    if(marathi>=35>)
    {
        cout<<"Passed in Marathi";
        if(maths>=35)
        {
            cout<<Passed in Maths"<<endl;
        }
         else
        {
        cout<<"Failed in Maths";
        }  
    }
    else
    {
       cout<<"Failed in Marathi";
    }
    return 0;
}
```
**⚙️ Output :**
>Passed in Maths<br>
Failed in Marathi


## 🏠  HomeWork
1️⃣ WAP to calculate largrst number among 3 using if-else-ladder ?

2️⃣ WAP to calculate largest number among 3 using nested-if ?

## 🔗 Some Useful Links

## 📖 References



