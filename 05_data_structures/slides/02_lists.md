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

# 📚 Lists in Python

---
<!-- _footer: ""  -->
# 🤔 What are Lists?

- Lists are a type of data structure in Python.
- They are used to store multiple items in a single variable.
- Lists are mutable, meaning they can be changed after creation.

```python
# Creating a list
my_list = [1, 2, 3, "apple", "banana"]
print(my_list)
```

<!--
- Lists group related data together.
- Mutability means you can modify a list after creation.
-->

---
<!-- _footer: ""  -->
# 🛠️ Creating Lists

- Use square brackets `[]` to create lists.
- Lists can store mixed data types.
- You can create an empty list using `[]`.

```python
# Creating a list
my_list = [1, 2, 3, "apple", "banana"]
print(my_list)

# Creating an empty list
empty_list = []
print(empty_list)
```

<!--
- Emphasize the use of square brackets.
- Lists can contain integers, strings, and other data types.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/cre_lists.mp4" controls width="100%"></video>

---

# 🔍 Accessing and Modifying List Elements

- Use indexing to access list elements.
- Indexing starts at 0.
- Lists support negative indexing to access elements from the end.
- Modify elements by assigning new values.

<!--
- Highlight that indexing starts from zero.
- Demonstrate accessing and modifying specific elements.

```python
# Accessing elements
print(my_list[0])  # Output: 1
print(my_list[3])  # Output: apple

# Modifying elements
my_list[1] = "orange"
print(my_list)  # Output: [1, 'orange', 3, 'apple', 'banana']
```
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/mod_lists.mp4" controls width="100%"></video>

---

# 🧰 List Methods

- `append()` adds an element to the end.
- `remove()` deletes the first matching element.
- `sort()` arranges elements in order.
- `reverse()` reverses the order of elements.

<!--
- Introduce common list methods.
- Demonstrate appending, removing, sorting, and reversing elements.

```python
# Appending and removing elements
my_list.append("cherry")
print(my_list)  # Output: [1, 'orange', 3, 'apple', 'banana', 'cherry']

my_list.remove("apple")
print(my_list)  # Output: [1, 'orange', 3, 'banana', 'cherry']

# Sorting and reversing elements
num_list = [3, 1, 4, 1, 5, 9]
num_list.sort()
print(num_list)  # Output: [1, 1, 3, 4, 5, 9]

num_list.reverse()
print(num_list)  # Output: [9, 5, 4, 3, 1, 1]
```

-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/list_methods.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 🔄 List Comprehensions

- Create lists using a concise syntax.
- Combine loops and conditionals to generate new lists.
- Enhance code readability and efficiency.

```python
# List comprehension
squares = [x**2 for x in range(5)]
print(squares)  # Output: [0, 1, 4, 9, 16]

# List comprehension with condition
evens = [x for x in range(10) if x % 2 == 0]
print(evens)  # Output: [0, 2, 4, 6, 8]
```

<!--
- Explain the concept of list comprehensions.
- Show examples with and without conditions.
-->
