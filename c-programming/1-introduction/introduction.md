# Introduction to C Programming

## 🤔What is Programming ?

Programming is the process of instructions that tell a computer how to perform a task.


## Different Programming Languages 💻
```c
C,C++,Java,Python,Kotlin,Javascript,Ruby,Typescript,C#, ...
```

## What is C Programming?

C is a general-purpose programming language.C prograamming created by **Dennis Ritchie** at the **Bell Laboratories** in **1972**.

**💻 Example 1 :**
```c
#include <stdio.h>

int main() 
{

    printf("Hello world");
    
    return 0;
}
```
**⚙️ Output :**
>Hello world

## Program Explanation:

**Line 1:** `#include <stdio.h>` is a header file. The header file `<stdio.h>` stands for **Standard Input Output**.
`#include <stdio.h>`support input output file like  printf() and scanf().**Printf( )** Means Print output on screen **scanf()** Give input from user.

**Line 2:** `int` means Return type of your Function. `main()` it is the first function of every C program that is responsible for starting the execution and termination of the program.

**Line 3:** `{` is used to Start of the function.

**Line 4:** `printf("Hello world");` `printf()` is a function used to output print text to the screen. In our example it will output "Hello World". **`;`** semicolon used to terminate any statement.

**Line 5:** `return 0;` return 0 means that the program will execute successfully.

**Line 6:** `}` closing curly bracket is used to end the main function.




**💻 Example 2 :**
```c

#include <stdio.h>

int main()
{
  
    printf("Hye");
    printf("How Are You ?");
    
    return 0;
}
```
**⚙️ Output :**
>HyeHow Are You ?

## New Line Charachter

`\n` is used to New line Character.

**Example 3 :**
```c
#include <stdio.h>

int main() {
  
    printf("Good Morning !\n");
    printf("Good afternoon !");
    
    return 0;
}

```

**⚙️ Output :**
>Good Morning !     
Good afternoon !