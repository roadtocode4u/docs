# Switch case in C Programming 

## Switch case

The switch statement allows us to execute one code block among many alternatives.

**Syntax:**
```c
switch (ch)
​{
    case 1:
      // statements
      break;

    case 2:
      // statements
      break;
   
    default:
      // default statements
}

```

**💻Example:**

```c
//Switch case 

#include <stdio.h>

int main() {
    int n;
    printf("Enter value of n: ");
    scanf("%d", &n);
    
    switch(n)
    {
        case 1:
            printf("One");
        break;
        
        case 2:
            printf("Two");
        break;
        
        case 3:
            printf("Three");
        break;
    }
}
```
**⚙️ Output :** 
>Enter value of n: 1 <br>
One        

## Switch case without using break statement

If we don't use **break** then next case statements will be executed until break appears.

**💻Example:**

```c
// Switch case without using break statement

#include <stdio.h>

int main() {
    int n;
    printf("Enter value of n: ");
    scanf("%d", &n);
    
    switch(n)
    {
        case 1:
            printf("One");
        
        case 2:
            printf("Two");
        
        case 3:
            printf("Three");
    }
    return 0;
}
```
**⚙️ Output :** 
>Enter value of n: 1 <br>
OneTwoThree               

**💻Example :**

```c
#include <stdio.h>

int main(){
    
    char ch;
    printf("Enter Alphabet : ");
    scanf("%c",&ch);
    
    if(ch=='a' || ch=='e' || ch=='i' || ch=='o' || ch=='u')
    {
        printf("Vowel");
    }
    else
    {
        printf("Consonant");
    }
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Alphabet : a<br>
Vowel<br>
Enter Alphabet : b<br>
Consonant

**🏠Homework**
> Write a C program to calculate area of rectangle, square, circle and triangle.

