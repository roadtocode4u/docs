# Array in C Programming 

## Array

An array is a variable that can store multiple values.

**Syntax :**
```c
datatype arrayname[size]

```

**💻Example :**

```c
//Array

int marks[5];
```
**💻Example 1 :**

```c
#include <stdio.h>

int main() {
    int marks[5];
    
    marks[0] = 10;
    marks[1] = 20;
    marks[2] = 30;
    marks[3] = 40;
    marks[4] = 50;
    
    printf("\n%d", marks[0]);
    printf("\n%d", marks[1]);
    printf("\n%d", marks[2]);
    printf("\n%d", marks[3]);
    printf("\n%d", marks[4]);
    
    return 0;
}
```
**⚙️ Output :** 
>10<br>
20<br>
30<br>
40<br>
50<br>

**💻Example 2 :**
```c
#include <stdio.h>

int main() {
    int marks[5];
    
    marks[0] = 10;
    marks[1] = 20;
    marks[2] = 30;
    marks[3] = 40;
    marks[4] = 50;
    
    for(int i=0;i<=4; i++){
    printf("\n%d", marks[i]);
    }
    
    return 0;
}
```
**⚙️ Output :** 
>10<br>
20<br>
30<br>
40<br>
50<br>

**💻Example 3 :**
```c
#include <stdio.h>

int main() {
    int marks[5];

    for(int i=0;i<=4; i++)
    {
    printf("\nEnter marks for %d :", i);
    scanf("%d", &marks[i]);
    }
    for(int i=0; i<=4; i++)
    {
        printf("\n%d", marks[i]);
    }
    
    return 0;
}
```
**⚙️ Output :** 
>Enter marks for 0 :10<br>
Enter marks for 1 :20<br>
Enter marks for 2 :30<br>
Enter marks for 3 :40<br>
Enter marks for 4 :50<br>
10<br>
20<br>
30<br>
40<br>
50<br>

**💻Example 4 :**
```c
#include <stdio.h>

int main() {
    int arr[5] = {5, 10, 15, 20, 25};
    
    for(int i=0; i<5; i++)
    {
        printf("\n%d", arr[i]);
    }
    return 0;
}
```
**⚙️ Output :** 
>5<br>
10<br>
15<br>
20<br>
25<br>


## Reverse an Array

Q1. Print an array in reverse format.


**💻Example 1 :**

```c
#include <stdio.h>

int main() {
    
    int arr[6] = {18, 2, 17, 19, 21, 45};
    
    for(int i=5; i>=0; i--)
    {
        printf("%d, ", arr[i]);
    }
    
    return 0;
}
```
**⚙️ Output :** 
>45, 21, 19, 17, 2, 18, 

**💻Example 2 :**
```c
#include <stdio.h>

int main() {
    
    int arr[6] = {18, 2, 17, 19, 21, 45};
    
      printf("\n Before Reverse: ");
    for(int i=0; i<6; i++)
    {
        printf("%d, ",arr[i]);
    }
    
    int start=0;
    int end=5;
    
    while(start<end)
    {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;
        
        start++;
        end--;
    }
    printf("\n After Reverse: ");
    for(int i=0; i<6; i++)
    {
        printf("%d, ",arr[i]);
    }
    
    return 0;
}
```
**⚙️ Output :** 
>Before Reverse: 18, 2, 17, 19, 21, 45, <br>
After Reverse: 45, 21, 19, 17, 2, 18, 