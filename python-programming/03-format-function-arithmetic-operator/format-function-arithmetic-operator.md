<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Format Function, Arithmetic Operators in Python

## End Variable In python

```python
print("Good Evening",end="\n")
print("Hello Everyone")
```
```python
print("Good Evening",end=" ")
print("Hello Everyone")
```
## What is the format () function in Python?
The Python format () function formats strings according to the position. 

Example=

```python
x="Vedika"
y=21
dob= "01/01/2001"
print("Hello {} .Your Age is {} .Your DOB is {}". format(x,y,dob))
```

```python
x="Vedika"
y=21
dob= "01/01/2001"
print("Hello {place1} .Your Age is {place2} .Your DOB is {place3}". format(place3=dob,place2=y,place1=x))
```

## Types of operators in Python
<br>

## Arithmetic Operators=
1. Addition Operator (+)

```python
a=10
b=20
c=a+b
print(c)
```
2. Subtraction Operator (-)

```python
a=10
b=20
c=a-b
print(c)
```
3. Multiplication Operator (*)

```python
a=10
b=20
c=a*b
print(c)
```
4. Division Operator (/)

```python
a=10
b=20
c=a/b
print(c)
```
5. Modulus Operator (%)

```python
a=10
b=20
c=a%b
print(c)
```
6. Exponentiation Operator (**)

```python
a=10
b=20
c=a**b
print(c)
```
7. Floor Operator (//)

```python
a=10
b=20
c=a//b
print(c)
```
## 🏠 HomeWork

>1️⃣Write a program to print student information and use format function to inject variable.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
a= "vedika"
b=19
c=2003
d=55

print("Hello {} .your Age is {} .your DOB is {}. and your Roll Number is {}".format(a, b, c, d))
  ```

  </p>

</details>

>2️⃣Write a program to implement an arithmetic operators.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
a=113
b=11
print("Addition(±)        :-",a+b)
print("Subtraction(-)     :-",a-b)
print("Mulitiplication(*) :-",a*b)
print("Division(\)        :-",a/b)
print('modules(**)        :-',a**b) 
print('Exponential(%)     :-',a%b)
print('Floor Division(//) :-',a//b)
  ```

  </p>

</details>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>