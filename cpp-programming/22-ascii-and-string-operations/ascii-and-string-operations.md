## ASCII and String Operations

ASCII (American Standard Code for Information Interchange) 

*ASCII Value of a Character*

```cpp
A -> 65               
B -> 66                   
C -> 67                
   .
   .
   .
Z -> 90


a -> 97
b -> 98
c -> 99
   .
   .
   .
z -> 122 
```

**💻Example 1️:**
```cpp
#include <iostream>
using namespace std;

int main() {
    char alpha = 'A';
    
    int val = alpha;
    cout<<"Char: "<<alpha<<endl;
    cout<<"ASCII: "<<val;   

    return 0;
}
```
**⚙️ Output :**
>Char: A<br>
ASCII: 65

**💻Example 2:**
```cpp
   #include <iostream>
using namespace std;

int main() {
    
int ascii = 65;

char alpha = ascii;

cout<<"ASCII: "<<ascii<<endl;
cout<<"Char: "<<alpha;

    return 0;
}
```
**⚙️ Output :**
>ASCII: 65<br>
Char: A

**💻Example 3:**
```cpp
  #include <iostream>
using namespace std;

int main() {
    
int ascii = 90;

cout<<char(ascii);

    return 0;
}
```
**⚙️ Output :**
>Z

**💻Example 4:**
```cpp
 #include <iostream>
using namespace std;

int main() {
    char alpha = 'B';
    
    cout<<int(alpha);
    
    return 0;
}
```
**⚙️ Output :**
>66

```cpp

int ascii = 65;
char alpha = ascii;

cout<<char(ascii);
```
How to convert char to ascii

```cpp
char -> ASCII

char alpha = 'A';
int ascii = alpha;

cout<<int(alpha);
```

How to find out length of a string

```cpp
string name = "RTC";

     0  1  2    3
     |  |  |    |
    [R][T][C]['\0']
```

**💻Example 5:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
   string name = "RTC";
   
   cout<<name.length();
   
    return 0;
}
```
**⚙️ Output :**
>3

**💻Example 6:**
```cpp
#include <iostream>
using namespace std;

int main() 
{
    
   string name = "RTC";
   
   int count = 0;
   while(true)
   {
       cout<<name[count];
       count++;
       
       if(name[count]=='\0'){
           break;
       }
   }
   
    return 0;
}
```
**⚙️ Output :**
>RTC

**💻Example 7:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
   string name = "RTC";
   
   int count = 0;
   while(true)
   {
       if(name[count]=='\0'){
           break;
       }
       cout<<name[count];
       count++;
   }
   cout<<"\nLength is: "<<count;
   
    return 0;
}
```
**⚙️ Output :**
>RTC<br>
Length is: 3

How to convert capital letter into small.

```cpp
capital -> small
A -> a
cap ascii + 32 => small
65 + 32 => 97
```

WAP to convert small letter into capital.

```cpp
small -> capital
a -> A
small-ascii - 32 => cap ascii
100 - 32 => 97
```

**💻Example 8:**
```cpp
int main() {
    
    string name;
    cout<<"Enter small name: ";
    cin>>name;
    
    int i=0;
    
    while(name[i]!='\0')
    {
        int curr_char = name[i];
        curr_char = curr_char - 32;
        name[i] = curr_char;
        
        i++;
    }
    
    cout<<"Capital Letter is: "<<name;
    return 0;
}
```
**⚙️ Output :**
>Enter small name: hello<br>
Capital Letter is: HELLO

**💻Example 9:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    string name;
    cout<<"Enter small name: ";
    cin>>name;
    
    int i=0;
    
    while(name[i]!='\0')
    {
        int curr_char = name[i];
        
        if(curr_char>=97 && curr_char<=122)
        {
        curr_char = curr_char - 32;
        }
        name[i] = curr_char;
        
        i++;
    }
    
    cout<<"Capital Letter is: "<<name;
    return 0;
}
```
**⚙️ Output :**
>Enter small name: abcd<br>
Capital Letter is: ABCD

## Total ascii values are 128

**💻Example 10:**
```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i=0; i<=127; i++)
    {
        cout<<i<<" => "<<char(i)<<endl;
    }
    return 0;
}
```
**⚙️ Output :**
>32 =>  <br>
33 => !<br>
34 => "<br>
35 => #<br>
36 => $<br>
37 => %<br>
38 => &<br>
39 => '<br>
40 => (<br>
41 => )<br>
42 => *<br>
43 => +<br>
44 => ,<br>
45 => -<br>
46 => .<br>
47 => /<br>
48 => 0<br>
49 => 1<br>
50 => 2<br>
51 => 3<br>
52 => 4<br>
53 => 5<br>
54 => 6<br>
55 => 7<br>
56 => 8<br>
57 => 9<br>
58 => :<br>
59 => ;<br>
60 => <<br>
61 => =<br>
62 => ><br>
63 => ?<br>
64 => @<br>
65 => A<br>
66 => B<br>
67 => C<br>
68 => D<br>
69 => E<br>
70 => F<br>
71 => G<br>
72 => H<br>
73 => I<br>
74 => J<br>
75 => K<br>
76 => L<br>
77 => M<br>
78 => N<br>
79 => O<br>
80 => P<br>
81 => Q<br>
82 => R<br>
83 => S<br>
84 => T<br>
85 => U<br>
86 => V<br>
87 => W<br>
88 => X<br>
89 => Y<br>
90 => Z<br>
91 => [<br>
92 => \<br>
93 => ]<br>
94 => ^<br>
95 => _<br>
96 => `<br>
97 => a<br>
98 => b<br>
99 => c<br>
100 => d<br>
101 => e<br>
102 => f<br>
103 => g<br>
104 => h<br>
105 => i<br>
106 => j<br>
107 => k<br>
108 => l<br>
109 => m<br>
110 => n<br>
111 => o<br>
112 => p<br>
113 => q<br>
114 => r<br>
115 => s<br>
116 => t<br>
117 => u<br>
118 => v<br>
119 => w<br>
120 => x<br>
121 => y<br>
122 => z<br>
123 => {<br>
124 => |<br>
125 => }<br>
126 => ~<br>
127 => <br>

## 🏠  HomeWork
1️⃣ WAP to convert capital letter into small.

## 🔗 Some Useful Links

## 📖 References