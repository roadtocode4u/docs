<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Logical Operators in Python


* If the condition sequence will change , then output will also change.👇👇 Because we have not set any boundary conditions.

**Example :**
```python
marathi,hindi,english,math,science= input("Enter Marks of 5 Subject : ").split()
sum=int(marathi)+int(hindi)+int(english)+int(math)+int(science)
per=(sum/500)*100
print("Percentage :",per,"%")
if per>=60:
  print("Grade D")  
elif per>=70:
  print("Grade C")
elif per>=80:
  print("Grade B")
elif per>=90:
  print("Grade A")
else:
  print("FAIl")
  ```

**⚙️ Output :**
>Enter Marks of 5 Subject : 90 96 97 94 95
>Percentage : 94.399%          
>Grade D


* Give Boundary conditions of the above Program 

**Example :**
```python
marathi,hindi,english,math,science= input("Enter Marks of 5 Subject : ").split()
sum=int(marathi)+int(hindi)+int(english)+int(math)+int(science)
per=(sum/500)*100
print("Percentage :",per,"%")
if per>=60 and per<70:
  print("Grade D")
elif per>=70 and per<80:
  print("Grade C")
elif per>=80 and per<90:
  print("Grade B")
elif per>=90: and per<=100:
  print("Grade A")
else:
  print("FAIl")

```
**⚙️ Output:**
>Enter Marks of 5 Subject : 91 93 93 98 85
>Percentage : 92.0 %   
>Grade A


## Logical Operators 

Logical operators are used to combine conditional statements.

### AND Operator

Result True, if both operand condition are true otherwise false.

**Example :**
```python
# hsc>60 and jee>120
hsc=50
jee=120
result= hsc>60 and jee>120
print(result)

```
**⚙️ Output :**
>False
* 🤔Why is this Output ??

Because , First condition is false and Second Condition is True therefore, result is false.

**Example :**
```python
# hsc>60 and jee>120
hsc=80
jee=50
result= hsc>60 and jee>120
print(result)
```
**⚙️ Output :**
> False
* 🤔Why is this Output ??

Because , First condition is True and Second Condition is False therefore, result is false.

**Example :**
```python
# hsc>60 and jee>120
hsc=5
jee=30
result= hsc>60 and jee>120
print(result)
```
**⚙️ Output :**
>False
* 🤔Why is this Output ??

Because , First condition is False and Second Condition is False therefore, result is false.

**Example :**
```python
# hsc>60 and jee>120
hsc=80
jee=130
result= hsc>60 and jee>120
print(result)
```
**⚙️ Output :**
>True
* 🤔Why is this Output ??

Because , First condition is True and Second Condition is True therefore, result is True.

### OR Operator

Result True if both operand condition are true and one of the condition is true otherwise result False.

**Example :**
```python
# neet>520 or aiims>220
neet=80
aiims=130
result=neet>520 or aiims>220
print(result)
```
**⚙️ Output :**
>False
* 🤔Why is this Output ??

Because , First condition is False and Second Condition is False therefore, result is False.

**Example :**
```python
# neet>520 or aiims>220
neet=530
aiims=130
result=neet>520 or aiims>220
print(result)
```
**⚙️ Output :**
>True 
* 🤔Why is this Output ??

Because ,  First condition is True and Second Condition is False therefore, result is True (one of the condition is true).

**Example :**
```python
# neet>520 or aiims>220
neet=120
aiims=230
result=neet>520 or aiims>220
print(result)
```
**⚙️ Output :**
>True
* 🤔Why is this Output ??

Because , First condition is False and Second Condition is True therefore, result is True (one of the condition is true).

**Example :**
```python
# neet>520 or aiims>220
neet=530
aiims=230
result=neet>520 or aiims>220
print(result)
```
**⚙️ Output :**
>True
* 🤔Why is this Output ??

 First condition is True and Second Condition is True therefore, result is True (both of the condition is true).


## 🧠📝Always Remember

In python don't use logical operator symbol like (&&) (||).

In python you can use Logical operator keywords like "and" "or".

## 🏠 HomeWork
>1️⃣ Write a program Check Number is Divisible by 3 and 5 using "and" operator.
<details>
  <summary>👁 Show Answer</summary>

  <p>
  
```python

number = int(input(" Please Enter any Positive Integer : "))

if((number % 3 == 0) and (number % 5 == 0)):
    print("Given Number {0} is Divisible by 3 and 5".format(number))
else:
    print("Given Number {0} is Not Divisible by 3 and 5 ".format(number))
```
  </p>

</details>

>2️⃣ Write a program to check person does gym or yoga and if one or both of them are doing ,then give healthy habit otherwise not.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
```python
exercise1=input("Enter your Exercise 1 name :")
exercise2=input("Enter your Exercise 2 name :")
if exercise1=="gym" or exercise1=="yoga" or exercise2=="gym" or exercise2=="yoga":
  print("Healthy life")
else :
  print("Not Healthy life")
```
  </p>

</details>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  