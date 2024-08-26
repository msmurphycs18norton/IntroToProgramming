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
# 🌀 Understanding While Loops in Python

<!--
- Introduction to while loops in Python.
-->

---

# 🤔 What is a While Loop?

- A while loop repeats a block of code as long as a condition is true.
- It's great for when you don't know in advance how many times you need to repeat an action.

```python
i = 1
while i <= 5:
    print(i)
    i += 1
```

<!--
- Explain that the loop starts with `i` equal to 1.
- Each iteration checks if `i` is less than or equal to 5.
- `i` is incremented by 1 each time.
- The loop stops when `i` becomes 6.
-->

---

# 🧩 Understanding Syntax

- While loop syntax:

```python
while condition:
    # code block
```
---
# 🛠 Example
- The code block inside the loop runs repeatedly as long as the condition is true.

```python
count = 0
while count < 3:
    print("Hello!")
    count += 1
```

<!--
- Show the general structure of a while loop.
- Explain that the condition is checked before each iteration.
- The loop prints "Hello!" three times.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/while_loops.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 🔄 While vs. If 

- A while is like an if that keeps checking the condition until it's false.
- If runs once if the condition is true, while keeps running.

```python
i = 1
while i <= 5:
    print(i)
    i += 1
if i <= 5:
    print(i)
```

<!--
- Highlight that the if statement checks the condition once.
- Emphasize that the while loop continues checking and executing until the condition is false.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/while_vs_if.mp4" controls width="100%"></video>
