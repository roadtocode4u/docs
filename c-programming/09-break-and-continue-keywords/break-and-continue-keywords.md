# Break & Continue Keyword in C Programming 

## Break  Keyword

Break keyword are used to stop loop permanently.

**💻Example:**

```c
//Break Keyword 

#include <stdio.h>

int main() {
    
    for(int i=1;i<=10;i++)
    {
        if(i==5)
        {
            break;
        }
        printf("\n%d",i);
    }
    
    return 0;
}
```
**⚙️ Output :** 
>1           
2         
3          
4          

## Continue Keyword

continue keyword are used to stop current loop.

**💻Example:**

```c
//continue Keyword 

#include <stdio.h>

int main() {
    
    for(int i=1;i<=10;i++)
    {
        if(i==5)
        {
            continue;
        }
        printf("\n%d",i);
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

