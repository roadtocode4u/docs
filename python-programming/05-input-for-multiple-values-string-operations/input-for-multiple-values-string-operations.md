<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Input for Multiple values And String Operations in Python

## IMP Point
  By Default data type of input function is String.

  ## Spilt Function 
  The split() method splits a string into a list.
  ```python
  sentence="My Name is vedika".split()
print(sentence)
  ```
  ```python
  a,b=input("Enter two values").split()
print("a= ",a)
print("b= ",b)
```
```python
rate,quantity=input("Enter rate and quantity").split()
bill=int(rate)*int(quantity)
print("bill :",bill)
```
```python
c=float(input("Enter tempreture in celsius :"))
f=c*(9/5)+32
print("Temperature in Fahrenheit =",f)
```

## Multiline String
You can have a string split across multiple lines by enclosing it in triple quotes

```python
poem="""
Twinkle, twinkle, little star,
How I wonder what you are.
Up above the world so high,
Like a diamond in the sky.
Twinkle, twinkle, little star,
How I wonder what you are!"""
print(poem)
```

## Slicing

A slice object is used to specify how to slice a sequence. You can specify where to start the slicing, and where to end.

```python
mystring="Road to Code"
print(mystring[0:4])
```
```python
mystring="Road to Code"
print(mystring[1:])
```
```python
mystring="Road to Code"
print(mystring[:8])
```
## Length Function

len() is a built-in function in python. You can use the len() to get the length of the given string, array, list.

```python
studentname="vedika"
print(len(studentname))
```
```python
studentname="vedika"
length=len(studentname)
print(length)
```

## in operator

The 'in' operator is used to check if a value exists in a sequence or not.

```python
mystring="Road to Code"
print("Road" in mystring)
```
```python
mystring="Dahi Puri"
print("Pani" in mystring)
```


## 🏠 HomeWork

>1️⃣Write a Python program to find area of a rectangle.

💡 HINT: use formula `area` = `length` * `breadth` .

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
a,b = input("Enter a length*breadth").split()
C =int(a)*int(b)
print("Area of rectangle =",C)
  ```

  </p>

</details>


## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>