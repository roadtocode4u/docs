##  Introduction to Inheritance

### Inheritance : 

Inheritance is a process in which one object acquires all the properties and behaviors of its parent object automatically. 

```cpp

A --> data members A          //Parent
|     member function A       //Base
|                             //Super
|
|
B --> data members A          //Child
      member functions A      //Derived
                              //Sub
      data members B 
      member functions B
```
Inheritance -> Is a relationship

```cpp    
      super class
           |
        Animal-eat()
           |  -sleep()
           |
     --------------
     |            |
    Dog          Cow
```

```cpp
[A]--> show A()
[B]--> show B()
```
*💻Example 1:*

```cpp
#include <iostream>
using namespace std;

class A
{
    public:
    void showA()
    {
        cout<<"I am showA()"<<endl;
    }
};

class B
{
    public:
    void showB()
    {
        cout<<"I am showB()"<<endl;
    }
};
int main() {
    A objA;
    objA.showA();
    
    B objB;
    objB.showB();
    return 0;
}
```

*⚙️ Output :*
>I am showA()<br>
I am showB()

```cpp
[A]-->showA()
 |
 |
 |
[B]-->showB()<=
      showA()<=
```

```cpp
class B:public A    //public->access
{                   //A->class

}
```
*💻Example 2:*
```cpp
#include <iostream>
using namespace std;

class A
{
    public:
    void showA()
    {
        cout<<"I am showA()"<<endl;
    }
};

class B : public A
{
    public:
    void showB()
    {
        cout<<"I am showB()"<<endl;
    }
};
int main() {
    B objB;
    objB.showA();
    return 0;
}
```

*⚙️ Output :*

>I am showA()

*💻Example 3:*

```cpp
#include <iostream>
using namespace std;

class A
{
    public:
    void showA()
    {
        cout<<"I am showA()"<<endl;
    }
};

class B : public A
{
    public:
    void showB()
    {
        cout<<"I am showB()"<<endl;
    }
};
int main() {
    B objB;
    objB.showA();
    objB.showB();
    return 0;
}
```

*⚙️ Output :*
>I am showA()<br>
I am showB()

```cpp

Single Level Inheritance

[A]----
 |    |
 |    | 1 Level 
 |    |
[B]----
```
```cpp
Multilevel Inheritance

[A]----
 |    |
 |    | 1 Level 
 |    |
[B]----
 |    |
 |    | 2 Level 
 |    |
[B]----
```
```cpp
Multiple Inheritance

[A]       [B]    [C]
 |         |      |
 |         |      |
 |___[Z]___|______|
```

```cpp
Hierarchical Inheritance

    --<----[RBI]---->--
    |        |        |
    |        |        |
  [BOI]    [SBI]    [HDFC]
```

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References