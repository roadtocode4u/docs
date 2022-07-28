# Call by Value and Call By Address 

## Call by Value and Call By Address

**💻Example 2 :**

```c
#include <stdio.h>
void fun(int x)
{
    x = (x * 2);
    printf("\n From Inside function: %d",x);
}
int main() {
    int x = 10;
    
    printf("\n Before function: %d",x);
    fun(x);
    printf("\n After function: %d",x);
    
    return 0;
}
```
**⚙️ Output :** 
>Before function: 10<br>
 From Inside function: 20<br>
 After function: 10<br>


**💻Example 3 :**
```c
#include <stdio.h>
int fun(int x)
{
    x = (x * 2);
    printf("\n From Inside function: %d",x);
    return x;
}
int main() {
    int x = 10;
    
    printf("\n Before function: %d",x);
    x = fun(x);
    printf("\n After function: %d",x);
    
    return 0;
}
```
**⚙️ Output :** 
>Before function: 10<br>
From Inside function: 20<br>
 After function: 20<br>
<br>

**💻Example 4 :**
```c
#include <stdio.h>
int fun(int x, int y)
{
    x = (x * 2);
    y = (y * 2);
    printf("\n From Inside function: %d",x);
    return x;
}
int main() {
    int x = 10;
    int y = 10;
    
    printf("\n Before function: %d",x);
    x = fun(x, y);
    printf("\n After function: %d",x);
    
    return 0;
}
```
**⚙️ Output :** 
>Before function: 10<br>
 From Inside function: 20<br>
 After function: 20<br>

<br>

**💻Example 5 :**
```c
#include <stdio.h>
void fun(int *x)
{
    *x = ((*x) * 2);
   
    printf("\n From Inside function: %d",*x);
}
int main() {
    int x = 10;
    
    printf("\n Before function: %d",x);
    fun(&x);
    printf("\n After function: %d",x);
    
    return 0;
}
```
**⚙️ Output :** 
>Before function: 10<br>
 From Inside function: 20<br>
 After function: 20<br>

