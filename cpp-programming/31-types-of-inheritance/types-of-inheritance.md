## Types of Inheritance

1. Single level inheritance
2. Multilevel inheritance
3. multiple inheritance
4. Hierachical inheritance
5. Hybrid inheritance


### 1) Single level inheritance :
```cpp
[A]
 |
 |  I Level
 |
[B]

Account
|___Salary
|___showSalary()

Emp
|_name
|_id   showEmp()
```
*💻Example 1:*

```cpp
#include <iostream>
using namespace std;

class Account
{
    public:
    int salary;
    void showSalary() 
    {
        cout<<"Salary is: "<<this->salary<<endl;
    }
};
class Emp
{
    public:
    int id;
    void showEmp()
    {
        cout<<"Emp ID: "<<this->id<<endl;
    }
};
int main() {
    Account objA;
    objA.salary = 1000;   
    objA.showSalary();

    Emp objE;
    objE.id = 123;
    objE.showEmp();

    return 0;
}
```

*⚙️ Output :*
>salary is: 1000<br>
Emp ID: 123

*💻Example 2:*

```cpp
#include <iostream>
using namespace std;

class Account
{
    public:
    int salary;
    void showSalary() 
    {
        cout<<"Salary is: "<<this->salary<<endl;
    }
};
class Emp : public Account
{
    public:
    int id;
    void showEmp()
    {
        cout<<"Emp ID: "<<this->id<<endl;
    }
};
int main() {
    Emp obj;
    obj.id = 123;
    obj.salary = 5000;
    obj.showEmp();
    obj.showSalary();

    return 0;
}
```

*⚙️ Output :*
>Emp ID: 123<br>
salary is: 5000

### 2) Multilevel Inheritance: 
```cpp
   [A] showA()
    |
    |
   [B] showB(), showA()
    |
    |
   [C] showC(), showB(), showA()
```
*💻Example 3:*

```cpp
#include <iostream>
using namespace std;

class A
{
    public:
    void showA()
    {
        cout<<"I am A"<<endl;
    }
    
};
class B : public A
{
    public:
    void showB()
    {
        cout<<"I am B"<<endl;
    }   
};
class C : public B
{
    public:
    void showC()
    {
        cout<<"I am C"<<endl;
    }  
};
int main()
{ 
    C obj:
    obj.showA();
    obj.showB();
    obj.showC();
    return 0;
}
```

*⚙️ Output :*
>I am A<br>
I am B<br>
I am C

### 3) Multiple Inheritance
```cpp

  [A]        [B]
   |          |
   | ________ |
        [C]

   [Mother]    [Father]
      |            |
      |            |
      |____________|
         [Child]
```

*💻Example 4:*

```cpp
#include <iostream>
using namespace std;

class Mother
{
    public:
    void showMother()
    {
        cout<<"Mother: Shantabai"<<endl;
    }   
};
class Father
{
    public:
    void showFather()
    {
        cout<<"Father: Rambhau"<<endl;
    }   
};
class Child: public Mother, public Father
{
    public:
    void showChild()
    {
        cout<<"I am Child"<<endl;
    }  
};
int main()
{ 
    Child c:
    c.showChild();
    c.showFather();
    c.showMother();
    return 0;
}
```

*⚙️ Output :*
>I am child<br>
Father: Rambhau<br>
Mother: Shantabai

### 4) Hierachical  Inheritance
```cpp
      _________[RBI]__________
     |           |            |
     |           |            |  
   [BOI]       [SBI]       [HDFC]
```
*💻Example 5:*

```cpp
#include <iostream>
using namespace std;

class RBI
{
    public:
    void showROI()
    {
        cout<<"According to RBI guidelines ROI is 10%"<<endl;
    }   
};
class BOI : public RBI
{
    public:
    void showBank()
    {
        cout<<"i am BOI"<<endl;
    }   
};
class SBI : public RBI
{
    public:
    void showBank()
    {
        cout<<"I am SBI"<<endl;
    }  
};
int main()
{ 
    SBI sbi;
    sbi.showROI();

    BOI boi;
    boi.showROI();
    return 0;
}
```

*⚙️ Output :*
>According to RBI guidelines ROI is 10%<br>
According to RBI guidelines ROI is 10%

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References
