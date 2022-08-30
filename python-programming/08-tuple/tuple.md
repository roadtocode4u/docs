<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Tuple in Python

## Tuple
Tuple are used to store multiple values in a single variable.

## Properties Of Tuple

* Ordered =

Tuples are an ordered sequences of items, just like lists.

* Unchangeable =

Tuples are unchangeable, meaning that we cannot change, add or remove items after the tuple has been created.

* Allow Duplicates =

tuples are indexed, they can have items with the same value.

## Manipulation of Tuple Example 

```python
MyBasket=('Apple','Banana','Grapes','Oranges')
ListMyBasket=list(MyBasket)
ListMyBasket[0]='Cherry'
MyBasket=tuple(ListMyBasket)
print(MyBasket)
```

## Index Position

```python
PythonStudent=('Neha','Gauri','Vaibhavi','Meghana')
print(PythonStudent.index("Neha"))
```

## Count()

The count() method returns the number of times the specified element appears in the list.
```python
PythonStudent=('Neha','Gauri','Vaibhavi','Gauri','Meghana','Gauri')
print(PythonStudent.count("Gauri"))
```

## Concatenation of String

To concatenate, or combine, two strings you can use the + operator.
```python
a = "Hello"
b = "World"
c = a + b
print(c)
```
## 🏠 HomeWork
> 1️⃣Write a program to change value touple to using extra overhead work.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
Colour=('Red','Blue','pink','Orange','Yellow')
ListColour=list(Colour)
ListColour[0]='Green'
Colour=tuple(ListColour)
print(Colour)    #change value of tuple
  ```

  </p>

</details>

>2️⃣ Write a program to use function index,count and also perform concatenation of two tuple.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
#Index Function
Colour=('Red','Blue','pink','Orange','Yellow')
print(Colour.index("pink"))  

#Count Function
Colour=('Red','Blue','pink','Orange','Yellow')
print(Colour.count("Yellow"))  

 #Concatenation of String
Name= "Mahatma"
Surname="  Gandhi" 
Full_Name = Name + Surname
print(Full_Name)    
  ```

  </p>

</details>

 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>