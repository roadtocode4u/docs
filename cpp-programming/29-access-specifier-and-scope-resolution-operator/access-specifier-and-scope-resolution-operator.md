## Access Specifier and Scope Resolution Operator

### Access Specifiers : 

The access modifiers of C++ allows us to determine which class members are accessible to other classes and functions, and which are not.

```cpp

public:
--------
--------
private:
--------
--------
public:

```

*💻Example 1:*

```cpp
#include <iostream>
using namespace std;

class Student
{
  public:
  string name;
  int age;
  
  void show()
  {
      cout<<"Name: "<<this->name<<endl;
      cout<<"Age: "<<this->age;
  }
};
int main() {
    Student s;
    
    s.name = "ABC";
    s.age = 12;
    
    s.show();
    return 0;
}
```

*⚙️ Output :*
>Name: ABC<br>
Age: 12

*💻Example 2:*
```cpp
#include <iostream>
using namespace std;

class Student
{
  public:
  string name;
  int age;
  
  void show()
  {
      cout<<"Name: "<<this->name<<endl;
      cout<<"Age: "<<this->age;
  }
};
int main() {
    Student s;
    
    s.age = 12;
    
    s.show();
    return 0;
}
```

*⚙️ Output :*

>Name: <br>
Age: 12

**This**

It is a special keyword which stores address of instance current class.

*💻Example 3:*

```cpp
#include <iostream>
using namespace std;

class Student
{
  public:
  string name;
  int age;
  int fees;
  
  void show()
  {
      cout<<"Name: "<<this->name<<endl;
      cout<<"Age: "<<this->age<<endl;
      cout<<"Fees: "<<this->fees;
  }
};
int main() {
    Student s;
    
    s.name = "ABC";
    s.age = 12;
    s.fees = 1000;
    
    s.show();
    return 0;
}
```

*⚙️ Output :*
>Name: ABC<br>
Age: 12<br>
Fees: 1000<br>


*💻Example 4:*
```cpp
#include <iostream>
using namespace std;

class Student
{
  private:
    string name;
    int age;
    int fees;
    
  public: 
  void getData()
  {
      cout<<"Enter name &  age: ";
      cin>>this->name>>this->age;
  }
  void show()
  {
      cout<<"Name: "<<this->name<<endl;
      cout<<"Age: "<<this->age<<endl;
      cout<<"Fees: "<<this->fees;
  }
};
int main() {
    Student s;
    
    s.getData();
    
    s.show();
    return 0;
}
```

*⚙️ Output :*

>Enter name &  age: Suraj 22<br>
Name: Suraj<br>
Age: 22<br>
Fees: 0<br>


*💻Example 5:*
```cpp
#include <iostream>
using namespace std;

class Student
{
  private:
    string name;
    int age;
    int fees;
    
  public: 
  void getData()
  {
      cout<<"Enter name &  age: ";
      cin>>this->name>>this->age;
  }
  void show()
  {
      cout<<"Name: "<<this->name<<endl;
      cout<<"Age: "<<this->age<<endl;
      cout<<"Fees: "<<this->fees;
  }
  void payFees()
  {
      cout<<"How much fees you want to pay: ";
      cin>>this->fees;
  }
};
int main() {
    Student s;
    
    s.getData();
    s.payFees();
    s.show();
    return 0;
}
```

*⚙️ Output :*

>Enter name &  age: Suraj 22<br>
How much fees you want to pay: 500<br>
Name: Suraj<br>
Age: 22<br>
Fees: 500<br>

*💻Example 6:*
```cpp
#include <iostream>
using namespace std;

class Student
{
  private:
    string name;
    int fees;
    
  public: 
  void getData()
  {
      cout<<"Enter name: ";
      cin>>this->name;
  }
  void show()
  {
      cout<<"Name: "<<this->name<<endl;
      cout<<"Fees: "<<this->fees<<endl;
  }
  void payFees()
  {
      cout<<"How much fees you want to pay: ";
      cin>>this->fees;
  }
};
int main() {
    Student s;
    
    s.getData();
    s.payFees();
    s.show();
    return 0;
}
```

*⚙️ Output :*

>Enter name: Suraj<br>
How much fees you want to pay: 21<br>
Name: Suraj<br>
Fees: 21<br>

**How to define class**
```cpp
variables

method1
method2
method3
method4
```
Student
```cpp
string name;
int fees;

void getData();
void showData();
void payFees();
```

Scope Resolution Operator ::

It is used to show origin.

```cpp
class p
{
    public:
    void sayHello();
};
```

```cpp
void p::sayHello()
{
    ------------
    ------------
    ------------
    ------------
}
```

*💻Example 7:*
```cpp
#include <iostream>
using namespace std;

class Student
{
    public:
    void sayHello(){
        cout<<"Hello Everyone";
    }
};
int main() {
    Student s;
    
    s.sayHello();
    
    return 0;
}
```

*⚙️ Output :*

>Hello Everyone

*💻Example 8:*
```cpp
#include <iostream>
using namespace std;

class Student
{
    public:
    
    void sayHello();
};

void Student::sayHello(){
    cout<<"Hello Everyone";
}
int main() {
    Student s;
    
    s.sayHello();
    
    return 0;
}
```

*⚙️ Output :*

>Hello Everyone


## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References