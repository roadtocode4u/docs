
## Linear Search, Largest Element From An Array

**💻Example 1️:**
```cpp
    #include <iostream>
    using namespace std;
    int main() {

        int arr[5];
        cout<<"Enter 5 values: ";

        for(int i=0; i<5 i++)
        {
            cin>>arr[i];
        }
        cout<<"\n Values from user are: ";
        for(int i=0; i<=5; i++)
        {
            cout<<arr[i]<<", ";
        }
       
        return 0;
    }

```
**⚙️ Output :**
>Enter 5 values: 2 4 6 8 10<br>
Values from user are: 2, 4, 6, 8, 10,

### Linear Search (one Line)
```cpp
yash ---> 7


 0  1  2  3  4    //index
[4][8][2][7][9]   //position
---------------->

<---------------

key / query <--- user

for --- i=0 to 4

arr[i] == key
```

**💻Example 2:**
```cpp
    #include <iostream>
    using namespace std;
    int main() {
       
       int arr[5];

       cout<<"Enter 5 Elements in Array: ";

       for(int i=0; i<5; i++)
       {
        cin>>arr[i];
       }
       
       int key;
       cout<<"Enter key to search: ";
       cin>>key;

       for(int i=0; i<5; i++)
       {
        if(key==arr[i])
        {
            cout<<"key found at: "<<i<<endl;
        }
       }
        return 0;
    }

```
**⚙️ Output :**
>Enter 5 Elements in Array: 2 4 6 7 8<br>
Enter key to search: 6<br>
key found at: 2

```cpp
example 3 explanation : 

for(int i=0; i<5; i++)
       {
        if(key==arr[i])
        {
            flag = i;
            cout<<"Key found at: "<<i<<endl;
            break;
        }
       }

     0  1  2  3  4
    [8][4][6][5][3]
    key = 5

    i=0 => (5 == 8) ?
    i=1 => (5 == 4) ?
    i=2 => (5 == 6) ?
    i=3 => (5 == 5) true

    flag = 3
    key found at 3
```

**💻Example 3:**
```cpp
    #include <iostream>
    using namespace std;
    int main() {
       
       int arr[5];

       cout<<"Enter 5 Elements in Array: ";

       for(int i=0; i<5; i++)
       {
        cin>>arr[i];
       }
       
       int key;
       cout<<"Enter key to search: ";
       cin>>key;

       int flag = -1;

       for(int i=0; i<5; i++)
       {
        if(key==arr[i])
        {
            flag = i;
            cout<<"Key found at: "<<i<<endl;
            break;
        }
       }
       if(flag== -1)
       {
        cout<<"Element Not found";
       }

        return 0;
    }

```
**⚙️ Output :**
>Enter 5 Elements in Array: 2 4 6 7 8<br>
Enter key to search: 10<br>
Element Not found

```cpp
example 4 explanation : 

 0  1  2   3  4   5
[8][5][15][9][51][80]
                   |

{80} => Biggest number
```
**💻Example 4:**
```cpp
    #include <iostream>
    using namespace std;
    int main() {
       
       int arr[5];

       cout<<"Enter 5 Elements in Array: ";

       for(int i=0; i<5; i++)
       {
        cin<<arr[i];
       }

       int biggest = arr[0];

       for(int i=1; i<5; i++)
       {
        if(arr[i]>biggest)
        {
            biggest = arr[i];
        }
       }

       cout<<"Biggest Number is "<<biggest;

        return 0;
    }
```
**⚙️ Output :**
>Enter 5 Elements in Array : 3 17 6 4 9<br>
Biggest Number is 17

## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References
