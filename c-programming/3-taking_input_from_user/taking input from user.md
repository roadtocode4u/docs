# Taking input from user

## scanf() function:

scanf() is one of the commonly used function to take input from the user, to  read the input data from the console.

 **💻Example :**
```c
#include <stdio.h>

int main() {
    
    int val;
    
    printf("Enter value of val:");
    scanf("%d",&val);
    
    printf("output is %d",val);
 
    return 0;
}
```
**⚙️ Output :**
>Enter value of val:10    
output is 10  

 **💻Example :**
```c
#include <stdio.h>

int main() {
    
     int num1;
     int num2;
     int sum;
     
     printf("Enter Value of num1 :");
     scanf("%d",&num1);
     
     printf("Enter Value of num2 :");
     scanf("%d",&num2);
     
     sum = num1 + num2;
     
     printf("sum:%d",sum);
 
    return 0;
}
```
**⚙️ Output :**
>Enter Value of num1 :10   
Enter Value of num2 :20    
sum:30   

<br>

# Practice Questions C Programming 


## 💻🏆Examples :

**💻Example:**
```c
// Sum of two numbers

#include <stdio.h>

int main() {
    int num1, num2;
    
    printf("Enter value of num1 :");
    scanf("%d",&num1);
    
    printf("Enter value of num1 :");
    scanf("%d",&num2);
    
    int sum = num1 + num2;
    printf("sum of num1 and num2 =%d",sum);
   
    return 0;
}
```
**⚙️ Output :**
>Enter value of num1 :10   
Enter value of num1 :20    
sum of num1 and num2 =30  

**💻Example:**
```c

#include <stdio.h>

int main() {
   int marathi,hindi,english;
   
   printf("Enter marks of Marathi :");
   scanf("%d", &marathi);
   
    printf("Enter marks of Hindi :");
   scanf("%d", &hindi);
   
    printf("Enter marks of English :");
   scanf("%d", &english);
   
   printf("M=%d H=%d E=%d",marathi,hindi,english);
    
    return 0;
}
```
**⚙️ Output :**
>Enter marks of Marathi :95    
Enter marks of Hindi :95   
Enter marks of English :95   
M=95 H=95 E=95


**💻Example:**
```c
#include <stdio.h>

int main() {
   int marathi,hindi,english;
   
   printf("Enter marks of Marathi ,Hindi,and English :");
   scanf("%d%d%d", &marathi,&hindi,&english);
  
   
   printf("M=%d H=%d E=%d",marathi,hindi,english);
    
    return 0;
}
```
**⚙️ Output :**
>Enter marks of Marathi ,Hindi,and English :95 95 95     
M=95 H=95 E=95

**💻Example:**
```c
//Take input from user and print sum and percentage 

#include <stdio.h>

int main() {
   int marathi,hindi,english;
   
   printf("Enter marks of Marathi ,Hindi,and English :");
   scanf("%d%d%d", &marathi,&hindi,&english);
  
   int sum = (marathi + hindi + english );
   
   int per =sum/3;
   char p ='%';
   
   printf("Sum=%d,Percentage=%d %c",sum,per,p);
   
    return 0;
}
```
**⚙️ Output :**
>Enter marks of Marathi ,Hindi,and English :95 95 95    
Sum=285,Percentage=95 %


**💻Example:**
```c
//C program to calculate Simple Interest
#include <stdio.h>

int main() {
    
    float p,r,t,si;
    
    printf("Enter Principle,Rate and Time:");
    scanf("%f%f%f", &p,&r,&t);
    
    si=(p*r*t)/100;
    
    printf("Simple Interest :%f",si);
    printf("\nPayable Amount:%f",p+si);
    
    return 0;
}
```
**⚙️ Output :**
>Enter Principle,Rate and Time:5000 300 2   
Simple Interest :30000.000000   
Payable Amount:35000.000000  

**💻Example:**
```c
//Program to convert temperature from celsius to fahrenheit 
#include <stdio.h>

int main() {
   
   float f,c;
   
   printf("Enter Temperature in Celsius :");
   scanf("%f",&c);
   
   f=1.8*c+32;
   
   printf(" Temperature in Fahrenheit =%f",f);
    
    return 0;
}
```
**⚙️ Output :**
>Enter Temperature in Celsius :36   
Temperature in Fahrenheit =96.800003


## 🏠Homework 

>1️⃣ Write a program to take input of 5 subject from user and print sum and percentage.

>2️⃣ Write a program to calculate bill when rate and quantity is give from user.

>3️⃣ Write a program to calculate perimeter and area of a circle when radius is given.

>4️⃣ Write a program to convert km to m and cm.

>5️⃣Write a program to calculate area and perimeter of rectangle when length and breadth is given.

<br>

