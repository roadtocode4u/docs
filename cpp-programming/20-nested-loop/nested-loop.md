## Nested Loop
 
### Nested Loop

Nested loop means a loop statement inside another loop statement

**Syntax :**
```cpp
for ( initialization; condition; increment ) {

   for ( initialization; condition; increment ) {
      
      // statement of inside loop
   }

   // statement of outer loop
}
```

**💻Example 1️:**

```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        for(int j=1; j<=2; j++)
        {
            cout<<j<<" ";
        }
    }
    return 0;
}
```
**⚙️ Output :**
>1 2 1 2 1 2 1 2 1 2  

**💻Example 2:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        for(int j=1; j<=2; j++)
        {
            cout<<j<<" ";
        }
        cout<<"Loop khatam"<<endl;
    }
    return 0;
}
```
**⚙️ Output :**
>1 2 Loop khatam<br>
1 2 Loop khatam<br>
1 2 Loop khatam<br>
1 2 Loop khatam<br>
1 2 Loop khatam<br>

**💻Example 3:**
```cpp

#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        cout<<"i: "<<i<<endl;
        for(int j=1; j<=2; j++)
        {
            cout<<j<<" ";
        }
        cout<<"Loop khatam"<<endl;
    }
    return 0;
}
```
**⚙️ Output :**
>i: 1<br>
1 2 Loop khatam<br>
i: 2<br>
1 2 Loop khatam<br>
i: 3<br>
1 2 Loop khatam<br>
i: 4<br>
1 2 Loop khatam<br>
i: 5<br>
1 2 Loop khatam<br>

**💻Example 4:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        cout<<"i: "<<i<<endl;
        for(int j=1; j<=5; j++)
        {
            cout<<j<<" ";
        }
        cout<<"Loop khatam"<<endl;
    }
    return 0;
}

```
**⚙️ Output :**
>i: 1<br>
1 2 3 4 5 Loop khatam<br>
i: 2<br>
1 2 3 4 5 Loop khatam<br>
i: 3<br>
1 2 3 4 5 Loop khatam<br>
i: 4<br>
1 2 3 4 5 Loop khatam<br>
i: 5<br>
1 2 3 4 5 Loop khatam<br>

**💻Example 5:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        for(int j=1; j<=3; j++)
        {
            cout<<"@";
        }
        cout<<endl;
    }
    return 0;
}
```
**⚙️ Output :**
> @@@<br>
@@@<br>
@@@<br>
@@@<br>
@@@<br>

**💻Example 6:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        for(int j=1; j<=10; j++)
        {
            cout<<j<<" ";
        }
        cout<<endl;
    }
    return 0;
}

```
**⚙️ Output :**
>1 2 3 4 5 6 7 8 9 10 <br>
1 2 3 4 5 6 7 8 9 10 <br>
1 2 3 4 5 6 7 8 9 10 <br>
1 2 3 4 5 6 7 8 9 10 <br>
1 2 3 4 5 6 7 8 9 10 <br>

**💻Example 6:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        for(int j=1; j<=i; j++)
        {
            cout<<j<<" "; 
        }
        cout<<endl;
    }
    return 0;
}
```
**⚙️ Output :**
>1 <br>
1 2 <br>
1 2 3 <br>
1 2 3 4 <br>
1 2 3 4 5 <br>


**💻Example 7:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=1; i<=5; i++)
    {
        for(int j=1; j<=i; j++)
        {
            cout<<i<<" "; 
        }
        cout<<endl;
    }
    return 0;
}
```
**⚙️ Output :**
>1 
2 2 
3 3 3 
4 4 4 4 
5 5 5 5 5 

**💻Example 8:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int count=1;
    for(int i=1; i<=5; i++)
    {
        for(int j=1; j<=i; j++)
        {
            cout<<count<<" ";
            count++;
        }
        cout<<endl;
    }
    return 0;
}
```
**⚙️ Output :**
>1 <br>
2 3 <br>
4 5 6 <br>
7 8 9 10 <br>
11 12 13 14 15<br> 


## 🏠  HomeWork

## 🔗 Some Useful Links


## 📖 References