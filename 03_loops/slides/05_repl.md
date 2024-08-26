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
# 🔄 REPL (Read-Evaluate-Print Loop) in Python

<!--
- Introduction to REPL: Read-Evaluate-Print Loop in Python.
-->

---
<!-- _footer: ""  -->
# 🌀 What is a REPL?

- REPL stands for Read-Evaluate-Print Loop.
- Continuously reads user input, evaluates it, and prints the result.
- Useful for creating interactive programs.

```python
while True:
    command = input("Enter command: ")
    if command == "exit":
        break
    print(f"Executing {command}")
```

<!--
- Explain the concept of REPL.
- Show a simple example that reads commands and prints them.
-->

---
<!-- _footer: ""  -->
# 📜 REPL Structure
  1. **Read**: Get user input.
  2. **Evaluate**: Process the input.
  3. **Print**: Display the result.
  4. **Loop**: Repeat until a termination condition is met.

```python
while True:
    command = input("Enter command: ")
    if command == "exit":
        print("Goodbye!")
        break
    print(f"Executing {command}")
```

<!--
- Highlight each step in the REPL structure.
- Explain how the loop continues until the user types "exit".
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/repl.mp4" controls width="100%"></video>

---

# 🚦 Using `break` in a REPL

- `break` is used to exit the loop and stop the REPL.

```python
while True:
    command = input("Enter command: ")
    if command == "exit":
        print("Goodbye!")
        break
    print(f"Executing {command}")
```

<!--
- Explain that typing "exit" will break the loop and end the REPL.
-->

---
<!-- _footer: ""  -->
# 🧩 Adding Functionality

- You can add more commands to your REPL for different functionalities.

```python
while True:
    command = input("Enter command: ")
    if command == "exit":
        print("Goodbye!")
        break
    elif command == "hello":
        print("Hello, user!")
    else:
        print(f"Unknown command: {command}")
```

<!--
- Show how to handle multiple commands.
- Explain the use of `elif` to add more functionalities.
-->
