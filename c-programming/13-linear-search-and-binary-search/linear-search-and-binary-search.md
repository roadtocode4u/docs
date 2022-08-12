# Linear Search, Sum of Array Elements and Largest Element from the Array in C Programming 

## Linear Search

Linear search is a search that finds an element in the list by searching the element sequentially until the element is found in the list.


**💻Example 1 :**

```c
#include <stdio.h>

int main() {
    
    int arr[10]={2, 4, 6, 78, 34, 12, 23, 98, 43, 22};
    
    int key = 12; 
    
    for(int i=0; i<10; i++)
    {
        if(arr[i]==key)
        {
            printf("Element found at %d", i);
            break;
        }
    }
    return 0;
}
```
**⚙️ Output :** 
>Element found at 5

**💻Example 2 :**
```c
#include <stdio.h>

int main() {
    
    int arr[10]={2, 4, 6, 78, 34, 12, 23, 98, 43, 22};
    
    int key; 
    printf("Enter key: ");
    scanf("%d", &key);
    
    for(int i=0; i<10; i++)
    {
        if(arr[i]==key)
        {
            printf("%d found at %d index",key, i);
            break;
        }
    }
    return 0;
}
```
**⚙️ Output :** 
>Enter key: 12<br>
12 found at 5 index

**💻Example 3 :**
```c
#include <stdio.h>

int main() {
    
    int arr[100];
    
    int n; 
    printf("How many elements do you want to add: ");
    scanf("%d", &n);
    
    for(int i=0; i<n; i++)
    {
        printf("Enter value for index %d: ",i);
        scanf("%d", &arr[i]);
    }
    int key;
    printf("Enter key: ");
    scanf("%d", &key);
    
    for(int i=0; i<n; i++)
    {
        if(arr[i]==key)
        {
            printf("%d found at %d index",key, i);
            break;
        }
    }
    return 0;
}
```
**⚙️ Output :** 
>How many elements do you want to add: 5<br>
Enter value for index 0: 2<br>
Enter value for index 1: 34<br>
Enter value for index 2: 52<br>
Enter value for index 3: 12<br>
Enter value for index 4: 22<br>
Enter key: 52<br>
52 found at 2 index

<hr>

## Flag Variable

A flag variable is usually given two values 0 (False) and 1 (True) . So, its used as a Boolean variable.

**💻Example 4 :**
```c
#include <stdio.h>

int main() {
    
    int arr[100];
    
    int n; 
    printf("How many elements do you want to add: ");
    scanf("%d", &n);
    
    for(int i=0; i<n; i++)
    {
        printf("Enter value for index %d: ",i);
        scanf("%d", &arr[i]);
    }
    int key;
    printf("Enter key: ");
    scanf("%d", &key);
    
    int flag = 0;
    
    for(int i=0; i<n; i++)
    {
        if(arr[i]==key)
        {
            printf("%d found at %d index",key, i);
            flag=1;
            break;
        }
    }
    
    if(flag==0)
    {
        printf("Element not found");
    }
    return 0;
}
```
**⚙️ Output :** 
>How many elements do you want to add: 4<br>
Enter value for index 0: 12<br>
Enter value for index 1: 24<br>
Enter value for index 2: 36<br>
Enter value for index 3: 48<br>
Enter key: 36<br>
36 found at 2 index<br>

**💻Example 5 :**
```c
#include <stdio.h>

int main() {
    
    int arr[100];
    
    int n; 
    printf("How many elements do you want to add: ");
    scanf("%d", &n);
    
    for(int i=0; i<n; i++)
    {
        printf("Enter value for index %d: ",i);
        scanf("%d", &arr[i]);
    }
    int key;
    printf("Enter key: ");
    scanf("%d", &key);
    
    int flag = 0;
    
    for(int i=0; i<n; i++)
    {
        if(arr[i]==key)
        {
            printf("%d found at %d index",key, i);
            flag=1;
            break;
        }
    }
    
    if(flag==0)
    {
        printf("Element not found");
    }
    return 0;
}
```
**⚙️ Output :** 
>How many elements do you want to add: 4<br>
Enter value for index 0: 12<br>
Enter value for index 1: 24<br>
Enter value for index 2: 36<br>
Enter value for index 3: 48<br>
Enter key: 40<br>
Element not found

<br>

**Sum of Array Elements**

**💻Example 6 :**
```c
#include <stdio.h>

int main() {
    int marks[] = {10, 20, 30, 40, 50};
    
    int sum = 0;
    
    for(int i=0; i<5; i++)
    {
        sum = sum + marks[i];
    }
    
    printf("Sum of marks: %d",sum);
    
    return 0;
}
```
**⚙️ Output :** 
>Sum of marks: 150

<br>

**Largest Element from the Array**

**💻Example 7 :**
```c
#include <stdio.h>

int main() {
    
    int arr[6];
    printf("Enter 6 values: \n");
    
    for(int i=0; i<6; i++)
    {
        printf("Enter value for index %d: ", i);
        scanf("%d", &arr[i]);
    }
    
    int max = arr[0];
    for(int i=0; i<6; i++)
    {
        if(arr[i]>max)
        {
            max = arr[i];
        }
    }
    
    printf("Maximum value from array is: %d", max);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter 6 values: <br>
Enter value for index 0: 12<br>
Enter value for index 1: 24<br>
Enter value for index 2: 56<br>
Enter value for index 3: 23<br>
Enter value for index 4: 6<br>
Enter value for index 5: 58<br>
Maximum value from array is: 58

**🏠Homework**
> Write a C program to find smallest element from an array

#  Binary Search in C Programming 
## Binary Search

**Binary Search is a search algorithm that is used to find the position of an element in a sorted array.**
<br>

**💻Example 1 :**

```c
#include <stdio.h>

int main() {
   int arr[] = {1, 5, 4, 7, 45, 23, 56};
   
   int key = 56;
   
   for(int i=0; i<7; i++)
   {
       if(arr[i]==key)
       {
           printf("Element found at %d",i);
           break;
       }
   }
    
    return 0;
}

```
**⚙️ Output :** 
>Element found at 6

<br>

### *Binary means (divide and conquer)*

* Bi   => Two
* n    => n
* ary  => array

<br>

**RULE**

* Data should be sorted


**FORMULA**

* mid = (start+end)/2 
* end=mid-1
* start=mid+1
* (start+end)/2

<br>

<p align="center">
  <img  src="./../assets/binary.png"/>
</p>

**💻Example 2 :**

```c
#include <stdio.h>

int main() {
   int arr[] = {1, 2, 5, 7, 9, 12, 17, 22, 25, 30};
   
   int key = 25;
   int start = 0;
   int end = 9;
   
   while(start<=end)
   {
       int mid = (start+end)/2;
        if(arr[mid]==key)
        {
            printf("Element found at %d", mid);
            break;
        }
        else if(key>arr[mid])
        {
            start = mid + 1;
        }
        else
        {
            end = mid -1;
        }
   }
    
    return 0;
}
```
**⚙️ Output :** 
>Element found at 8

**🏠Homework**

## 🔗 Some Useful Links
https://www.cs.usfca.edu/~galles/visualization/Search.html