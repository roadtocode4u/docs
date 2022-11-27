<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Sets in Python

## Sets

It Data type which Act like Mathmatical sets.
{ }= Define sets.

## Properties of Sets 
* Unorderd  =

Unordered means that the items in a set do not have a defined order.
```python
MyColor={'Sky','Red','Pink','Yellow','Green'}
print(MyColor)
```

* Unindexed =

we cannot access the elements.

* Unique values 
```python
MyColor={'Sky','Red','Pink','Yellow','Green','Sky','Pink'}
print(MyColor)
```

## Adding values to Sets 

add()=The add() method adds an element to the set.But position is not decide because set are unorderd.
```python
Students={ "Aniket","Avishkar","priyanka"}
print(Students)
Students.add("Prachi")
print(Students)
```
## Remove Elements to Sets 

* remove() = Hard Removal
```python
Students={ "Aniket","Avishkar","priyanka","Vaibhavi","Vaishnavi"}
print(Students)
Students.remove("Vaibhavi")
print(Students)
```

* discard() = Soft Removal
```python
Students={ "Aniket","Avishkar","priyanka","Vaibhavi","Vaishnavi"}
print(Students)
Students.discard("Yash")
print(Students)
```
## Union of Sets 

The union() method returns a set that contains all items from the original set, and all items from the specified set.
```python
StudentsList1={ "Aniket","Avishkar","priyanka","Vaibhavi"}
StudentsList2={"Vaishnavi","Divya","Pranali","Meghana","Vaibhavi"}
AllStudents=StudentsList1.union(StudentsList2)
print(AllStudents)
```

## Intersection of Sets

The intersection() method returns a set that contains the similarity between two or more sets.
```python
StudentsList1={ "Aniket","Avishkar","priyanka","Vaibhavi","Vaishnavi"}
StudentsList2={"Vaishnavi","Divya","Pranali","Meghana","Vaibhavi"}
AllStudents=StudentsList1.intersection(StudentsList2)
print(AllStudents)
```
## Symmetric Differnce

```python
StudentsList1={ "Aniket","Avishkar","priyanka","Vaibhavi","Vaishnavi"}
StudentsList2={"Vaishnavi","Divya","Pranali","Meghana","Vaibhavi"}
OnlyOneClassStudent=StudentsList1.symmetric_difference(StudentsList2)
print(OnlyOneClassStudent)
```
The symmetric_difference() method in Python for two elements StudentsList1 and StudentsList2 is used to return the set of elements contained in both StudentsList1 and StudentsList2 but not common in both of them.

## 🏠 HomeWork
>1️⃣Write a program to use Add(),Remove() function to Sets.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
 #Add() Function
Colour={ "Red","Pink","Yellow"}
print(Colour)
Colour.add("Blue")
print(Colour)  

#Remove() Function
Colour={ "Red","Pink","Yellow"}
print(Colour)
Colour.remove("Pink")
print(Colour) 

  ```

  </p>

</details>

>2️⃣Write a program to use 5 different operation on sets.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python

# union operation(1)
Girls={ "Gita","Radha","Sangita","Priya"}
Boys={"Omkar","Raj","Vaibhav","Sumit","Ganesh","Rohit"}
Class =Girls.union(Boys) 
print(Class)

# intersection operation(2)
Girls={ "Gita","Kiran","Sangita","Priya"}
Boys={"Omkar","Kiran","Vaibhav","Sumit","Ganesh","Rohit"}
Class =Girls.intersection(Boys) 
print(Class) 

# symmetric_difference operation(3)
Girls={ "Gita","Kiran","Sangita","Priya"}
Boys={"Omkar","Kiran","Vaibhav","Sumit","Ganesh","Rohit"}
Class =Girls.symmetric_difference(Boys) 
print(Class)

# Discard operation(4)
Boys={"Omkar","Kiran","Vaibhav","Sumit","Ganesh","Rohit"}
Boys.discard(3)
print(Boys)    

 # add operation(5)
Boys={"Omkar","Kiran","Vaibhav","Sumit","Ganesh","Rohit"}
Boys.add("Rahul")
print(Boys)   
  ```

  </p>

</details>

🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  