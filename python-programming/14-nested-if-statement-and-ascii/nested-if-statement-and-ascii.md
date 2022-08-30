<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Nested if-Statement And ASCII  in Python

## Nested if

A nested if is a flow control statement that’s the target of another if-statement. By nested-if statements, we mean to use an if-statement inside another if-statement.

**Syntax:**
 ```python
if condition-1:
if condition-2:
   if condition-n:
     statement-1
     statement-2


     statement-n
```

**Example:**
```python
jee=150
hsc=80
if hsc>60:
  print("congrats You cleared HSC")
  if jee>120:
    print("Admission Granted")
  else:
    print("Sorry.You did not cleared JEE")
else:
  print("sorry you need to improved your HSC Score")
```

⚙️ Output:
>congrats You cleared HSC   
Admission Granted

**Example:**
>Write a program to Find the Largest Number Among Three Numbers by using if,elif statement.
```python
a=int(input("Enter a :"))
b=int(input("Enter b :"))
c=int(input("Enter c :"))

if a>b and a>c :
  print("a is largest ")
elif b>a and b>c :
  print("b is largest")
else :
  print("c is largest")
```
⚙️ Output:
>Enter a :10   
Enter b :20   
Enter c :30  
c is largest

**Example:**
>Write a program to Find the Largest Number Among Three Numbers by using Nested-if statement.
```python
a=int(input("Enter a :"))
b=int(input("Enter b :"))
c=int(input("Enter c :"))

if a>b:
  if a>c:
    print("a is largest ")
  else:
    print("c is largest")
else:
  if b>c:
    print("b is largest ")
  else:
    print("c is largest 21")
```
⚙️ Output:
>Enter a :300     
Enter b :200        
Enter c :100     
a is largest 

## ASCII 

ASCII stands for American Standard Code For Information Interchange.

The ascii() function returns a readable version of any object (Strings, Tuples, Lists, etc).

## 🏠 HomeWork

>1️⃣ Write a program to Find the Largest Number Among Three Numbers by using Nested-if statement.
<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
  a=int(input("Enter a :"))
b=int(input("Enter b :"))
c=int(input("Enter c :"))

if a>b:
  if a>c:
    print("a is largest ")
  else:
    print("c is largest")
else:
  if b>c:
    print("b is largest ")
  else:
    print("c is largest 21")
  ```

  </p>

</details>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  