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
# 🖥️ Introduction to DRY Programming

<!--
- Welcome to the DRY Programming module!
- Today, we will explore the importance of the DRY principle in coding.
- We will learn how to avoid repetition in our code by using functions.
-->

---
<!-- _footer: ""  -->
# 🛠️ DRY 

- **DRY Principle:** Avoid repeating code.
- **Importance:** Makes code easier to read, maintain, and debug.
  
```python
# Without DRY
print("Hello, Alice!")
print("Hello, Bob!")
# With DRY
def greet(name):
    print(f"Hello, {name}!")
greet("Alice")
greet("Bob")
```

<!--
- DRY stands for Don't Repeat Yourself.
- It helps in reducing redundancy and making code maintainable.
- Show how using a function can avoid repeated code blocks.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/dry.mp4" controls width="100%"></video>

---

<!-- _footer: ""  -->
# 🔍 What is a Function?

- **Function:** A reusable block of code that performs a specific task.
- **Purpose:** Simplifies complex programs by breaking them into smaller, manageable pieces.
- **Example:** A basic function that prints a message.

```python
# Example of a simple function
def say_hello():
    print("Hello, World!")

say_hello()
```

<!--
- Explain that a function is a named section of a program that performs a specific task.
- Functions help in organizing code logically.
- Provide a basic example of a function that prints a message.
-->

---

# 📝 Basic Function

- **Define Function:** Use `def` keyword.
- **No Arguments, No Return Value:** Simple structure.
- **Example:** Function with no arguments and no return value.

```python
def greet():
    print("Hi there!")
greet()
```

<!--
- Define a basic function with no arguments and no return value.
- Emphasize the use of the `def` keyword.
- Show an example function and how to call it.
-->

---

# 🏃‍♂️ Calling Functions

- **Call Function:** Use function name followed by parentheses.
- **Example:** Execute a simple function.

```python
def greet():
    print("Hello, everyone!")

greet()  # Calling the function
```

<!--
- Explain how to call a function by using its name and parentheses.
- Demonstrate with an example of a simple function call.
-->
---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/funs.mp4" controls width="100%"></video>