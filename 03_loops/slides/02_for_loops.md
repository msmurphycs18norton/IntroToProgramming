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
# 🔁 Understanding For Loops in Python

<!--
- Introduction to for loops in Python.
-->

---

# 🔄 What is a For Loop?

- A for loop is used to iterate over a sequence (like a list, tuple, string).
- It's great for when you know the number of iterations in advance.

```python
for i in range(5):
    print(i)
```

<!--
- Mention that the for loop iterates over a sequence.
- Explain that `range(5)` generates numbers from 0 to 4.
- The loop prints each number.
-->

---

# 🌀 What is "Iteration"?

- Iteration means repeating a process.
- In programming, it's the repetition of a block of code.

```python
for char in "hello":
    print(char)
```

<!--
- Define iteration simply.
- Show how each character in the string "hello" is printed one by one.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/for_loops.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# 🔍 For vs. While 

- For loops: Ideal for iterating over a sequence when the number of iterations is known.
- While loops: Better for situations where the number of iterations isn't known in advance.

```python
for i in range(5):
    print(i)

i = 0
while i < 5:
    print(i)
    i += 1
```

<!--
- Contrast the use cases for for loops and while loops.
- Both examples do the same thing, but one uses a for loop and the other uses a while loop.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/for_vs_while.mp4" controls width="100%"></video>
