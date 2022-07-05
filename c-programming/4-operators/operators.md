# Operators and Comments in C Programming 

## Operators 

Operators are used to perform operations on variables and values.

**Types of Operators =**
* Arithmetic operators (+,-,*,/,%)
* Increment Decrement Operators(++,--)
* Assignment operators (=,+=,-=,*=,/=,%=)
* Relational Operators (<,<=,>,>=,==,!=)
* Logical operators (&&,||,!)
* Bitwise operators (&,<<,>>,^,|,~)

**Arithmetic Operators**

* Addition (+)

Adds together two values.

**💻Example :**
```c
#include <stdio.h>

int main() {
    
    int val1=10;
    int val2=20;
    int sum=val1+val2;
    
    printf("%d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>30

* Substraction (-)

Subtracts one value from another.

**💻Example :**
```c
#include <stdio.h>

int main() {
    
    int val1=10;
    int val2=20;
    int sum=val1-val2;
    
    printf("%d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>-10

* Multiplication (*)

Multiplies two values.

**💻Example :**
```c
#include <stdio.h>

int main() {
    
    int val1=10;
    int val2=20;
    int sum=val1*val2;
    
    printf("%d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>200

* Division (/)

Divides one value by another.

**💻Example :**
```c
#include <stdio.h>

int main() {
    
    int val1=30;
    int val2=20;
    int sum=val1/val2;
    
    printf("%d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>1

* Modulus (%)

Returns the division remainder

**💻Example :**
```c
#include <stdio.h>

int main() {
    
    int result=11 % 4;
    
    printf("%d",result);
    
    return 0;
}
```
**⚙️ Output :**
>3

## Comments in C

Comments can be used to explain code, and to make it more readable. 

## Single-line Comments

Single-line comment are use to comment in single line.
Single-line comments start with two forward slashes (`//`).

**💻Example :**
```c
#include <stdio.h>

int main() {
    
    // This is a comment
      printf("Hye!");
    
    return 0;
}
```
**⚙️ Output :**
>Hye!

## Multi-line Comments

Multi-line comment are used comment in multiple Line.
Multi-line comments start with `/*` and ends with `*/`.

**💻Example :**
```c
#include <stdio.h>

int main() {
    
    /* This is a Multi-line comment
    and multi-line comment are use to comment on multiple line.*/

      printf("Hye!");
    
    return 0;
}
```
**⚙️ Output :**
>Hye!

<br>

# Increment, Decrement Operator and Scanf Functions in C Programming 

**💻Example :**
```c
#include <stdio.h>

int main() {
   
   int count=5;
   
   count=count + 1;
   
    printf("%d",count);
    
    return 0;
}
```
**⚙️ Output :**
>6

* value Increase 

**💻Example :**
```c
#include <stdio.h>

int main() {
   
   int count=5;
   //count => 5
   printf("\n%d",count);
   
   count=count + 1;
   //count => 6
   printf("\n%d",count);
    
    count=count + 1;
    //count => 7
    printf("\n%d",count);
    return 0;
}
```
**⚙️ Output :**
>5   
6   
7


* value Decrease

**💻Example :**
```c

#include <stdio.h>

int main() {
   
   int count=5;
   //count => 5
   printf("\n%d",count);
   
   count=count - 1;
   //count => 4
   printf("\n%d",count);
    
    count=count - 1;
    //count => 3
    printf("\n%d",count);
    return 0;
}
```
**⚙️ Output :**
>5     
4    
3  

## Increment Operator (++)

This Operator are used to increase the value of variable.

By Default, the value is incremented by **1**.

**💻Example :**
```c

#include <stdio.h>

int main() {
   
   int count=5;
   //count => 5
   printf("\n%d",count);
   
   count++;
   //count => 6
   printf("\n%d",count);
    
    count++;
    //count => 7
    printf("\n%d",count);
    return 0;
}
```
**⚙️ Output :**
>5  
6     
7

**💻Example :**
```c

#include <stdio.h>

int main() {
   
   int count=5;
   count =count+2;
    printf("\n%d",count);
    return 0;
}
```
**⚙️ Output :**
>7

## Type of Increment Operator

1. Pre-Increment (++var)
2. Post-Increment (var++)

**💻Example :**
```c
#include <stdio.h>

int main() {
   
   int val1 = 0;
   val1++; //Post Increment 
   printf("\n%d",val1);
   
   
   int val2 = 0;
   ++val2; //Pre Increment 
   printf("\n%d",val2);
   
    return 0;
}
```
**⚙️ Output :**
>1  
1

**💻Example :**
```c
#include <stdio.h>

int main() {
   
   int val1 = 0;
   
   int result = val1++;
   
   printf("\n%d",result);

   printf("\n%d",val1);
    return 0;
}
```
**⚙️ Output :**
>0    
1 

**💻Example :**
```c
#include <stdio.h>

int main() {
   
   int val1 = 0;
   
   int result = ++val1;
   
   printf("\n%d",result);
   
   printf("\n%d",val1);
    return 0;
}
```
**⚙️ Output :**
>1    
1

## Decrement Operator (--)

This Operator are used to decrease the value of variable.

By Default, the value is Decremented by **1**.

**💻Example :**
```c


#include <stdio.h>

int main() {
   
   int count=5;
   //count => 5
   printf("\n%d",count);
   
   count--;
   //count => 4
   printf("\n%d",count);
    
    count--;
    //count => 3
    printf("\n%d",count);
    return 0;
}
```
**⚙️ Output :**
>5   
4    
3


**💻Example :**
```c
#include <stdio.h>

int main() {
   
   int count=5;
   count--;
   count--;
   count--;
    printf("\n%d",count);
    return 0;
}
```
**⚙️ Output :**
>2

## Type of Decrement Operator

1. Pre-Decrement (--var)
2. Post-Decrement (var--)

**💻Example :**
```c

#include <stdio.h>

int main() {
   
   int val1 = 5;
   
   int result = val1--;
   
   printf("\n%d",result);
   
   printf("\n%d",val1);
    return 0;
}
```
**⚙️ Output :**
>5   
 4  

 **💻Example :**
```c
#include <stdio.h>

int main() {
   
   int val1 = 5;
   
   int result = --val1;
   
   printf("\n%d",result);
   
   printf("\n%d",val1);
    return 0;
}
```
**⚙️ Output :**
>4      
4  

<br>

# Assignment Operators, Comparison Operators and  Ternary Operator in C Programming 

## Assignment operators

Assignment operators applied to assign the result of an expression to a variable.

### Assign (=)

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int a = 10;
    
    printf("%d",a);
    
    return 0;
}
```
**⚙️ Output :**
>10

 ### Add then assign (+=)

**💻Example:**
```c

#include <stdio.h>

int main() {
    
    int a =5;
    
    a += 3; //a = a + 3;
    
    printf("%d",a);
    
    return 0;
}
```
**⚙️ Output :**
>8

 ### Substract then assign (-=)
 
**💻Example:**
```c

#include <stdio.h>

int main() {
    
    int a =5;
    
    a -= 3; //a = a - 3;
    
    printf("%d",a);
    
    return 0;
}
```
**⚙️ Output :**
>2

### Multiplies then assign (*=)
 
**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int a =5;
    
    a *= 3; //a = a * 3;
    
    printf("%d",a);
    
    return 0;
}
```
**⚙️ Output :**
>15

### Divides then assign(/=)
 
**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int a =10;
    
    a /= 2; //a = a / 2;
    
    printf("%d",a);
    
    return 0;
}
```
**⚙️ Output :**
>5

### Modulus then assign(%=)
 
**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int a =7;
    
    a %= 2; //a = a % 2;
    
    printf("%d",a);
    
    return 0;
}
```
**⚙️ Output :**
>1

## Comparison Operators 

### Equal to (==)

Equal to are used to compare to object. 

**💻Example:**
```c
// if value are not equal then print 0 means false.
#include <stdio.h>

int main() {
    
    int a = 5;
    int b = 10;
    
    int ans = (a==b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>0 

**💻Example:**
```c
// if value are equal then print 1 means true.
#include <stdio.h>

int main() {
    
    int a = 10;
    int b = 10;
    
    int ans = (a==b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>1 

### Greater than (>)

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int a = 5;
    int b = 10;
    
    int ans = (a>b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>0 

**💻Example:**
```c
//a is greater than b then true.
#include <stdio.h>

int main() {
    
    int a = 5;
    int b = 2;
    
    int ans = (a>b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>1

### Less than (<)

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int a = 20;
    int b = 10;
    
    int ans = (a<b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>0 

**💻Example:**
```c
// a is less than b then true .
#include <stdio.h>

int main() {
    
    int a = 10;
    int b = 20;
    
    int ans = (a,b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>1

### Less than or equal to (<=)

**💻Example:**
```c
// a is less than or equal to b then true otherwise false.
#include <stdio.h>

int main() {
    
    int a = 100;
    int b = 10;
    
    int ans = (a<=b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>0 

**💻Example:**
```c
// a is less than or equal to b then true.
#include <stdio.h>

int main() {
    
    int a = 10;
    int b = 10;
    
    int ans = (a<=b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>1

### greater  than or equal to (>=)

**💻Example:**
```c
// a is greater  than or equal to b then true otherwise false.
#include <stdio.h>

int main() {
    
    int a = 1;
    int b = 10;
    
    int ans = (a<=b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>0 

**💻Example:**
```c
// a is greater than or equal to b then true.
#include <stdio.h>

int main() {
    
    int a = 100;
    int b = 10;
    
    int ans = (a<=b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>1

###	not equal to (!=)

**💻Example:**
```c
//a is not equal to b then true otherwise false.
#include <stdio.h>

int main() {
    
    int a = 10;
    int b = 10;
    
    int ans = (a!=b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>0 

**💻Example:**
```c
//a is not equal to b then true.
#include <stdio.h>

int main() {
    
    int a = 20;
    int b = 10;
    
    int ans = (a!=b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>1

## Ternary Operator 

**Syntax :**
```c
(condition)?True:False
```

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int a = 100;
    int b = 10;
    
    int ans = (a>b?a:b);
    
    printf("%d",ans);
    
    return 0;
}
```
**⚙️ Output :**
>100

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int num;
    printf("Enter Number :");
    scanf("%d",&num);
    
    int ans = (num%2==0)?printf("Even"):printf("odd");
    
    return 0;
}
```
**⚙️ Output :**
>Even

## 🏠Homework 

>1️⃣ Write a program to take age from user and check if he / she eligible for voting.

<br>