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

# Arithmetic and Compound Operations 🧮

*Python Basics 03*

---

## 📚 What will we learn?

- How to perform basic arithmetic operations
- How to use compound assignment operators

---

## ➕ Basic Arithmetic Operations

- Addition: `+`
- Subtraction: `-`
- Multiplication: `*`

```python
a = 10
b = 5

print(a + b)  # 15
print(a - b)  # 5
print(a * b)  # 50
```

<!-- 
- This slide explains the basic arithmetic operations in Python.
- Show examples of addition, subtraction, multiplication, division, and exponentiation.
- Emphasize the importance of understanding these fundamental operations.
-->

---

## 🧮 Division and Exponentiation

- Division uses `/` and always returns a float.
- Exponentiation uses `**` for powers.

```python
a = 9
b = 2

print(a / b)  # 4.5
print(a ** b) # 81
```

<!-- 
- Highlight the fact that division results in a float even if the numbers are integers.
- Show how to use `**` for exponentiation, providing examples.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/arithmetic_ops.mp4" controls width="100%"></video>

---

## 📥 Compound Assignment Operators

- Shorthand for arithmetic operations and assignment.
- `+=`, `-=`, `*=`, `/=`, `**=`

```python
x = 10
x += 5  # x = x + 5
x *= 2  # x = x * 2
print(x) # 30
```

<!-- 
- Introduce the concept of compound assignment operators as shortcuts for combining operations with assignment.
- Provide examples showing how to use `+=`, `*=`, and others.
- Emphasize the convenience and efficiency of using these operators.
-->

---

## 🧑‍💻 Practical Example: Compound Operations

```python
total = 100
total -= 20  # total = total - 20
total /= 4   # total = total / 4
print(total) # 20.0
```

- Decrease total by 20 and then divide by 4.
- Shows use of `-=` and `/=`.

<!-- 
- Provide a practical example to illustrate compound assignment operations in a real-world context.
- Emphasize the steps and the resulting value after each operation.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/compound_ops.mp4" controls width="100%"></video>

---

## 📝 Practice Activity: Simple Calculator

- Create a program that:
    - Assigns two numbers to variables.
    - Performs all basic arithmetic operations with these numbers.
    - Displays the results using print().

<!-- 
- Encourage students to apply what they’ve learned by creating a simple program that performs arithmetic operations.
- Guide them through assigning values to variables, performing arithmetic operations, and displaying the results using F-strings.
- Emphasize the importance of practicing these concepts to solidify understanding.
- num1 = 8
  num2 = 3

  print(f"{num1} + {num2} = {num1 + num2}")
  print(f"{num1} - {num2} = {num1 - num2}")
  print(f"{num1} * {num2} = {num1 * num2}")
  print(f"{num1} / {num2} = {num1 / num2}")
  print(f"{num1} ** {num2} = {num1 ** num2}")
-->
