# Functions in C Programming 

## Functions

**A function is a block of code that performs a specific task.**<br>

__Types of function__<br>
_There are two types of function in C programming:_ <br>
* Standard library *(inbuilt)* functions
* User-defined functions

User-defined functions

**Syntax 1 :**
```c
returntype functionname()
{
    //implementation of function

    return value;
}
```

**💻Example 1 :**

```c
#include <stdio.h>

void hello()
{
    printf("\n Hello Everyone");
}
int main() {
    
    hello();
    
    return 0;
}
```
**⚙️ Output :** 
>Hello Everyone

**Syntax 2 :**
```c
#include <stdio.h>
//declaration  
void hello();

int main() {
    //calling
    hello();

    return 0;
}
//defination
void hello()
{
    printf("\n Hello Everyone");
}
```

**Syntax 3 :**
```c
#include <stdio.h>
//declaration with defination
void hello()
{
    printf("\n Hello Everyone");
}
int main() {
    //calling
    hello();

    return 0;
}
```

### WAP to calculate square of a number using function<br>
**💻Example 2 :**
```c
#include <stdio.h>

void cal_square(int n)
{
    int sq = n * n ;
    printf("\nSquare is %d",sq);
}
int main() {
    cal_square(2);
    return 0;
}
```
**⚙️ Output :** 
>Square is 4

**💻Example 3 :**
```c
#include <stdio.h>

void cal_square(int n)
{
    int sq = n * n ;
    printf("\nSquare is %d",sq);
}
int main() {
    cal_square(8);
    
    cal_square(7);
    return 0;
}
```
**⚙️ Output :** 
>Square is 64<br>
Square is 49

<br>

### WAP to calculate area of rectangle using function.<br>
**💻Example 4 :**
```c
#include <stdio.h>

void cal_area(int l, int b)
{
    int area = l * b;
    printf("\nArea of Rectangle is: %d",area);
}
int main() {
    
    cal_area(5, 2);
    
    return 0;
}
```
**⚙️ Output :** 
>Area of Rectangle is: 10

**💻Example 5 :**
```c
#include <stdio.h>

void cal_area(int l, int b)
{
    int area = l * b;
    printf("\nArea of Rectangle is: %d",area);
}
int main() {
    
    cal_area(5, 2);
    
    cal_area(10, 3);
    
    return 0;
}

```
**⚙️ Output :** 
>Area of Rectangle is: 10<br>
Area of Rectangle is: 30


**💻Example 6 :**
```c
#include <stdio.h>

int cal_area(int l, int b)
{
    int area = l * b;
    
    return area;
}
int main() {
    
    int res = cal_area(5, 2);

    printf("Result = %d", res);

    return 0;
}

```
**⚙️ Output :** 
>Result = 10

# Types of Functions Based on Arguments and Returntype in C Programming 

## Function argument and return values

**There are following categories:**<br>
* Function with arguments and return value.
* Function with arguments but no return value.
* Function with no arguments but returns a value.
* Function with no argument and no return value. <br>

_Function with arguments and return value_

**💻Example 1 :**
#### WAP to calculate area of rectangle
```c
#include <stdio.h>

int cal_area(int l, int b)
{
    int area = l * b;
    
    return area;
}
int main() {
    
    int l, b, area;
    
    printf("Enter length & breadth: ");
    scanf("%d%d",&l, &b);
    
    area = cal_area(l, b);
    
    printf("Area: %d",area);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter length & breadth: 10 5<br>
Area: 50

<br>  

_Function with arguments but no return value._

**💻Example 2 :**
```c
#include <stdio.h>

void cal_area(int l, int b)
{
    int area = l * b;
    
    printf("Area: %d",area);
    
}
int main() {
    
    int l, b;
    
    printf("Enter length & breadth: ");
    scanf("%d%d",&l, &b);
    
    cal_area(l, b);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter length & breadth: 10 5<br>
Area: 50

<br>

_Function with no arguments but returns a value._

**💻Example 3 :**
```c
#include <stdio.h>

int cal_area()
{
    int l, b;
    
    printf("Enter length & breadth: ");
    scanf("%d%d",&l, &b);
    
    int area = l * b;
    
    return area;
}

int main() {
    
    int area = cal_area();
    
    printf("Area: %d", area);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter length & breadth: 10 5<br>
Area: 50

<br>

_Function with no argument and no return value._

**💻Example 4 :**
```c
#include <stdio.h>

void cal_area()
{
    int l, b;
    
    printf("Enter length & breadth: ");
    scanf("%d%d",&l, &b);
    
    int area = l * b;
    
    printf("Area: %d", area);
}

int main() {
    
    cal_area();
    
    return 0;
}
```
**⚙️ Output :** 
>Enter length & breadth: 10 5<br>
Area: 50

**🏠Homework**
>WAP to calculate simple interest using all 4 types of functions.
