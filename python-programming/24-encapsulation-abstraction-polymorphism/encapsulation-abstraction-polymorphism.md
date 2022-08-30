<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Encapsulation, Abstraction and Polymorphism in Python

**Example :**
```python
class RBI:
  def SanctionLoan(self):
    print("Loan Sanction")

  def credit(self):
    print("Amount Creadited")

  def debit(self):
    print("Amount Debited")
  
class SBI(RBI):
  def openAccount(self):
    print("Account is Created")

obj=SBI()
obj.openAccount()
obj.SanctionLoan()
obj.credit()
obj.debit()
```

**⚙️ Output:**
>Account is Created    
Loan Sanction   
Amount Creadited    
Amount Debited 

**Example :**

```python
class Helper:
  def cal_si(self,p,r,t):
    si= (p*r*t)/100
    print(si)

  def cal_area(self,l,b):
    area=l*b
    print(area)

class Bank(Helper):
  def sanction_loan(self):
    print("Loan Sanctioned")

obj=Bank()
obj.sanction_loan()
obj.cal_area(10,20)
obj.cal_si(5000,3,2)
```
**⚙️ Output:**
>Loan Sanctioned   
200   
300.0   

**Encapsulation :**
 
 Binding similar data and its functionality.

**Abstraction :**

 Show the necessary things and hiding unnecessary information from the user.

 **Polymorphism :**

 Polymorphism in python defines methods in the child class that have the same name as the methods in the parent class.


**Example :**
```python
class Cat:
  def speak (self):
     print("Meowwww! #$%$@%^@$^")

class Dog:
  def speak (self):
     print("bhooooooooo!")

cat = Cat()
cat.speak()

dog = Dog()
dog.speak()
```
**⚙️ Output:**
>Meowwww! #$%$@%^@$^         
bhooooooooo!  

**Example :**
```python
class Department:
  def showDepartment (self): 
    print("This is default department")
    
  def showLeader (self):
     print("I am leader")

class CSE (Department):
  def showDepartment (self):
    print("CSE Department") 
    
  def showLeader (self):
    print("Department Leader is Avishkar")

obj= CSE () 
obj.showDepartment ()
obj.showLeader()
```
**⚙️ Output:**
>CSE Department    
Department Leader is Avishkar

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p> 