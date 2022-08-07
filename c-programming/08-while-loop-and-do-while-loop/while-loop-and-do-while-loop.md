# While loop & Do-while loop in C Programming           

## While Loop

* Entry Controlled
* Pre-Tested Loop
* if condition will false it will run zero times 

**Syntax:**
```c
while(condition)
{

}
```

**💻Example :**

```c
#include <stdio.h>

int main() {
    
    int i=0;
    
    while(i<5)
    {
        printf("\n%d",i);
        
        i++;
    }
    return 0;
}
```
**⚙️ Output :** 
0       
1       
2       
3    
4  

## Do-While Loop

* Exit Controlled
* Post-Tested Loop 
* if condition will false it will run ones

**Syntax:**
```c
do
{
 
}
while(condition);
```

**💻Example:**
```c
#include <stdio.h>

int main() {
    
    int i=0;
    
    do
    {
        printf("\n%d",i);
        
        i++;
    }
    
    while(i<5);
    
    return 0;
}
```
**⚙️ Output :** 
>0     
1     
2      
3    
4    
