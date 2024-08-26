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
# 🛠️ Advanced Function Features

<!--
- Today, we will learn about advanced function features.
- We will explore default values for arguments, type hinting, and documenting functions.
- These features make functions more versatile, readable, and understandable.
-->

---
<!-- _footer: ""  -->
# 📜 Default Values 

- **Default Values:** Specify default values for parameters.
- **Purpose:** Allows functions to be called with fewer arguments.

```python
def greet(name="stranger"):
    print(f"Hello, {name}!")

greet()          # Uses default value
greet("Alice")   # Overrides default value
```

<!--
- Default values provide a way to make some arguments optional.
- This can simplify function calls when certain arguments often have the same value.
- Show an example with a default parameter value.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/default.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 🔠 Type Hinting

- **Type Hinting:** Specify expected types of arguments and return values.
- **Purpose:** Enhances code readability and helps catch errors early.

```python
def add(a: int, b: int) -> int:
    return a + b

result = add(3, 5)
print(result)  # Outputs: 8
```

<!--
- Type hinting indicates what types the function expects for its arguments and return value.
- This makes the code easier to understand and debug.
- Provide an example with type hints.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/type_hint.mp4" controls width="100%"></video>

---

# 📝 Documenting Your Functions

- **Docstrings:** Write clear descriptions of what the function does.
- **Purpose:** Helps others understand the function's purpose and usage.

<!--
- Documentation is crucial for maintaining and sharing code.
- A well-documented function is easier to use and debug.
- Show an example of a well-documented function.

```python
def add(a: int, b: int) -> int:
    """
    Adds two numbers and returns the result.
    
    Parameters:
    a (int): The first number.
    b (int): The second number.
    
    Returns:
    int: The sum of a and b.
    """
    return a + b
```
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/doc_funs.mp4" controls width="100%"></video>
