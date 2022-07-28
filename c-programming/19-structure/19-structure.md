# Lecture-28 Structures in C Programming 

## Structures

What is structure?<br>
A structure is used to define a custom datatype.

**Syntax :**
```c
struct structName
{
   datatype var1;
   datatype var2;
   datatype var3;
};

```
*Defining a structure*
```c
struct student
{
  char name[100];
  int roll;
  int age;
};

```
<br>

*creating object / variable of structure*

**💻Example 1 :**
```c
#include <stdio.h>

struct student{
    int roll;
    int age;
};
int main(){
    
    struct student s1;
    s1.roll = 1;
    s1.age = 22;
    
    printf("Roll: %d", s1.roll);
    printf("Age: %d", s1.age);
    
    return 0;
};


```
**⚙️ Output :** 
>Roll: 1Age: 22

<br>

**💻Example 2 :**

```c
#include <stdio.h>

struct student{
    int roll;
    int age;
};
int main(){
    
    struct student s1, s2;
    s1.roll = 1;
    s1.age = 22;
    
    s2.roll = 2;
    s2.age = 21;
    
    printf("\nRoll: %d", s1.roll);
    printf("\nAge: %d", s1.age);
    
    printf("\nRoll: %d", s2.roll);
    printf("\nAge: %d", s2.age);
    
    return 0;
};

```
**⚙️ Output :** 
>Roll: 1<br>
Age: 22<br>
Roll: 2<br>
Age: 21<br>

<br>

**💻Example 3 :**

```c
#include <stdio.h>

struct rectangle{
  int length;
  int breadth;
};
int main(){
    struct rectangle r1;
    
    printf("Enter Length: ");
    scanf("%d", &r1.length);
    
    printf("Enter Breadth: ");
    scanf("%d", &r1.breadth);
    
    int area = r1.length * r1.breadth;
    
    printf("Area: %d", area);
    
    return 0;
};

```
**⚙️ Output :** 
>Enter Length: 5<br>
Enter Breadth: 6<br>
Area: 30<br>

<br>

**💻Example 4 :**

```c
#include <stdio.h>

struct rectangle{
  int length;
  int breadth;
  int area;
};
int main(){
    struct rectangle r1;
    
    printf("Enter Length: ");
    scanf("%d", &r1.length);
    
    printf("Enter Breadth: ");
    scanf("%d", &r1.breadth);
    
    r1.area = r1.length * r1.breadth;
    
    printf("Area: %d", r1.area);
    
    return 0;
};

```
**⚙️ Output :** 
>Enter Length: 4<br>
Enter Breadth: 7<br>
Area: 28<br>
