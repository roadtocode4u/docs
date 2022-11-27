<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Getter and Setter, Four Pillars Methods in Python

## Getter

Getter Method is use to provide a data.

## Setter 

Setter Method is use to set or manipulate data.


**Example :**
```python
class Student:
  name=''
  roll_no=''
  def SetName(self,name):
    self.name=name
  def SetRollno(self,roll_no):
    self.roll_no=roll_no
  def SetStudent(self,name,roll_no):
    self.name=name
    self.roll_no=roll_no
  
  def GetName(self):
    return self.name
  def GetRollno(self):
    return self.roll_no
  def GetStudent(self):
    print("Name :",self.name)
    print("Roll No :",self.roll_no)
  
avishkar=Student()
avishkar.SetStudent("Avishkar","123")
avishkar.GetStudent()
```

**⚙️ Output:**
>Name : Avishkar   
Roll No : 123

## Four Pillars

Encapsulation. 
Abstraction.        
Polymorphism.    
Inheritance.

**Encapsulation :**
 
 Binding similar data and its functionality.

**Abstraction :**

 Show the necessary things and hiding unnecessary information from the user.

 **Polymorphism :**

 Polymorphism in python defines methods in the child class that have the same name as the methods in the parent class.

 **Inheritance :**

 Inheritance  a class that inherits all the methods and properties from another class.
## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  