# Pointers in C Programming 

## Pointers

**Pointers is a variable which stores the address of another variable.**<br>
### ampersand or address of operator is used to find address of a variable.
This address operator is denoted by “&”.

**💻Example 1 :**

```c
#include <stdio.h>

int main() {
    int age = 22;
    
    printf("%d", age);
    return 0;
}
```
**⚙️ Output :** 
>22

<br>

**💻Example 2 :**

```c
#include <stdio.h>

int main() {
    int age = 22;
    
    printf("%p", &age);
    return 0;
}
```
**⚙️ Output :** 
>0x7ffc1af67b64


**💻Example 3 :**
```c
#include <stdio.h>

int main() {
    int age = 22;
    
    printf("\nValue: %d", age);
    printf("\nAddress: %p", &age);
    
    return 0;
}
```
**⚙️ Output :** 
>Value: 22<br>
Address: 0x7ffc07a9acb4

<br>

**Syntax :**
```c
<datatype> *<variable name>;

int *age;

```

**💻Example 4 :**
```c
#include <stdio.h>

int main() {
    int age = 22;
    int *p = &age;
    
    printf("\n1-> %d",age);
    printf("\n2-> %p",&age);
    printf("\n3-> %p",p);
    printf("\n4-> %d",&p);
    
    return 0;
}
```
**⚙️ Output :** 
>1-> 22<br>
2-> 0x7ffd8d74869c<br>
3-> 0x7ffd8d74869c<br>
4-> -1921743200<br>

<br>

**💻Example 5 :**
```c
#include <stdio.h>

int main() {
    int age = 22;
    int *p = &age;
    
    printf("\n1-> %d",age);
    printf("\n2-> %p",&age);
    printf("\n3-> %p",p);
    printf("\n4-> %p",&p);
    
    return 0;
}
```
**⚙️ Output :** 
>1-> 22<br>
2-> 0x7ffdc6aa44fc<br>
3-> 0x7ffdc6aa44fc<br>
4-> 0x7ffdc6aa4500<br>

<br>

**Dereferencing**

*Dereferencing a pointer means getting the value that is stored in the memory location pointed by the pointer.*

* *-> dereferencing operator
* *-> asterik/star
* *-> value of
* *-> indirection operator

**💻Example 6 :**
```c
#include <stdio.h>

int main() {
    int age = 22;
    int *p = &age;
    
    printf("\n1-> %d",age);
    printf("\n2-> %p",&age);
    printf("\n3-> %p",p);
    printf("\n4-> %p",&p);
    printf("\n5-> %d",*p);
    
    return 0;
}
```
**⚙️ Output :** 
>1-> 22<br>
2-> 0x7fff4e58c3dc<br>
3-> 0x7fff4e58c3dc<br>
4-> 0x7fff4e58c3e0<br>
5-> 22<br>

**💻Example 7 :**
```c
#include <stdio.h>

int main() {
    int age = 22;
    int *p = &age;
    
    printf("\n1-> %d",age);
    printf("\n2-> %p",&age);
    printf("\n3-> %p",p);
    printf("\n4-> %p",&p);
    printf("\n5-> %d",*p);
    printf("\n6-> %p",*(&p));
    
    return 0;
}
```
**⚙️ Output :** 
>1-> 22<br>
2-> 0x7fff9cb6955c<br>
3-> 0x7fff9cb6955c<br>
4-> 0x7fff9cb69560<br>
5-> 22<br>
6-> 0x7fff9cb6955c<br>

<br>

**💻Example 8 :**
```c
#include <stdio.h>

int main() {
    int age = 22;
    int *p = &age;
    
    printf("\n1-> %d",age);
    printf("\n2-> %p",&age);
    printf("\n3-> %p",p);
    printf("\n4-> %p",&p);
    printf("\n5-> %d",*p);
    printf("\n6-> %p",*(&p));
    printf("\n7-> %d",*(&age));
    
    return 0;
}

```
**⚙️ Output :** 
>1-> 22<br>
2-> 0x7ffca32b909c<br>
3-> 0x7ffca32b909c<br>
4-> 0x7ffca32b90a0<br>
5-> 22<br>
6-> 0x7ffca32b909c<br>
7-> 22<br>

<br>
## Pointers

**💻Example 1 :**

```c
#include <stdio.h>

int main() {
    
    int num;
    
    int *p = &num;
    printf("Enter Number: ");
    scanf("%d", p);
    
    printf("Value is: %d", num);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Number: 10<br>
Value is: 10<br>

<br>