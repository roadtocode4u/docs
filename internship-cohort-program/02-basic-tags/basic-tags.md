# Lecture-1 Basic Tags of HTML

## 💁🏻‍♀️ Types of Tags

### Based on closing tag

1. Empty Tag :- Tags with no closing tag
```
for e.g. :- <br> , <br/>
```
2. Container Tag :- Tags with both opening and closing tag
```
for e.g. :- <h1> </h1>
```

### Based on Names

1. Semantic Tags :- Semantic tag have meaningful name of the information in webpage.
```
for e.g. :- <form> , <table>
```

2. Non Semantic Tags :- Non Semantic tag don't tell anything about the content.
```
for e.g. :- <div> , <a>
```

## Bold Tag

Defines bold text

```
<b>Bold Text</b>
```
**💻Example :**
```html
<!Doctype html>
<html>
    <head>
        <title>Basic Tags</title>
    </head>
    <body>
        Normal Text <br/>
        <b>Bold Text</b>
    </body>

</html>
```
**⚙️ Output :**

![Output](output.png) 

## Italic Tag

Defines italic text

```
<i>Text</i>
```
**💻Example :**
```html
<body>
    Normal Text <br/>
    <i>Italic Text</i>
</body>
```
**⚙️ Output :**

![Output](output1.png)

## Underline Tag

Use to underline a text in HTML

```
<u>Underline Text</u>
```
**💻Example :**
```html
<body>
    Normal Text <br/>
    <u>Underline Text</u>
</body>
```
**⚙️ Output :**

![Output](output2.png)

## Delete Tag

It is used to mark a portion of text which has been deleted from the document.

```
<del>Delete Text</del>
```
**💻Example :**
```html
<body>
    Normal Text <br/>
    <del>Delete Text</del>
</body>
```
**⚙️ Output :**

![Output](output3.png)

## Bold & Italic Tag

Defines bold & italic text

```
<i><b>Sample Text</b></i>
OR
<b><i>Sample Text</i></b>
```
**💻Example :**
```html
<body>
    Normal Text <br/>
    <i><b>Sample Text</b></i><br/>
    <b><i>Sample Text</i></b>
</body>
```
**⚙️ Output :**

![Output](output4.png)

#### If you want to underline text

**💻Example :**
```html
<body>
    Normal Text <br/>
    <i><b>Sample<u> Text</u></b></i>
</body>
```
**⚙️ Output :**

![Output](output5.png)

## Superscript

Superscript is a number or letter that written above the normal text.

```
10<sup>th</sup>

```
**💻Example :**
```html
<body>
    10th<br/>
    10<sup>th</sup><br/>
</body>
```
**⚙️ Output :**

![Output](output6.png)

## Subscript

Subscript is a number or letter that written below the normal text.

```
H<sub>2</sub>O

```
**💻Example :**
```html
<body>
    H20<br/>
    H<sub>2</sub>0
</body>
```
**⚙️ Output :**

![Output](output7.png)

## 🤔 How to add image in webpage ?

```
<img/>
```
### Attribute

It provide extra information about tag
  
```
src = source
key = src
value = url
```
**💻Example :**
```html
<body>
    <img src="bike.jpg"/>
</body>
```
**⚙️ Output :**

![Output](output8.png)

```
alt = alternative text
```
**💻Example :**
```html
<body>
    <img src="bike.jpg" alt="image of bike"/>
</body>
```
**⚙️ Output :**

![Output](output9.png)

  
## 🤔 How to add width & height to image in html ?

**💻Example :**
```html
<body>
    <img src="bike.jpg" width="50px" alt="image of bike"/>
</body>
```
**⚙️ Output :**

![Output](output10.png)

**💻Example :**
```html
<body>
    <img src="bike.jpg" height="200px" alt="image of bike"/>
</body>
```
**⚙️ Output :**

![Output](output8.png)


## 🏠 HomeWork

>1️⃣ Create a Webpage using basic html tags and image tag where all the info is shown about you.
