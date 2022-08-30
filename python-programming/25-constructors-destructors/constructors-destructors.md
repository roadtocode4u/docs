<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Constructors and Destructors in Python

## Constructor :

Constructor invokes automatically at the time of object creation.

**Syntax :**
```python
def __init__ (self):
```

**💻Example :**
```python
class Student:
  first_name=''
  roll_no=''
  def setFirstName(self,First_Name):
    self.First_Name=First_Name
  def setRollNo(self,Roll_No):
    self.Roll_No=Roll_No
  def getFirstName(self):
    print(self.First_Name)
  def getRollNo(self):
    print(self.Roll_No)

obj=Student()
obj.setFirstName("suraj")
obj.setRollNo(123)

obj.getFirstName()
obj.getRollNo()
```

**⚙️ Output:**
>suraj    
123

**💻Example :**
```python
class sample:
  def __init__(self):
    print("constructor called")
  def showsample(self):
    print("This is sample")

obj=sample()
obj
```
**⚙️ Output:**
>constructor called     
This is sample


**💻Example :**
```python
class sample:
  def showsample(self,param):
    print("This is sample",param)

  def __init__(self):
    print("constructor called")

obj=sample()
obj.showsample("code")
```
**⚙️ Output:**
>constructor called   
This is sample code

## Destructor :

Destructor invokes when object goes out of scope .

**Syntax :**

```python
def __del__(self):
```
**💻 Example :**
```python
class Sample:
  def __init__(self):
    print("Constuctor called")
  def fun(self):
    print("Fun called")
  def __del__(self):
    print("Destructor called")

obj=Sample()
obj.fun()
```
**⚙️ Output:**
>Constuctor called    
Fun called

**💻 Example :**
```python
class Student:
  first_name=''
  roll_no=''

  def __init__(self, first_name, roll_no):
    self.first_name= first_name
    self.roll_no = roll_no

  def getFirstName(self):
     print(self.first_name)

  def getRollNo(self):
     print(self.roll_no)

objects = []
objects.append(Student("Suraj", 123)) 
objects.append(Student("Aniket", 456))
objects.append(Student("Aniket", 456))
objects.append(Student("Meghana", 789))

for obj in objects:
  print("Student Details:")
  obj.getFirstName()
  obj.getRollNo()
```
**⚙️ Output:**
>  Student Details:   
Suraj   
123   
 Student Details:   
Aniket   
456   
 Student Details:   
Aniket    
456  
 Student Details:   
Meghana   
789   
## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p> 