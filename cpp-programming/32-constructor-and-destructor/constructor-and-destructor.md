# Constructor & Destructor

```cpp
1. Constructor() :

i)  It is special function.
ii) It invokes automatically, when object is created.
iii) It does not return value.
iv) Constructor name & classname must be same.
v) It is used to initialize data members.

                     id
                     name
                     show()
                      |
                      |
                      obj  
Syntax : 
class Emp <-- constructor name
{
    public:
    Emp() <-- class name
    {
        //-----
    }
}      
```

**💻Example 1️:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    int roll;
    string name;
    void showStudent()
    {
        cout<<"Name: "<<this->name<<endl;
        cout<<"Roll: "<<this->roll<<endl;
        
    }
};
int main() {
    Student obj;
    obj.showStudent();

    return 0;
}
```
**⚙️ Output :**
>Name:<br>
Roll: 2

**💻Example 2:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    int roll;
    string name;
    Student()
    {
        this->roll = 0;
        this->name = "Emplty Student";
    }
    void showStudent()
    {
        cout<<"Name: "<<this->name<<endl;
        cout<<"Roll: "<<this->roll<<endl;
    }
};
int main() {
    Student s1, s2;
    s1.name = "Anand";
    s1.roll = 123;
    s1.showStudent();
    s2.name = "Suraj";
    s2.roll = 456;
    s2.showStudent();

    return 0;
}
```
**⚙️ Output :**
>Name: Anand<br>
Roll: 123 <br>
Name: Suraj<br>
Roll: 456

**💻Example  3:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    Student()
    {
        cout<<"Constructor called...";
    }
};
int main() {
    Student obj;

    return 0;
}
```
**⚙️ Output :**
>Constructor called..

**💻Example 4:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    Student()
    {
        cout<<"Constructor called..."<<endl;
    }
};
int main() {
    Student s1,s2;

    return 0;
}
```
**⚙️ Output :**
>Constructor called...<br>
Constructor called...

**💻Example 5:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    Student()
    {
        cout<<"Constructor called..."<<endl;
    }
    void show()
    {
        cout<<"Show is called...";
    }
};
int main() {
    Student s1;
    s1.show();

    return 0;
}
```
**⚙️ Output :**
>Constructor called...<br>
Show is called...

## Parameterized constructor :
```cpp
Parameterized constructor :
Arguments can be passed to constructors. When an object is created, these arguments help initialize an object. 

Student(int roll, string name)
{
    this->roll = roll;
    this->name = name;
}

Student obj(p1, p2, p3);
```

**💻Example 6:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    Student(int num)
    {
        cout<<"I got"<<num<<endl;
    }
};
int main() {
    Student s1(1);
    Student s2(10);
    Student s3(100); 

    return 0;
}
```
**⚙️ Output :**
>I got 1<br>
I got 10<br>
i got 100

**💻Example 7:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    int roll;
    string name;
    Student(int roll, string name)
    {
        this->roll = roll;
        this->name = name;
    }
    void showStudent()
    {
        cout<<"Name: "<<this->name<<endl;
        cout<<"Roll: "<<this->roll<<endl;
    }
};
int main() {
    Student s1(1, "Anand");
    Student s2(2,
    "Prajakta");

    s1.showStudent();
    s2.showStudent();

    return 0;
}
```
**⚙️ Output :**
>Name: Anand<br>
Roll: 1 <br>
Name: Prajakta<br>
Roll: 2

## Destructor :
```cpp
2. Destructor() : it calls when object goes out of scope.

destructor ---> destroy

~className()
{
    //---
}

execution : 
1. constructor

2. member function

3. destructor
```

**💻Example 8:**
```cpp
#include <iostream>
using namespace std;
class Student
{
    public:
    int roll;
    string name;
    Student(int roll, string name)
    {
        this->roll = roll;
        this->name = name;
        cout<<"Constructor is called..."<<endl;
    }
    void showStudent()
    {
        cout<<"Name: "<<this->name<<endl;
        cout<<"Roll: "<<this->roll<<endl;
    }
    ~Student()
    {
        cout<<"Object is going to be killed";
    }
};
int main() {
    Student s1(1, "Anand");
    s1.showStudent();

    return 0;
}
```
**⚙️ Output :**
>Name: Anand<br>
Roll: 1 <br>
Object is going to be killed


## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References
