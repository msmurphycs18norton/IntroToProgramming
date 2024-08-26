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
# User Input 📝

*Python Basics 04*

---

## 📚 What will we learn?

- How to accept user input
- How to store user input in variables
- How to convert user input to different data types

---

## 📝 Accepting User Input

- Use `input()` to accept user input as a string.

```python
name = input("Enter your name: ")
print("Hello,", name)
```

- The `input()` function displays a prompt and waits for the user to type something and press Enter.

<!-- 
- Explain that `input("Enter your name: ")` asks the user to type their name.
- `print("Hello,", name)` shows how to use the input value.
-->

---

## 🔄 Converting User Input

- By default, `input()` returns a string.
- Convert input to other types using `int()`, `float()`, etc.

```python
age = input("Enter your age: ")
age = int(age)
print("You are", age, "years old.")
```

- This converts the age input from a string to an integer.

<!-- 
- Highlight that input is initially a string and needs conversion to other types.
- Show an example of converting a string to an integer.
-->

---

## 🧪 Practical Example: Simple Calculator

- Create a program that:
  - Accepts two numbers from the user.
  - Performs basic arithmetic operations.
  - Displays the results using `print()`.

<!-- 
- Encourage students to apply what they’ve learned by creating a simple calculator program.
- Guide them through accepting user input, converting it, and performing arithmetic operations.
- Emphasize the importance of practicing these concepts to solidify understanding.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/user_input.mp4" controls width="100%"></video>

---
## 📦 Storing Multiple Inputs

- Store multiple inputs in different variables.

```python
first_name = input("Enter your first name: ")
last_name = input("Enter your last name: ")

print("Hello,", first_name, last_name)
```

- Combines multiple inputs to form a complete output.

<!-- 
- Show how to store and use multiple pieces of input data.
- Emphasize combining inputs to create a complete message.
-->
