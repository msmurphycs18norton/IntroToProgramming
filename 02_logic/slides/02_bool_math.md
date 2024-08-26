---
marp: true
author: Grader Than Technology LLC
title: "Variables"
theme: uncover
//class: invert
lang: en
size: 16:9
header: ![Grader Than Logo w:40](../media/gt-logo.png)
footer: © [Grader Than Technology LLC](https://www.graderthan.com/)
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

# Boolean Math in Python 🐍

*Logic 02*

---

## 📚 What will we learn?

- What is Boolean math?
- The order of operations in logical expressions
- How to perform Boolean operations?
- Understanding Boolean values in arithmetic operations.

---


## 📏 What is Boolean Math?

- Boolean values: `True` and `False`
- Used in logical operations and conditions
- `True` is equivalent to `1`
- `False` is equivalent to `0`

```python
print(True)   # 1
print(False)  # 0
```

<!-- 
- Describe what Boolean math is.
- Show how Boolean values can be treated as integers (True = 1, False = 0).
- Demonstrate simple Boolean values as integers.
-->

---

## 🧮 Order of Operations in Logical Expressions

- Use parentheses `()` to group expressions.
- Follow the order: `not`, `and`, `or`.

```python
result = (True or False) and not False
print(result)  # True
```

<!-- 
- Explain the order of operations in logical expressions.
- Illustrate with an example that uses multiple logical operators.
- Stress the importance of parentheses for clarity.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/order_of_ops_logical_exps.mp4" controls width="100%"></video>

---

## ✖️ `and` as Multiplication in Boolean Math

- `and` is similar to multiplication.
- Both must be `True` to be `True` (1 * 1 = 1).

```python
print(True and True)   # True (1 * 1)
print(True and False)  # False (1 * 0)
```

<!-- 
- Explain how `and` works like multiplication.
- Provide examples showing the equivalence.
- Emphasize the logical consistency of this approach.
-->

---

## ➕ `or` as Addition in Boolean Math

- `or` is similar to addition.
- At least one must be `True` to be `True` (1 + 0 = 1).

```python
print(True or False)   # True (1 + 0)
print(False or False)  # False (0 + 0)
```

<!-- 
- Explain how `or` works like addition.
- Provide examples showing the equivalence.
- Highlight the intuitive nature of this logic.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/bool_math.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
## 🧠 Boolean Values in Arithmetic Operations

- Combining Boolean values with integers.
- Boolean values can be used in arithmetic operations with integers.

```python
result = True + 3
print(result)  # 4

result = False + 10
print(result)  # 10
```

<!-- 
- Explain how Boolean values can be combined with integers in arithmetic operations.
- Provide examples to illustrate this combination.
- Highlight the practicality of Boolean arithmetic in programming.
-->