<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# While-loop,Practice Questions in Python

## While-loop

```python
while True :
    statements
if stopping condition :
    break
```

**Example:**
>Write a program to Count the Number of Digits Present In a Number.
```python
num=int(input("Enter Any number :"))
count=0
while num>0:
  num=num // 10
  count=count + 1
print("Total Digits =",count)
```
**⚙️ Output:**
>Enter Any number :7121     
Total Digits = 4

**Example:**

>Write a program to Count the Number of Digits if number is 0 .
```python
num=int(input("Enter Any number :"))
count=0
flag=1
while num>=0 and flag==1:
  num=num // 10
  count=count + 1
  if num==0:
   flag=0
print("Total Digits =",count)
```
**⚙️ Output:**
>Enter Any number :0  
Total Digits = 1

**Example:**

>1Write a program to reversed the Present Number.

```python
num=int(input("Enter Any number :"))
rev=0
while num>0:
  rem=num%10
  rev=(rev*10)+rem
  num=num // 10
print("Reversed number is :",rev)
```
**⚙️ Output:**
>Enter Any number :58644   
Reversed number is : 44685

**Example:**

>Write a program to Print the Fibonacci sequence.
```python
n=int(input("How many time do you want to print :"))
f=0
s=1
print(f ," , " , s ,end=(" "))
for i in range(n):
  num=f+s
  f=s
  s=num
  print(" , ",num)
```
**⚙️ Output:**
>How many time do you want to print :5 
0,1,1,2,3,5,8
## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p> 

