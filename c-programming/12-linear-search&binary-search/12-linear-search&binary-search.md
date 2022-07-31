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

# ASCII in C Programming 

## ASCII

**ASCII stands for American Standard Code for Information Interchange.**<br>
_ASCII in C is used to represent numeric values for each character._

**💻Example 1 :**

```c
#include <stdio.h>

int main() {
    char alpha = 'A';
    
    printf("%d", alpha);
    return 0;
}
```
**⚙️ Output :** 
>65

**💻Example 2 :**
```c
#include <stdio.h>

int main() {
    char alpha = 'b';
    
    printf("%d", alpha);
    return 0;
}
```
**⚙️ Output :** 
>98

**💻Example 3 :**
```c
#include <stdio.h>

int main() {
    char alpha = 65;
    
    printf("%c", alpha);
    return 0;
}
```
**⚙️ Output :** 
>A

**💻Example 4 :**
```c
#include <stdio.h>

int main() {
    for(int i=0; i<=127; i++)
    {
        printf("\n%d =>%c ",i,i);
    }
    return 0;
}

```
**⚙️ Output :** 
>32 =>   <br>
33 => ! <br>
34 => " <br>
35 => # <br>
36 => $ <br>
37 => % <br>
38 => & <br>
39 => ' <br>
40 => ( <br>
41 => ) <br>
42 => * <br>
43 => + <br>
44 => , <br>
45 => - <br>
46 => . <br>
47 => / <br>
48 => 0 <br>
49 => 1 <br>
50 => 2 <br>
51 => 3 <br>
52 => 4 <br>
53 => 5 <br>
54 => 6 <br>
55 => 7 <br>
56 => 8 <br>
57 => 9 <br>
58 => : <br>
59 => ; <br>
60 => < <br>
61 => = <br>
62 => > <br>
63 => ? <br>
64 => @ <br>
65 => A <br>
66 => B <br>
67 => C <br>
68 => D <br>
69 => E <br>
70 => F <br>
71 => G <br>
72 => H <br>
73 => I <br>
74 => J <br>
75 => K <br>
76 => L <br>
77 => M <br>
78 => N <br>
79 => O <br>
80 => P <br>
81 => Q <br>
82 => R <br>
83 => S <br>
84 => T <br>
85 => U <br>
86 => V <br>
87 => W <br>
88 => X <br>
89 => Y <br>
90 => Z <br>
91 => [ <br>
92 => \ <br>
93 => ] <br>
94 => ^ <br>
95 => _ <br>
96 => ` <br>
97 => a <br>
98 => b <br>
99 => c <br>
100 => d <br>
101 => e <br>
102 => f <br>
103 => g <br>
104 => h <br>
105 => i <br>
106 => j <br>
107 => k <br>
108 => l <br>
109 => m <br>
110 => n <br>
111 => o <br>
112 => p <br>
113 => q <br>
114 => r <br>
115 => s <br>
116 => t <br>
117 => u <br>
118 => v <br>
119 => w <br>
120 => x <br>
121 => y <br>
122 => z <br>
123 => { <br>
124 => | <br>
125 => } <br>
126 => ~ <br>
127 =>  <br>

**💻Example 5 :**
```c
#include <stdio.h>

int main() {
    
    char input;
    printf("Enter a Character: ");
    scanf("%c", &input);
    
    printf("%c", input);
    
    return 0;
}

```
**⚙️ Output :** 
>Enter a Character: A<br>
A

**💻Example 6 :**
```c
#include <stdio.h>

int main() {
    
    char input;
    printf("Enter a Character: ");
    scanf("%c", &input);
    
    input = input + 32;
    
    printf("small letter is %c", input);
    
    return 0;
}

```
**⚙️ Output :** 
>Enter a Character: G<br>
small letter is g

**💻Example 7 :**
```c
#include <stdio.h>

int main() {
    
    char input;
    printf("Enter a CAPITAL Character: ");
    scanf("%c", &input);
    
    if(input>=65 && input<=90)
    {
        input = input + 32;
    }
    
    printf("small letter is %c", input);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter a CAPITAL Character: a<br>
small letter is a


**💻Example 8 :**
```c
#include <stdio.h>

int main() {
    char word[10];
    
    printf("Enter a word in small letters: ");
    scanf("%s", word);
    
    int i=0;
    
    while(word[i]!='\0')
    {
        word[i] = (word[i] - 32);
        
        i++;
    }
    
    printf("CAPITAL WORD is: %s ", word);
    
    return 0;
}
```
**⚙️ Output :** 
>Enter a word in small letters: roadtocode<br>
CAPITAL WORD is: ROADTOCODE

**🏠Homework**
>i.  Write a C program to convert small character to capital.<br>
ii.  Write a C program to character from user and print wheather it is small or capital.

## 🔗 Some Useful Links
https://www.cs.cmu.edu/~pattis/15-1XX/common/handouts/ascii.html

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