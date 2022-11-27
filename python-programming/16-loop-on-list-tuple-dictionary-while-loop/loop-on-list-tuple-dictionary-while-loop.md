<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Loops On List,Tuples, Dictionary And While Loop in Python

## Python - else in Loop

Python allows the else keyword to be used with the for loop too.

**💻Example:**

```python
for i in range(5):
  print(i)
else:
  print("Loop executed successfully ")
```
**⚙️ Output:**
>0     
1    
2     
3    
4    
Loop executed successfully 


**💻Example:**
```python
for i in range(5):
  if i==2:
    continue
  print(i)
else:
  print("Loop executed successfully ")
```
**⚙️ Output:**
>0     
1     
3    
4    
Loop executed successfully 

**💻Example:**
```python
for i in range(5):
  if i==2:
    break
  print(i)
else:
  print("Loop executed successfully ")
```
**⚙️ Output:**
>0    
1

## Iterating through List using for-loop

**💻Example:**
```python
students=["Anuprita","Shraddha","Chaitrali","Prajkta"]
for student in students:
  print("Sending mail to ..",student)
```
**⚙️ Output:**
>Sending mail to .. Anuprita  
Sending mail to .. Shraddha   
Sending mail to .. Chaitrali   
Sending mail to .. Prajkta

**💻Example:**

Sum of List 
```python
marks=[90,80,70,56,78]
sum=0
for mark in marks:
  sum=sum+mark
print(sum)
```
**⚙️ Output:**
>374

## Iterating through tuple using for-loop

**💻Example:**
```python
tuple1=(10,20,30,40,50)
for tup in tuple1:
   print(tup)
```
**⚙️ Output:**
>10   
20    
30   
40   
50

## Iterating through Dictionaries using for-loop

**Iterates through the keys**

**💻Example:**

```python
progress={
    "vedika":90,
    "Aniket":91,
    "Pranali":93,
    "prajkta":94
}

for i in progress.keys():
  print(i)
```
**⚙️ Output:**
>vedika   
Aniket    
Pranali    
prajkta

**Iterates through the values**

**💻Example:**
```python
progress={
    "vedika":90,
    "Aniket":91,
    "Pranali":93,
    "prajkta":94
}

for i in progress.values():
  print(i)
```
**⚙️ Output:**
>90   
91   
93   
94

**Iterates through the keys and values**

**💻Example:**
```python
progress={
    "vedika":90,
    "Aniket":91,
    "Pranali":93,
    "prajkta":94
}

for k,v in progress.items():
  print(k,"scored",v,"marks")
```
**⚙️ Output:**
>vedika scored 90 marks  
Aniket scored 91 marks   
Pranali scored 93 marks  
prajkta scored 94 marks

**💻Example:**
```python
FoodItems={
    "vedika":"🍕",
    "Aniket":"🥭",
    "Pranali":"🍍",
    "prajkta":"🍔"
}

for name,food in FoodItems.items():
  print(name,"likes",food)
```
**⚙️ Output:**
>vedika likes 🍕    
Aniket likes 🥭    
Pranali likes 🍍   
prajkta likes 🍔

## While Loop 

While loop is called as Entry control Loop. The while loop in Python is used to iterate over a block of code as long as the test expression (condition) is true.

**Syntax :**

```python
while test_expression:
    Body of while
```
**💻Example:**
```python
i=0
while i<5:
  print(i)
  i=i+1
```
**⚙️ Output:**
>0       
1    
2    
3    
4

## 🏠 HomeWork

>1️⃣ Write a program to print Grocery Items using keys and values.
<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
GroceryItems={
    "Sugar":50,
    "Cakes":40,
    "Sauces":50,
    "Rice":80
}

for name,price in GroceryItems.items():
  print(name,"price is",price)
  ```

  </p>

</details>

>2️⃣Write a program How to ask a user "Do you want continue ??" in python using while loop.
<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
  while input("Do You Want To Continue? [yes/no]") == "y":
    print("doing something")
  ```

  </p>

</details>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  