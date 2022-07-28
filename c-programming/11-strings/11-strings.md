## String

A String in C is nothing but a collection of characters in a linear sequence. <br>*or*<br> Array of characters.<br><br>

**💻Example 1 :**

```c
#include <stdio.h>

int main() {
    char arr[10];
    
    printf("Enter name: ");
    scanf("%s",arr);
    
    printf("Hello %s",arr);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter name: Suraj<br>
Hello Suraj

<br>

*Assignment operator ( = ) : Assignment operators are used to assigning value to a variable.*<br><br>

_Without mentioning size_

**💻Example 2 :**
```c
#include <stdio.h>

int main() {
    char arr[] = {'r', 't', 'c', '\0'};
    
    printf("Hello %s", arr);
    
    return 0;
}
```
**⚙️ Output :** 
>Hello rtc

<br>

**💻Example 3 :**
```c
#include <stdio.h>

int main() {
    
    char str[100];
    printf("Enter Name: ");
    scanf("%s", str);
    
    printf("Hello %s", str);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Name: Suraj<br>
Hello Suraj

<br>

## WAP to find length of a string.
**💻Example 4 :**
```c
#include <stdio.h>

int main() {
    
    char str[100];
    printf("Enter Name: ");
    scanf("%s", str);
    
    for(int i=0; i<100; i++)
    {
        if(str[i]=='\0')
        {
            printf("%d", i);
            break;
        }
    }
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Name: Suraj<br>
5

**💻Example 5 :**
```c
#include <stdio.h>

int main() {
    
    char str[100];
    printf("Enter Name: ");
    scanf("%s", str);
    
    int count = 0;
    
    for(int i=0; i<100; i++)
    {
        if(str[i]=='\0')
        {
            break;
        }
        else
        {
            count++;
        }
    }
    printf("Length of string is: %d", count);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Name: Prajakta<br>
Length of string is: 8

<br>

**Using while loop**

**💻Example 6 :**
```c
#include <stdio.h>

int main() {
    
    char str[100];
    printf("Enter Name: ");
    scanf("%s", str);
    
    int count = 0;
    
    while(str[count]!='\0')
    {
        count++;
    }
    printf("Length of string is: %d", count);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Name: Suraj<br>
Length of string is: 5

<br>