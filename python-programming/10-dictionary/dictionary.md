<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# Dictionary in Python

## Dictionary

Dictionaries are used to store data values in key:value pairs.
```python
syntax = dictionary_name={
    key1:value1,
    key2:value2,
    key3:value3
}
```

```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
print(phonebook["Prachi"])
```
```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
print(phonebook.get("Pranali"))
```
```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
name=input("Enter Name to find mobile no: ")
mobile=phonebook.get(name)
print("Mobile Number :",mobile)
```
```python
FruitNameToImage={
    "apple":"🍎",
    "banana":"🍌",
    "cherry":"🍒",
    "grapes":"🍇",
    "orange":"🍊"
}
fruitkey=input("Enter fruit name :")
Image=FruitNameToImage.get(fruitkey)
print("{} looks like {} " .format(fruitkey,Image))
```
```python
courses={
    "c":"299",
    "c++":"299",
    "python":"499",
    "web":"999",
    "java":"499"
}
print(courses.keys())
```
```python
courses={
    "c":"299",
    "c++":"299",
    "python":"499",
    "web":"999",
    "java":"499"
}
print(courses.values())
```
### Adding New Key =
```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
print(phonebook)
phonebook["Anjali"]=8745478798
print(phonebook)
```
### Update Key =
```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
print(phonebook)
phonebook["Pranali"]="2367632673"
print(phonebook)
```
### Remove key =
```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
print(phonebook)
phonebook.pop("Pranali")
print(phonebook)
```
### Clear Dictionary =
```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
print(phonebook)
phonebook.clear()
print(phonebook)
```
## 🏠 HomeWork
>1️⃣Write a program to create a phonebook  dictionary and use lowercase function to convert all keys in lowercase.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
phonebook={
    "Harshada":"8578571958",
    "Prachi":"9093238098",
    "Pranali":"9855893498",
    "Prajkta":"4789848908",
    "Vaishnavi":"4879448987",
}
name = input("Enter name to find number :").lower()
mobile = phonebook.get(name)
print("Name : {} \n mobile : {} :".format(name,mobile))

  ```

  </p>

>2️⃣Write a program to create a fruits dictionary and its meaning.

<details>
  <summary>👁 Show Answer</summary>

  <p>
  
  ```python
FruitNameToImage={
    "apple":"🍎",
    "banana":"🍌",
    "cherry":"🍒",
    "grapes":"🍇",
    "orange":"🍊"
}
fruitkey=input("Enter fruit name :")
Image=FruitNameToImage.get(fruitkey)
print("{} looks like {} " .format(fruitkey,Image))

  ```

  </p>

## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  