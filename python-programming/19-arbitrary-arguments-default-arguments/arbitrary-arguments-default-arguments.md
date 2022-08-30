<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Arbitrary Arguments, Default Arguments in Python

>  Write a program to find simple interest using function all cases .

💡 HINT : Simple Interest = (P x T x R)/100  
           Where,    
              P is the principle amount    
              T is the time and   
              R is the rate  
 
👉Answer Of this program based on following 4 ways:

**1. No Arguments And No Return:**

**Program:**
```python
def cal_si():
  p=int(input("Enter Principle :"))
  r=int(input("Enter Rate :"))
  t=int(input("Enter Time :"))
  si=p*r*t/100
  print(si)
cal_si()
```
**⚙️ Output:**
>Enter Principle :5000    
Enter Rate :3   
Enter Time :2   
300.0

**2. Arguments but No Return:**

**Program:**
```python
def cal_si(p,r,t):
  si=p*r*t/100
  print(si)
p=int(input("Enter Principle :"))
r=int(input("Enter Rate :"))
3
t=int(input("Enter Time :"))
cal_si(p,r,t)
```

**⚙️ Output:**
>Enter Principle :5000   
Enter Rate :3   
Enter Time :2   
300.0  

**3. No Arguments but Return:**

**Program:**
```python
def cal_si():
  p=int(input("Enter Principle :"))
  r=int(input("Enter Rate :"))
  t=int(input("Enter Time :"))
  si=p*r*t/100
  print(si)

ans=cal_si()
print(ans)
```
**⚙️ Output:**
>Enter Principle :5000   
Enter Rate :3   
Enter Time :2   
300.0  

**4. Arguments And Return:**

**Program:**
```python
def cal_si(p,r,t):
  si=p*r*t/100
  return si
p=int(input("Enter Principle :"))
r=int(input("Enter Rate :"))
t=int(input("Enter Time :"))

ans=cal_si(p,r,t)
print(ans)
```

**⚙️ Output:**
>Enter Principle :5000   
Enter Rate :3   
Enter Time :2   
300.0 

## Arbitrary Arguments :

Especially useful when we are not sure in the advance that how many arguments, the function would require.

We define the arbitrary arguments while defining a function using the asterisk (*) sign.

**Program:**
```python
def greeting (* students):
  print(students[0])
  print(students[1])
  print(students[2])
greeting("Gauri","Vidya","Vaibhavi")
```

**⚙️ Output:**
>Gauri  
Vidya  
Vaibhavi

**Program:**
```python
def greeting (* students):
  for i in students:
    print("Hello",i)
greeting("Gauri","Vidya","Vaibhavi")
```
**⚙️ Output:**
>Hello Gauri   
Hello Vidya   
Hello Vaibhavi  

## Default Arguments :

**Program:**
```python
def greeting(name="Yash"):
  print("Hello",name)
greeting()
```
**⚙️ Output:**
>Hello Yash

**Program:**
```python
def fruits(fruits1,fruits2="R"):
  print(fruits1)
  print(fruits2)
fruits("A")
```

**⚙️ Output:**
>A    
R

## Types of Function 
1. Inbuilt
2. User Define

## 🔗 Some Useful Links

## 📖 References


<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>