<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Variables & Data Type in Python

## What is Variable
Variables are used to store data, they take memory space based on the type of value we assigning to them.<br><br>
 Example =

 ```python
 Name="Vedika"
 print(Name)
 ```
 Here,We are storing vedika in the variable name.

## Rules to declare a variable in python

1. A variable name must start with a letter (a-z or A-Z) or the underscore (_) character.
2. A variable name cannot start with a number.
3. variable are case-sensitive
4. A variable name can not used reserved keyword
5. A variable name can include (a-z,A-z, 0-9, and _ )

## Code Blocks

```python
age=21
print(age)
```
```python
name="Vedika"
age=20
weight=50.50

print("Name: ",name)
print("Age: ",age)
print("Weight: ",weight)
```
```python
name="Vedika"
age=20
weight=50.50

print(type(name))
print(type(age))
print(type(weight))
```
```python
a,b,c=10,20,30
print(a)
print(b)
print(c)
```
```python
val=10
print(val)
val=20
print(val)
val=30
val=40
val=50
print(val)
```

## 🏠 HomeWork

>1️⃣ Write a program to declare variables and then store your own information in the variable and print in a formatted way.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
Name='Vedika'
Age=18
Weight=50
Clg_name="GP"
Email_id="PQR123@gmail.com"
Studied_at="Pune"
print("Name:",Name)
print("Age:",Age)
print("Weight:",Weight)
print("Email_id",Email_id)
print("Studied_at",Clg_name)
  ```

  </p>

</details>

> 2️⃣ Write a program to find data type of three different variable.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
a="Vedika"
b=10000
c=10.222
print("type of a:",type(a))
print("type of b:",type(b))
print("type of c:",type(c))
  ```

  </p>

</details>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>