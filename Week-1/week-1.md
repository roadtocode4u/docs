# Introduction to C Programming

## 🤔What is Programming ?

Programming is the process of instructions that tell a computer how to perform a task.


## Different Programming Languages 💻
```c
C,C++,Java,Python,Kotlin,Javascript,Ruby,Typescript,C#, ...
```

## What is C Programmong?

C is a general-purpose programming language.C prograamming created by **Dennis Ritchie** at the **Bell Laboratories** in **1972**.

**💻 Example :**
```c
#include <stdio.h>

int main() 
{

    printf("Hello world");
    
    return 0;
}
```
**⚙️ Output :**
>Hello world

## Program Explanation:

**Line 1:** `#include <stdio.h>` is a header file. The header file `<stdio.h>` stands for **Standard Input Output**.
`#include <stdio.h>`support input output file like  printf() and scanf().**Printf( )** Means Print output on screen **scanf()** Give input from user.

**Line 2:** `int` means Return type of your Function. `main()` it is the first function of every C program that is responsible for starting the execution and termination of the program.

**Line 3:** `{` is used to Start of the function.

**Line 4:** `printf("Hello world");` `printf()` is a function used to output print text to the screen. In our example it will output "Hello World". **`;`** semicolon used to terminate any statement.

**Line 5:** `return 0;` return 0 means that the program will execute successfully.

**Line 6:** `}` closing curly bracket is used to end the main function.




**💻 Example :**
```c

#include <stdio.h>

int main()
{
  
    printf("Hye");
    printf("How Are You ?");
    
    return 0;
}
```
**⚙️ Output :**
>HyeHow Are You ?

## New Line Charachter

`\n` is used to New line Character.

**Example :**
```c
#include <stdio.h>

int main() {
  
    printf("Good Morning !\n");
    printf("Good afternoon !");
    
    return 0;
}

```

**⚙️ Output :**
>Good Morning !     
Good afternoon !


<br>

# Datatype, Variables and Format Specifiers


## String :

Strings is represented as Collection of characters.

## Variable :

Variable is used to store data.

## Datatype :

**1. Integers (int)**

 Intergers means Stores whole numbers without decimals point.

💻Example  = 1,2,2253,899,44,55...

**2. Character (char)**

Stores a single character,letter.

💻Example='r','v','s'....

**3. Float (float)**

float means Stores numbers with decimals point.

💻Example= 15.7,89.0,46.84 ....

## Format Specifiers:
 
 There are different format specifiers for each data type.

`%d`=int

`%f`=float

`%c`=char

**💻Example :**
```c
#include <stdio.h>

int main()
 {
  
   int age=10;
   
   printf("%d",age);
    
    return 0;
}
```
**⚙️ Output :**
>10 

**💻Example :**
```c
#include <stdio.h>

int main()
{
    
   int age;
   age=30;
   
   printf("%d",age);
    
    return 0;
}
```
**⚙️ Output :**
>30 

**💻Example :**
```c
#include <stdio.h>

int main()
{
    
   int age;
   age=30;
   age=50;
   
   printf("%d",age);
    
    return 0;
}
```
**⚙️ Output :**
>50 

**💻Example :**
```c
#include <stdio.h>

int main()
{
    
   int age;
   age=30;
   printf("%d",age);
   
   age=50;
   printf("%d",age);
    
    return 0;
}
```
**⚙️ Output :**
>3050 

**💻Example :**
```c
#include <stdio.h>

int main()
{
    float weight=80.5;
    
    printf("%f",weight);
    
    return 0;
}
```
**⚙️ Output :**
>80.500000

**💻Example :**
```c
#include <stdio.h>

int main()
{
    char alpha='c';
    
    printf("%c",alpha);
    
    return 0;
}
```
**⚙️ Output :**
>c

<br>

# Rules to Declare Variables and Formatting Output

## Rules of Declare Variables

1. A Variable Name Can contain alphabates (A to Z)(a to z) , digits (0-9),underscore( _ ).

2. Cannot Start with digit.

3. Cannot use reserved keyword or special character.

4. Length of variable name should be less than 31 character.

## Case Sensitivity 

Text that is sensitive to capitalization of letters. For example, `NAME` ,`name`,`NaMe` are three different.

**Example :** 

*Write a program to sum of 2 variable*

```c
#include <stdio.h>

int main() {
    int a=10;
    int b=20;
    int c;
    
    c=a+b;
    
    printf("%d",c);
    
    return 0;
}
```

**⚙️ Output :**
>30

**💻Example :**
```c
#include <stdio.h>

int main() {
    int val1=30;
    int val2=20;
    int sum;
    
    sum=val1 + val2;
    
    printf("%d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>50

**💻Example :**
```c
#include <stdio.h>

int main() {
    int val1=30, val2=20, sum;
    
    sum=val1 + val2;
    
    printf("%d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>50 

## Formatting Output

**💻Example :**
```c
#include <stdio.h>

int main() {
    int val1=30, val2=20, sum;
    
    sum=val1 + val2;
    
    printf(" sum = %d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>sum = 50 

**💻Example :**
```c
#include <stdio.h>

int main() {
    float num = 20.5;
    
    printf("Numberis %f", num);
    
    return 0;
}
```
**⚙️ Output :**
>Numberis 20.500000

**💻Example :**
```c
#include <stdio.h>

int main()
{
    float weight=80.5;
    
    printf("%f",weight);
    
    return 0;
}
```
**⚙️ Output :**
>80.500000

**💻Example :**
```c
#include <stdio.h>

int main() {
    int a = 10;
    int b = 20;
    int c = a + b;
    
    printf("a=%d b=%d",a,b);
    
    return 0;
}
```
**⚙️ Output :**
>a=10 b=20

**💻Example :**
```c
#include <stdio.h>

int main() {
    int val1 = 10;
    int val2 = 20;
    int sum = val1 + val2;
    
    printf("sum of %d and %d is %d",val1,val2,sum);
    
    return 0;
}
```
**⚙️ Output :**
>sum of 10 and 20 is 30

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

By Defalut, the value is incremented by **1**.

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

By Defalut, the value is Decremented by **1**.

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

## scanf() function:

The scanf() function which is used for input, to  read the input data from the console.

 **💻Example :**
```c
#include <stdio.h>

int main() {
    
    int val;
    
    printf("Enter value of val:");
    scanf("%d",&val);
    
    printf("output is %d",val);
 
    return 0;
}
```
**⚙️ Output :**
>Enter value of val:10    
output is 10  

 **💻Example :**
```c
#include <stdio.h>

int main() {
    
     int num1;
     int num2;
     int sum;
     
     printf("Enter Value of num1 :");
     scanf("%d",&num1);
     
     printf("Enter Value of num2 :");
     scanf("%d",&num2);
     
     sum = num1 + num2;
     
     printf("sum:%d",sum);
 
    return 0;
}
```
**⚙️ Output :**
>Enter Value of num1 :10   
Enter Value of num2 :20    
sum:30   

<br>

# Practice Questions C Programming 


## 💻🏆Examples :

**💻Example:**
```c
// Sum of two numbers

#include <stdio.h>

int main() {
    int num1, num2;
    
    printf("Enter value of num1 :");
    scanf("%d",&num1);
    
    printf("Enter value of num1 :");
    scanf("%d",&num2);
    
    int sum = num1 + num2;
    printf("sum of num1 and num2 =%d",sum);
   
    return 0;
}
```
**⚙️ Output :**
>Enter value of num1 :10   
Enter value of num1 :20    
sum of num1 and num2 =30  

**💻Example:**
```c

#include <stdio.h>

int main() {
   int marathi,hindi,english;
   
   printf("Enter marks of Marathi :");
   scanf("%d", &marathi);
   
    printf("Enter marks of Hindi :");
   scanf("%d", &hindi);
   
    printf("Enter marks of English :");
   scanf("%d", &english);
   
   printf("M=%d H=%d E=%d",marathi,hindi,english);
    
    return 0;
}
```
**⚙️ Output :**
>Enter marks of Marathi :95    
Enter marks of Hindi :95   
Enter marks of English :95   
M=95 H=95 E=95


**💻Example:**
```c
#include <stdio.h>

int main() {
   int marathi,hindi,english;
   
   printf("Enter marks of Marathi ,Hindi,and English :");
   scanf("%d%d%d", &marathi,&hindi,&english);
  
   
   printf("M=%d H=%d E=%d",marathi,hindi,english);
    
    return 0;
}
```
**⚙️ Output :**
>Enter marks of Marathi ,Hindi,and English :95 95 95     
M=95 H=95 E=95

**💻Example:**
```c
//Take input from user and print sum and percentage 

#include <stdio.h>

int main() {
   int marathi,hindi,english;
   
   printf("Enter marks of Marathi ,Hindi,and English :");
   scanf("%d%d%d", &marathi,&hindi,&english);
  
   int sum = (marathi + hindi + english );
   
   int per =sum/3;
   char p ='%';
   
   printf("Sum=%d,Percentage=%d %c",sum,per,p);
   
    return 0;
}
```
**⚙️ Output :**
>Enter marks of Marathi ,Hindi,and English :95 95 95    
Sum=285,Percentage=95 %


**💻Example:**
```c
//C program to calculate Simple Interest
#include <stdio.h>

int main() {
    
    float p,r,t,si;
    
    printf("Enter Principle,Rate and Time:");
    scanf("%f%f%f", &p,&r,&t);
    
    si=(p*r*t)/100;
    
    printf("Simple Interest :%f",si);
    printf("\nPayble Amount:%f",p+si);
    
    return 0;
}
```
**⚙️ Output :**
>Enter Principle,Rate and Time:5000 300 2   
Simple Interest :30000.000000   
Payble Amount:35000.000000  

**💻Example:**
```c
//Program to convert temperature from celsius to fahrenheit 
#include <stdio.h>

int main() {
   
   float f,c;
   
   printf("Enter Temperature in Celsius :");
   scanf("%f",&c);
   
   f=1.8*c+32;
   
   printf(" Temperature in Fahreinheit =%f",f);
    
    return 0;
}
```
**⚙️ Output :**
>Enter Temperature in Celsius :36   
Temperature in Fahreinheit =96.800003


## 🏠Homework 

>1️⃣ Write a program to take input of 5 subject from user and print sum and percentage.

>2️⃣ Write a program to calculate bill when rate and quantity is give from user.

>3️⃣ Write a program to calculate perimeter and area of a circle when radius is given.

>4️⃣ Write a program to convert km to m and cm.

>5️⃣Write a program to calculate area and perimeter of rectangle when length and breadth is given.

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