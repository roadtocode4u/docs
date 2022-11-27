## 2D Array

```cpp
1. 1D - Array
int arr[5];

    0 1  2 3 4
--->[][][5][][] //one dimentional array 

    index
    |
arr[2];
```

```cpp
2. 2D - Array

  bus
[1][2]    [][][][][]
[3][4]
[5][6]
[7][8]
[9][0]

syntax : 
datatype array-name[row][col];


       row col 
        |  |
int arr[4][3]
                                          
                                           row col
                                             |  |
            columns                      arr[1][2]
             0      1      2              |
             |      |      |              |
      0-->[(0,0)][(0,1)][(0,2)]           |
rows  1-->[(1,0)][(1,1)][(1,2)] <----------
      2-->[(2,0)][(2,1)][(2,2)]<= cell
      3-->[(3,0)][(3,1)][(3,3)]
```
```cpp
example 1 explanation: 
int arr[3][4]; //3 rows 4 columns
  
   0  1  2  3
   |  |  |  |
0 [ ][ ][8][ ]         arr[0][2] = 8;
1 [5][ ][ ][ ]         arr[2][3] = 7;
2 [ ][3][ ][7]         arr[1][0] = 5;
                       arr[2][1] = 3;
```

**💻Example 1️:**
```cpp
    #include <iostream>
    using namespace std;
    int main() {

        int arr[3][4];

        arr[0][2]=8;
        arr[2][3]=7;
        arr[1][0]=5;
        arr[2][1]=3;

        cout<<arr[0][2]<<endl;
        cout<<arr[2][3]<<endl;
        cout<<arr[1][0]<<endl;
        cout<<arr[2][1]<<endl;

        return 0;
    }
```
**⚙️ Output :**
>8<br>7<br> 5<br> 3

**💻Example 2:**
```cpp
    #include <iostream>
    using namespace std;
    int main() {

        int arr[3][4];

       for(int i=0; i<3; i++)
       {
        for(int j=0; j<4; j++)
        {
            cout<<"Enter value of: ["<<i<<"]["<<j<<"]: ";
            cin>>arr[i][j];
       }
       }
        for(int i=0; i<3; i++)
       {
        for(int j=0; j<4; j++)
        {
            cout<<arr[i][j]
        }
       cout<<endl;
       }
       return 0;
    }
```
**⚙️ Output :**
>Enter val of[0][0]: 2<br>
Enter val of[0][1]:  5<br>
Enter val of[0][2]:  8<br>
Enter val of[0][3]:  7<br>
Enter val of[1][0]:  11<br>
Enter val of[1][1]:  45<br>
Enter val of[1][2]:  49<br>
Enter val of[1][3]:  34<br>
Enter val of[2][0]:  6<br>
Enter val of[2][1]:  7<br>
Enter val of[2][2]:  8<br>
Enter val of[2][3]:  9<br>
2587<br>
11454934<br>
6789

```cpp
int [3][2] ={{5,2},{8,10}, {16,21}};
             ____   ____     ____
               r=1   r=2      r=3

  0   1
0[5 ][2]
1[8 ][10]
2[16][21]
```

**💻Example 3:**
```cpp
    #include <iostream>
    using namespace std;
    int main() {

        int arr[3][4]={
                       {1, 2, 3, 4}, 
                       {5, 6, 7, 6}, 
                       {5, 4, 3, 2}
                      };

       for(int i=0; i<3; i++)
       {
        for(int j=0; j<4; j++)
        {
            cout<<"Enter value of: ["<<i<<"]["<<j<<"]: ";
            cin>>arr[i][j];
       }
       }
        for(int i=0; i<3; i++)
       {
        for(int j=0; j<4; j++)
        {
            cout<<arr[i][j]
        }
       cout<<endl;
       }
       return 0;
    }
```
**⚙️ Output :**
>1234<br> 5676<br> 5432
## 🏠  HomeWork

## 🔗 Some Useful Links

## 📖 References