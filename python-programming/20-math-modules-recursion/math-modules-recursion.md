<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Math Modules , Recursion in Python

## math.ceil() Method

Round a number upward to its nearest integer.

**Example :**
```python
import math 
num=19.5
newNumber=math.ceil(num)
print(newNumber)
```
**⚙️ Output:**
>20

## math.floor() Method

Round numbers down to the nearest integer.

**Example :**
```python
import math 
num=19.1
newNumber=math.floor(num)
print(newNumber)
```
**⚙️ Output:**
>19

## math.sqrt() Method

Find the square root of different numbers.

**Example :**
```python
import math
num=int(input("Enter number :"))
ans=math.sqrt(num)
print(ans)
```
**⚙️ Output:**
>Enter number :25   
5.0 

## math.pi Constant

Print the value of PI.

**Example :**
```python
import math
print(math.pi)
```
**⚙️ Output:**
>3.141592653589793

## Datetime

A date in Python is not a data type of its own, but we can import a module named datetime to work with dates as date objects.

**Example :**
```python
import datetime
currentDate = datetime.datetime.now()
print(currentDate)
print("Year",currentDate.year)
print("Month",currentDate.month)
print("Day",currentDate.day)
```
**⚙️ Output:**
>2022-03-31 15:49:47.362068    
Year 2022    
Month 3    
Day 31

## strftime 

**Example :**
```python
import datetime
print("Dayname",currentDate.strftime("%A"))
```
**⚙️ Output:**
>Dayname Thursday

## Recursion

Recursion is a common mathematical and programming concept. It means that a function calls itself. This has the benefit of meaning that you can loop through data to reach a result.

**Example :**
```python
def counter(n):
  print(n)
  if n==0:
    return
  else:
    counter(n-1)
counter(5)
```
**⚙️ Output:**
>5    
4   
3   
2        
1   
0   

**Example :**
```python
# Factorial of a number using recursion
def fact(num):
  if num==1:
    return 1
  else:
    return num*fact(num-1)

fact(4)
```
**⚙️ Output:**
>24

## 🏠 HomeWork
>1️⃣ Write a program to give greeting by using Datetime and strftime library python.

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  