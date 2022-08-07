# Loops in C Programming 

## Loops

### Types of Loops
 
  * For-Loop
  * While Loop
  * Do-While Loop

### For Loop 

   For loops are used when you have a block of code which you want to repeat a fixed number of times.


**💻Example:**
```c
#include <stdio.h>

int main() {
    
    for(int i=0;i<=5; i++)
    {
        printf("\nHello ");
    }
    return 0;
}
```
**⚙️ Output :**
>Hello    
Hello    
Hello     
Hello     
Hello    
Hello     

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int n;
    printf("Enter Number :");
    scanf("%d",&n);
    
    for(int i=1;i<=n; i++)
    {
        printf("\nHello ");
    }
    return 0;
}
```
**⚙️ Output :**
>Enter Number :5     
Hello     
Hello    
Hello      
Hello    
Hello    

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int n;
    printf("Enter Number :");
    scanf("%d",&n);
    
    for(int i=1;i<=n; i++)
    {
        printf("\nXerox... %d",i);
    }
    return 0;
}
```
**⚙️ Output :**
>Enter Number :3    
Xerox... 1    
Xerox... 2    
Xerox... 3  

**💻Example:**
```c
#include <stdio.h>

int main() {
 
    for(int i=5;i>=0; i--)
    {
        printf("\n%d",i);
    }
    return 0;
}
```
**⚙️ Output :**
>5         
4           
3             
2            
1          
0 

# Practice Questions In Loops in C Programming 

## Practice Question in Loops

**💻Example:**
```c
//Odd Numbers 

#include <stdio.h>

int main() {
    
    int n;
    printf("Enter Number :");
    scanf("%d",&n);
    
    for(int i=1;i<=n;i++)
    {
        if(i%2==1)
        {
            printf("\n%d",i);
        }
    }
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Number :5   
1         
3         
5      

**💻Example:**
```c
// Even Numbers 
#include <stdio.h>

int main() {
    
    int n;
    printf("Enter Number :");
    scanf("%d",&n);
    
    for(int i=2;i<=n;i++)
    {
        if(i%2==0)
        {
            printf("\n%d",i);
        }
    }
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Number :10          
2         
4           
6         
8        
10                   

**💻Example:**
```c
// Sum of  Numbers 
#include <stdio.h>

int main() {
    
    int n=3;
    
    printf("Enter Number :");
    scanf("%d",&n);
    
    int sum=0;
    
    for(int i=1;i<=n;i++)
    {
        sum=sum+i;
    }
    
    printf("Sum=%d",sum);
    
    return 0;
}
```
**⚙️ Output :**
>Enter Number :10    
Sum=55        

**💻Example:**
```c
// Factorial Of Numbers 
#include <stdio.h>

int main() {
    
    int n;
    printf("Enter Number :");
    scanf("%d",&n);
    
    int fact=1;
    
    for(int i=1;i<=n;i++)
    {
        fact=fact * i;
    }
    
    printf("Factorial=%d",fact);
    return 0;
}
```
**⚙️ Output :**
>Enter Number :5       
Factorial=120  

**💻Example:**
```c

#include <stdio.h>

int main() {
    
    int n;
    printf("Enter Number :");
    scanf("%d",&n);
    
    for(int i=1;i<=n;i++)
    {
        if(i%3==0 && i%5==0)
        {
            printf("\n%d is Divisible by both ",i);
        }
        else if (i%3==0 && i%5==0)
        {
            printf("\n%d is Divisible by 3 Or 5",i);
        }
        else
        {
            printf("\n%d is not Divisible by 3 Or 5",i);
        }
    }
    
    return 0;
}
```
**⚙️ Output :** 
>Enter Number :15           
1 is not Divisible by 3 Or 5             
2 is not Divisible by 3 Or 5   
3 is not Divisible by 3 Or 5     
4 is not Divisible by 3 Or 5          
5 is not Divisible by 3 Or 5          
6 is not Divisible by 3 Or 5           
7 is not Divisible by 3 Or 5      
8 is not Divisible by 3 Or 5      
9 is not Divisible by 3 Or 5         
10 is not Divisible by 3 Or 5         
11 is not Divisible by 3 Or 5           
12 is not Divisible by 3 Or 5          
13 is not Divisible by 3 Or 5          
14 is not Divisible by 3 Or 5           
15 is Divisible by both      


# Example Of Loop in C Programming 

**💻Example:**

```c
#include <stdio.h>

int main() {
    
    int i=1;
    
    while(i<=10)
    {
        if(i==5)
        {
            i++;
            continue;
        }
        printf("%d\n",i);
         i++;
    }
    
    return 0;
}
```
**⚙️ Output :** 
>1           
2       
3         
4         
6           
7           
8         
9      
10             


**💻Example:**

```c
#include <stdio.h>

int main() {
    
    int i=1;
    
    do
    {
         if(i==5)
         {
           break;
         }
         printf("\n%d",i);
         i++;
    }
    while(i<10);
    
    
    return 0;
}
```
**⚙️ Output :** 
>1       
2        
3       
4      
                   
**💻Example :**

```c
#include <stdio.h>

int main() {
    
    int i=1;
    
    do
    {
         if(i==5)
         {
             i++;
           continue;
         }
         printf("\n%d",i);
         i++;
    }
    while(i<10);
    
    
    return 0;
}
```
**⚙️ Output :** 
>0     
1     
2      
3    
4   
5    
6    
7    
8   
9

**💻Example :**

```c
#include <stdio.h>

int main() {
    
    for(int i=1;i<=5;i++)
    {
        int roll;
        printf("\nEnter Roll:");
        scanf("%d",&roll);
        printf("\n Your roll is:%d",roll);
    }
    return 0;
}
```
**⚙️ Output :** 
>Enter Roll:1    
Your roll is:1   
Enter Roll:2   
Your roll is:2 

**💻Example :**

```c
#include <stdio.h>

int main() { 
    char ch=1;
    
    while(ch==1)
    {
        printf("\nHello");
        printf("\n Do you want to Continue (1/0):");
        scanf("%d",&ch);
    }
    return 0;
}
```
**⚙️ Output :** 
>Hello     
 Do you want to Continue (1/0):1     
 Hello                          
 Do you want to Continue (1/0):1        
 Hello  
 Do you want to Continue (1/0):1     
 Hello        
 Do you want to Continue (1/0): 

 **Homework 🏠**
 > Write a C Program to reverse number using while loop 
