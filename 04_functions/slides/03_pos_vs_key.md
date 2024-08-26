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
# ⚙️ Positional vs Keyword Arguments

<!--
- Today, we will learn about positional and keyword arguments.
- We will explore the order and importance of these arguments in functions.
- We will see how positional arguments can be used as keyword arguments.
-->

---

# 📌 Positional Arguments

- **Definition:** Arguments matched to parameters by their position.
- **Order Matters:** Must be passed in the same order as parameters.

```python
def describe_pet(animal, name):
    print(f"I have a {animal} named {name}.")

describe_pet("dog", "Buddy")  # Correct order
```

<!--
- Positional arguments are assigned based on their order.
- The first argument goes to the first parameter, the second to the second, and so on.
- Provide an example with correctly ordered positional arguments.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/pos_arg.mp4" controls width="100%"></video>

---

# 🗝️ Keyword Arguments

- **Definition:** Arguments matched to parameters by their names.
- **Flexibility:** Can be passed in any order.

```python
def describe_pet(animal, name):
    print(f"I have a {animal} named {name}.")

describe_pet(name="Buddy", animal="dog")  # Order doesn't matter
```

<!--
- Keyword arguments are assigned based on the parameter names.
- They allow more flexibility as the order does not matter.
- Provide an example using keyword arguments.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/key_arg.mp4" controls width="100%"></video>

---

# 🛠️ Combining Positional and Keyword Arguments

- **Rule:** Positional arguments must come before keyword arguments.

```python
def describe_pet(animal, name):
    print(f"I have a {animal} named {name}.")

describe_pet("dog", name="Buddy")  # Valid
```

<!--
- When combining both types of arguments, positional arguments must come first.
- Show an example combining positional and keyword arguments correctly.
-->

---

# 🔄 Converting Positional to Keyword Arguments

- **All Positional Can Be Keyword:** Positional arguments can also be used as keyword arguments.

```python
def describe_pet(animal, name):
    print(f"I have a {animal} named {name}.")

describe_pet(animal="dog", name="Buddy")  # Using keyword arguments
```

<!--
- Positional arguments can always be passed as keyword arguments for clarity.
- Demonstrate converting positional arguments to keyword arguments.
-->