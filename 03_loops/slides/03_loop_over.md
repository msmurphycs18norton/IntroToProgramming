---
marp: true
author: Grader Than Technology LLC
title: "Variables"
theme: uncover
//class: invert
lang: en
size: 16:9
header: ![Grader Than Logo w:40](../media/gt-logo.png)
footer: © <a href="https://www.graderthan.com/">Grader Than Technology LLC</a>
enableHtml: true
style: |
    :root {
    --color-background: #eeeeee;
    --color-foreground: #070D59;
    --color-background-code: #DCDCDC;
    }
    header img {
        float: left;
    }
    footer {
        font-weight: 500;
        color: #4178bc;
        padding: 10px;
    }
    footer a {
        color: #4178bc;
    }
    pre code {
        padding: .7rem !important;
        border-radius: 8px;
    }
    section {
        font-family: 'Poppins' 'Roboto', 'Segoe UI', 'Liberation Sans', 'Helvetica', 'Arial', sans-serif;
    }
---
# 🔄 Looping Over Sequences in Python

<!--
- Introduction to looping over different sequences in Python.
-->

---
<!-- _footer: ""  -->
# 📏 Looping Over `range()`

- `range()` generates a sequence of numbers.
- Different ways to use `range()`: `range(stop)`, `range(start, stop)`, `range(start, stop, step)`.

```python
for i in range(1, 6):
    print(i)
```

```python
for i in range(1, 10, 2):
    print(i)
```

<!--
- Explain `range(stop)` starts from 0.
- `range(start, stop)` starts from start.
- `range(start, stop, step)` allows custom steps.
- First example prints 1 to 5.
- Second example prints 1, 3, 5, 7, 9.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/range.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 🔡 Looping Over Strings

- Strings are sequences of characters.
- You can loop through each character in a string.

```python
for char in "hello":
    print(char)
```

```python
word = "world"
for char in word:
    print(char)
```

<!--
- Explain that each character in "hello" is printed one by one.
- Show how to iterate through a string stored in a variable.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/over_strings.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 📋 Looping Over Lists

- Lists are ordered collections of items.
- You can loop through each item in a list.

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

```python
colors = ["red", "green", "blue"]
for color in colors:
    print(color)
```

<!--
- Define a list as an ordered collection.
- Show how each fruit in the list is printed.
- Demonstrate looping over a list of colors.
-->
---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/over_lists.mp4" controls width="100%"></video>