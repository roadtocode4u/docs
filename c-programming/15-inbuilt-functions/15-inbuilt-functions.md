# Inbuilt Math and String Functions in C Programming 

## Inbuilt Functions

**<math.h>**<br>
_Predefined function of math.h header file._
* ceil()<br>
* floor()<br>
* sqrt()<br>
* pow()<br>
* abs()<br>

_ceil( ) function returns nearest integer value which is greater than or equal to the value of floating point._<br>

**💻Example 1 :**

```c
#include <math.h>
#include <stdio.h>

int main() {
    float num = 50.6;
    
    float ans = ceil(num);
    
    printf("%f",ans);
    return 0;
}
```
**⚙️ Output :** 
>51.000000

<br>

_floor() function used to return the closest integer value which is less than or equal to a given number._

**💻Example 2 :**
```c
#include <math.h>
#include <stdio.h>

int main() {
    float num = 50.6;
    
    float ans = floor(num);
    
    printf("%f",ans);
    return 0;
}
```
**⚙️ Output :** 
>50.000000

<br>

_sqrt() function used to calculate the square root of a given number._

**💻Example 3 :**
```c
#include <math.h>
#include <stdio.h>

int main() {
    int num;
    printf("Enter Number: ");
    scanf("%d", &num);
    
    int ans = sqrt(num);
    
    printf("Square Root: %d", ans);
    return 0;
}
```
**⚙️ Output :** 
>Enter Number: 81<br>
Square Root: 9

<br>

_pow() function is used to calculate the power of any given number._

**💻Example 4 :**
```c
#include <math.h>
#include <stdio.h>

int main() {
    
    int ans = pow(3, 3);
    
    printf("%d", ans);
    return 0;
}
```
**⚙️ Output :** 
>27

<br>

_abs( ) function returns the absolute value of an integer._<br>
_The absolute value of a number is always positive._<br>

**💻Example 5 :**
```c
#include <math.h>
#include <stdio.h>

int main() {
   
   int ans = abs(-20);
   
    printf("%d", ans);
    
    return 0;
}

```
**⚙️ Output :** 
>20

**💻Example 6 :**
```c
#include <math.h>
#include <stdio.h>

int main() {
   
   int ans = abs(20);
   
    printf("%d", ans);
    
    return 0;
}

```
**⚙️ Output :** 
>20

<br>

**<string.h>**
* strlen()
* strupr()
* strlwr()
* strcpy()
* strrev()
* strcat()

_strlen() function calculates the length of a given string_<br>

**💻Example 7 :**
```c
#include <string.h>
#include <stdio.h>

int main() {
   
   char str[] = "Hello World";
   
   int length = strlen(str);
   
    printf("%d", length);
    
    return 0;
}

```
**⚙️ Output :** 
>11

<br>

_strupr( ) function is used to converts a given string to uppercase._<br>

_strlwr( ) function is used to convert a given string into lowercase._<br>

_strcpy( ) function is used to copy one string to another._<br>

_strrev( ) function is used for reversing a string._<br><br>

_strcat( ) function is used to concatenates two strings and result is returned to first string._<br>

**💻Example 8 :**
```c
#include <string.h>
#include <stdio.h>

int main() {
   
   char str1[100] = "Road";
   char str2[50] = " To Code";
   
   strcat(str1, str2);
   
    printf("%s", str1);
    
    return 0;
}

```
**⚙️ Output :** 
>Road To Code
