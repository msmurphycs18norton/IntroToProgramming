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
# 📚 Components of Functions

<!--
- Today, we will learn about the different components of a function.
- We will explore the function name, parameters, body, and return statement.
- Each component plays a crucial role in defining the functionality of a function.
-->

---

# 🔖 Function Name

- **Name:** The identifier used to call the function.
- **Rules:** Must follow naming conventions (e.g., no spaces, can't start with a number).
- **Example:**

```python
def greet():
    print("Hi there!")
```

<!--
- The function name is how we reference and call the function in our code.
- It should be descriptive and follow Python's naming conventions.
- Show an example of a function name.
-->

---

# 📥 Parameters

- **Parameters:** Variables listed inside the parentheses in the function definition.
- **Purpose:** Allow functions to accept input values.
- **Example:**

```python
def greet(name):
    print(f"Hello, {name}!")
```

<!--
- Parameters are placeholders for the values (arguments) that the function will use.
- They help make functions more flexible and reusable.
- Provide an example of a function with a parameter.
-->

---

# 🔄 Function Body

- **Body:** The block of code that performs the function's task.
- **Indentation:** Must be indented to distinguish it from the rest of the code.
- **Example:**

```python
def greet(name):
    print(f"Hello, {name}!")
```

<!--
- The function body contains the code that runs when the function is called.
- Proper indentation is crucial in Python to define the scope of the function.
- Show the function body in an example.
-->

---

# ⏭️ Return Statement

- **Return Statement:** Sends a value back to the caller.
- **Purpose:** Allows functions to produce an output.
- **Example:**

```python
def add(a, b):
    return a + b
result = add(3, 5)
print(result)  # Outputs: 8
```

<!--
- The return statement allows a function to output a value to its caller.
- It's useful for functions that perform calculations or need to give back a result.
- Provide an example with a return statement.
-->
---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/comps_funs.mp4" controls width="100%"></video>