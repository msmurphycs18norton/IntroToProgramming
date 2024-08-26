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

# 📚 Dictionaries in Python

---

# 🤔 What are Dictionaries?

- Dictionaries are collections of key-value pairs.
- Each key is unique and maps to a value.
- Dictionaries are mutable, meaning they can be changed after creation.

```python
# Creating a dictionary
my_dict = {"name": "Alice", "age": 25, "city": "New York"}
print(my_dict)
```

<!--
- Dictionaries store data as key-value pairs.
- Keys must be unique within a dictionary.
- Values can be any data type.
-->

---

# 🛠️ Creating Dictionaries
<!-- _footer: ""  -->
- Use curly braces `{}` to create dictionaries.
- Keys and values are separated by colons `:`.
- You can create an empty dictionary using `{}`.

```python
# Creating a dictionary
my_dict = {"name": "Alice", "age": 25, "city": "New York"}
print(my_dict)

# Creating an empty dictionary
empty_dict = {}
print(empty_dict)
```

<!--
- Emphasize the use of curly braces.
- Explain the key-value pair format.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/cre_dict.mp4" controls width="100%"></video>

---
# 🔍 Accessing and Modifying Dictionary Elements

- Access elements by their keys.
- Modify elements by assigning new values.
- Add new key-value pairs.
- Delete key-value pairs.

<!--
- Demonstrate accessing dictionary values.
- Show how to update, add, and delete dictionary values.

```python
# Accessing elements
print(my_dict["name"])  # Output: Alice

# Modifying elements
my_dict["age"] = 26
print(my_dict)  # Output: {'name': 'Alice', 'age': 26, 'city': 'New York'}

# Adding new key-value pairs
my_dict["country"] = "USA"
print(my_dict)  # Output: {'name': 'Alice', 'age': 26, 'city': 'New York', 'country': 'USA'}

# Deleting key-value pairs
del my_dict["city"]
print(my_dict)  # Output: {'name': 'Alice', 'age': 26, 'country': 'USA'}
```

-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/mod_dict.mp4" controls width="100%"></video>

---

# 🧰 Dictionary Methods

- `keys()` returns all keys.
- `values()` returns all values.
- `items()` returns key-value pairs.
- `update()` adds key-value pairs from another dictionary.

<!--
- Introduce common dictionary methods.
- Demonstrate using keys, values, items, and update methods.

```python
# Dictionary methods
print(my_dict.keys())    # Output: dict_keys(['name', 'age', 'country'])
print(my_dict.values())  # Output: dict_values(['Alice', 26, 'USA'])
print(my_dict.items())   # Output: dict_items([('name', 'Alice'), ('age', 26), ('country', 'USA')])

# Updating a dictionary with another dictionary
new_info = {"email": "alice@example.com", "age": 27}
my_dict.update(new_info)
print(my_dict)  # Output: {'name': 'Alice', 'age': 27, 'country': 'USA', 'email': 'alice@example.com'}
```

-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/dict_methods.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 🔄 Using Dictionaries for Data Operations

- Add new key-value pairs to store additional information.
- Use dictionaries to organize and retrieve data efficiently.
- Iterate over dictionary keys and values for data processing.
- Combine dictionaries for comprehensive data storage.

<!--
- Explain the versatility of dictionaries.
- Show adding new data to dictionaries.
- Demonstrate iterating over dictionary keys and values.

```python
# Using dictionaries in operations
my_dict["hobbies"] = ["reading", "cycling"]
print(my_dict)  # Output: {'name': 'Alice', 'age': 27, 'country': 'USA', 'email': 'alice@example.com', 'hobbies': ['reading', 'cycling']}

# Iterating over dictionary keys and values
for key, value in my_dict.items():
    print(f"{key}: {value}")
```
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/dict_ops.mp4" controls width="100%"></video>