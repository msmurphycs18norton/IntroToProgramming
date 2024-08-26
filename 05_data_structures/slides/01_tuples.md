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

# 📚 Tuples in Python

---
<!-- _footer: ""  -->
# 🤔 What are Tuples?

- Tuples are a type of data structure in Python.
- They are used to store multiple items in a single variable.
- Tuples are immutable, meaning once created, they cannot be changed.

```python
# Creating a tuple
my_tuple = (1, 2, 3, "apple", "banana")
print(my_tuple)
```

<!--
- Tuples group related data together.
- Immutability means you can't modify a tuple after creation.
-->

---
<!-- _footer: ""  -->
# 🛠️ How to Create Tuples?

- Use parentheses `()` to create tuples.
- Tuples can store mixed data types.
- You can create an empty tuple using `()`.

```python
# Creating a tuple
my_tuple = (1, 2, 3, "apple", "banana")
print(my_tuple)

# Creating an empty tuple
empty_tuple = ()
print(empty_tuple)
```

<!--
- Emphasize the use of parentheses.
- Tuples can contain integers, strings, and other data types.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/cre_tuples.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 🔍 Accessing Elements in a Tuple

- Use indexing to access tuple elements, indexing starts at 0.
- Tuples support negative indexing to access elements from the end.

```python
# Accessing elements
print(my_tuple[0])  # Output: 1
print(my_tuple[3])  # Output: apple
print(my_tuple[-1]) # Output: banana
```

<!--
- Highlight that indexing starts from zero.
- Demonstrate accessing specific elements.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/acc_tuples.mp4" controls width="100%"></video>

---

# 🚫 Immutability of Tuples

- Tuples cannot be changed after creation.
- Any attempt to modify will result in an error.
- Immutability makes tuples useful for read-only data.

```python
# Attempting to change a tuple element
try:
    my_tuple[1] = "orange"  # This will cause an error
except TypeError as e:
    print(e)
```

<!--
- Explain what immutability means.
- Show an example that results in an error.
-->

---

# 🔄 Common Tuple Operations

- Use slicing to get a range of elements.
- Negative indexing accesses elements from the end.
- You can concatenate tuples using the `+` operator.
- You can repeat tuples with the `*` operator.

<!--
- Explain slicing and its syntax.
- Show examples of negative indexing, concatenation, and repetition.

```python
# Indexing and slicing
print(my_tuple[1:3])  # Output: (2, 3)
print(my_tuple[-1])  # Output: banana

# Concatenation
new_tuple = my_tuple + ("cherry",)
print(new_tuple)  # Output: (1, 2, 3, 'apple', 'banana', 'cherry')

# Repetition
repeated_tuple = my_tuple * 2
print(repeated_tuple)  # Output: (1, 2, 3, 'apple', 'banana', 1, 2, 3, 'apple', 'banana')
```

-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/com_tuples.mp4" controls width="100%"></video>