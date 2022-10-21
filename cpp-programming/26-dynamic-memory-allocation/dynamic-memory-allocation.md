## Dynamic Memory Allocation

### Dynamic Memory Allocation : 

Dynamic memory allocation is the process of assigning the memory space during the execution time or the run time.

```cpp

     
stack       
[  ]            
[  ]
[  ]
[  ]
[  ]

```

```cpp
            delete
[  ( )  ]    
[  /|\  ]     ❌
[  / \  ]
             new

int num; <---- 4byte
--->
--->

```


```cpp
int *ptr;  <--- create a pointer

ptr = new int;
       |
       |________[  19  ]
            (101) 4 byte

*ptr = 19;
cout<< *ptr;

delete ptr;
```

*💻Example 1:*

```cpp

    #include <iostream>
    using namespace std;
    int main() {

        int *ptr = new int;

        *ptr = 10;

        cout<<"Initial Value: "<<*ptr<<endl;

        delete ptr;

        cout<<"Final Value: "<<*ptr<<endl;

        return 0;
    }
```

*⚙️ Output :*
>Initial Value: 10<br>
Final Value: 0


<br>

```cpp

int arr[100];

n = 10;   loop --->10 times

int arr[10];     4*100
                 =>400
                 
```

```cpp
           Array
int *ptr;   

ptr = new int[4];
 |
 |    0     1     2    3
 |__ [0 ][ 20 ][ 15 ][ 7 ]
   =>100  104   108  112

*ptr = 10;
*(ptr + 1) = 20;
*(ptr + 2) = 15;
*(ptr + 3) = 7;

```

```cpp
     0    1     2   3
arr[ 7 ][ 6 ][ 8 ][ 3 ]
   100  104  108   112

newArray[ 7 ][ 6 ][ 3 ]
        200   204  208
```

*💻Example 2:*
```cpp
    #include <iostream>
    using namespace std;
    int main() {
        int n = 4;
        
        int* ptr = new int[n];
        
        *(ptr+0) = 10;
        *(ptr+1) = 20;
        *(ptr+2) = 30;
        *(ptr+3) = 40;
        
        cout<<"arr[0]:"<< *(ptr+0)<<endl;
        cout<<"arr[1]:"<< *(ptr+1)<<endl;
        cout<<"arr[2]:"<< *(ptr+2)<<endl;
        cout<<"arr[3]:"<< *(ptr+3)<<endl;
   
        return 0;
    }

```

*⚙️ Output :*
>arr[0]:10<br>
arr[1]:20<br>
arr[2]:30<br>
arr[3]:40<br>

*💻Example 3:*
```cpp
#include <iostream>
using namespace std;
int main() {
    int n;
   cout<<"Enter size of array: ";
   cin>>n;
    
    int* ptr = new int[n];
    
    for(int i=0; i<n; i++)
    {
        cout<<"Enter val for "<<i<<" position:";
        cin>> *(ptr+i);
    }
    
    for(int i=0; i<n; i++)
    {
        cout<<"arr["<<i<<"]: "<<*(ptr+i)<<endl;
    }
    
    delete [] ptr;

        return 0;
    }
```

*⚙️ Output :*
>Enter size of array: 3<br>
Enter val for 0 position:5<br>
Enter val for 1 position:6<br>
Enter val for 2 position:7<br>
arr[0]: 5<br>
arr[1]: 6<br>
arr[2]: 7<br>


## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References