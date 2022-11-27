<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# If, Elif in Python

## Comparison/Relational Operators

Comparison operators are to test the condition. The conditional operator result as boolean True or False.

 #### equals to (==)

This operator returns True if both the operands are equal.if both the left and the right operand are equal to each other.
```python
a=10
b=10
result= a==b
print(result)
```

⚙️ Output:
>True  

#### less than ( < )

This operator returns True if the left operand is less than the right operand.

```python
a=10
b=20
result= a<b
print(result)
```

⚙️ Output:
>True  

#### greater than ( > )

This operator returns True if the left operand is greater than the right operand.
```python 
a=30
b=20
result= a>b
print(result)
```

⚙️ Output:
>True  

#### less than or equal to ( <= )

This operator returns True if the left operand is less than or equal to the right operand.
```python
a=10
b=20
result= a<=b
print(result)
```

⚙️ Output:
>True  

#### greater than or equal to ( >= )

This operator returns True if the left operand is greater than or equal to the right operand.
```python
a=50
b=20
result= a>=b
print(result)
```

⚙️ Output:
>True

#### not equal to (!=)

This operator returns True if both the operands are not equal.
```python
a=50
b=20
result= a!=b
print(result)
```

⚙️ Output:
>True

```python
a=20
b=20
result= a!=b
print(result)
```

⚙️ Output:
>False

## Indentation

Python relies on indentation (whitespace at the beginning of a line) to define scope in the code. Other programming languages often use curly-brackets for this purpose.

## Conditional Statements

#### if Statement
**Syntax:**
 ```python
 if condition :
     statements-1
     statements-2
     .....
     .....
     statements-n
```

**Example:**
```python
a=20
b=20
if a==b:
  print("A is Equals to B ")
```

⚙️ Output:
>A is Equals to B

#### if--else Statements
**Syntax:**
```python
if condition :
     statements-1
     statements-2
     .....
     .....
     statements-n
else:
    statements-1
     statements-2
     .....
     .....
     statements-n
```

**Example:**
```python
a=20
b=30
if a==b:
  print("A is Equals to B ")
else :
   print("B is Unequals to A ")
```
 ⚙️ Output:
 >B is Unequals to A

```python
a=50
b=30
if a>b:
  print("A is greater than B")
else :
  print("B is greater than to A ")
```
⚙️ Output:
>A is greater than B

#### 💡Difference between = and == operators in Python

The “ = ” is an assignment operator is used to assign the value on the right to the variable on the left. 

The ‘==’ operator checks whether the two given operands are equal or not.

## 🏠 HomeWork

>1️⃣ Write a program to check whether applicant is eligible for voting or not using if statement.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
  age=int(input("Enter Your age :"))
  if age>=18:
    print("You are eligible for Voting")
  else:
    print("You are not eligible for Voting")
  ```

  </p>
</details>

>2️⃣ Write a program to check whether entered number is even ir odd by using if-else statements.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
  num=int(input("Enter Number :"))
  rem=num%2
  if rem==0:
    print("Given Number is Even")
  else:
    print("Given Number is Odd")
  ```

  </p>

</details>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  