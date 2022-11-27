<!-- HEADER -->
<p align="center">
  <img  src="./../assets/header.png?" />
</p>

# If else Ladder in Python

> 🚁Write a program which asks user to enter rate and quantity of a product. Your program should calculate and display the the bill amount as rate * quantity. If bill amount is more than 500 discount of 20% on bill and less than 500 then discount of 5% on bill.

```python
Program 1 =

rate,quantity=input("Enter rate And quantity :").split()
bill=int(rate)*int(quantity)
if bill>500:
  print("### 20% Off ###")
  print("Actual Bill:",bill)
  discount=(bill/100)*20
  print("discount:",discount)
  print("payble amount :", bill - discount)
else :
  print("### 5% Off ###")
  print("Actual Bill:",bill)
  discount=(bill/100)*20
  print("discount:",discount)
  print("payble amount :" ,bill - discount)

  program 2 =

rate,quantity=input("Enter rate And quantity :").split()
bill=int(rate) * int(quantity)
disc_per=0

if bill>500:
  disc_per=20
else :
  disc_per=5

discount=(bill/100)*disc_per
payble_amount=bill-discount
print("### {} ### ".format(disc_per))
print("Bill Amount :",bill)
print("Discount :",discount)
print("Payble Amount :",payble_amount)
```

## If Else Ladder

Python elif is used to execute a continuous chain of conditional logic ladder. In elif, there are multiple conditions and the corresponding statements as a ladder.

```python
syntax=

if condition-1:
  statements-1
  statements-2
elif condition-2:
  statements-1
  statements-2
elif condition-3:
  statements-1
  statements-2
elif condition-4:
  statements-1
  statements-
else:
  statements-1
  statements-2
```

```python
Example-1 =

num=int(input("Enter number from 1-5 :"))
if num==1:
  print("You Selected Option 1")
elif num==2:
  print("You Selected Option 2")
elif num==3:
 print("You Selected Option 3")
elif num==4:
 print("You Selected Option 4")
elif num==5:
 print("You Selected Option 5")
else:
 print("You Selected wrong input")

 Example-2 =

 name=input("Enter fruit or vegetable name :") 
if name=="onion":
  print("🧅")
elif name=="apple":
  print("🍎")
elif name=="banana":
  print("🍌")
elif name=="pineapple":
  print("🍍")
else:
  print("Not available")
```

## 🏠 HomeWork
>1️⃣ Write a program to take input for marks of 5 subject and display the grade.

💡 HINT : Per=(total/500)*100

* If the percentage  greater than 90 “Grade: A” is printed.
* If the percentage  greater than 80 “Grade: B” is printed.
* If the percentage  greater than 70 “Grade: C” is printed.
* If the percentage  greater than 60 “Grade: D” is printed.
* otherwise , Fail is Printed.

<details>
  <summary>👁 Show Answer</summary>

  <p>

  📝 Code:

  ```python
  marathi,hindi,english,math,science= input("Enter Marks of 5 Subject").split()
  sum=int(marathi)+int(hindi)+int(english)+int(math)+int(science)
  per=(sum/500)*100
  print("Percentage :",per,"%")
  if per>=90:
    print("Grade A")
  elif per>=80:
    print("Grade B")
  elif per>=70:
    print("Grade c")
  elif per>=60:
    print("Grade D")
  else:
    print("FAIl")
  ```
  ⚙️ Output:
  >Enter Marks of 5 Subject: 91 92 93 94 95
  Percentage : 93.0 %
  Grade A
  </p>
</details>


## 🔗 Some Useful Links

## 📖 References

<!-- FOOTER -->
<p align="center">
  <img  src="./../assets/footer.png" />
</p>  