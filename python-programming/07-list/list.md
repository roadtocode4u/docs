<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

#  Lists in Python

## Lists 
Lists are used to store multiple items in a single variable.

Example :
```python
Students=['Yash','Vidya','Gauri']
print(Students)
```
```python
Students=['Yash','Vidya','Gauri','Prachi']
print(Students[1])
```
```python
Students=['Yash','Vidya','Gauri','Prachi']
print(Students[0:3])
```
```python
Students=['Yash','Vidya','Gauri','Prachi']
print(Students[-1])
```


## Properties Of List 
1. Ordered


Lists are ordered, it means that the items have a defined order, and that order will not change.

2. Allow Duplicates

Lists can have items with the same value
```python
Fruits = ["apple", "banana", "cherry", "apple", "cherry"]
print(Fruits)
```

3. List can contain Different Data Type

A list can contain different data types
```python
RandomData = ["abc", 34, True, 40, "Hi"]
print(RandomData)
```

4. Changeable 

The list is changeable, that we can change, add, and remove items in a list after it has been created.

* Update =
```python
Courses=['c','c++','Python','Java']
print("Before Changes",Courses)
Courses[1]="C++ Programming"
print("After Changes",Courses)
```

* Insert =
```python
Courses=['c','c++','Python','Java']
print("Before Changes:",Courses)
Courses.insert(1,'Android Development')
print("After Changes:",Courses)
```
* Append =

The append() method appends an element to the end of the list.
```python
Courses=['c','c++','Python','Java']
print("Before Changes:",Courses)
Courses.append('Android Development')
print("After Changes:",Courses)
```
* Remove =

The remove() method removes the specified item.
```python
Fruits = ["apple","banana","orange","grepes"]
Fruits.remove("banana")
print(Fruits)
```

* Pop =

The pop() method takes a single argument (index).
```python
Fruits = ["apple","banana","orange","grepes"]
Fruits.pop(2)
print(Fruits)
```
* Delete =
```python
Fruits = ["apple","banana","orange","grepes"]
del Fruits[1]
print(Fruits)
```

* Clear =

The clear() method removes all the elements from a list.

```python
Fruits = ["apple","banana","orange","grepes"]
Fruits.clear()
print(Fruits)
```

* Sort =

List objects have a sort() method that will sort the list alphanumerically, ascending,descending.

Ascending Order=
```python
alphabets=['A','R','V','S','P']
alphabets.sort()
print(alphabets)
```
Descending Order=
```python
alphabets=['A','R','V','S','P']
alphabets.sort(reverse=True)
print(alphabets)
```

## 🏠 HomeWork

>1️⃣Write a program to implement deletion of items from list using four different methods. 

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
colour=["Red","Pink","Orange","Yellow","Green"]
colour.remove("Pink")
print(colour)       #Remove Method

colour=["Red","Pink","Orange","Yellow","Green"]
colour.pop(3)
print(colour)       #Pop Method

colour=["Red","Pink","Orange","Yellow","Green"]
del colour[1]
print(colour)       #Delete Method

colour=["Red","Pink","Orange","Yellow","Green"]
colour.clear()
print(colour)       #Clear Method
  ```

  </p>

</details>

>2️⃣ Write a program to implement sort the given list in ascending and descending order.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
colour=["Red","Pink","Orange","Yellow","Green"]
colour.sort()
print(colour)       #Ascending order

colour=["Red","Pink","Orange","Yellow","Green"]
colour.sort(reverse=True)
print(colour)       #descending order
  ```

  </p>

</details>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>