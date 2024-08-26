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
# 🚦 Circuit Breakers in Loops

<!--
- Introduction to circuit breakers in loops: break and continue.
-->

---

# 🛑 Using `break` in Loops

- The `break` statement exits the loop immediately.
- Useful for stopping a loop when a certain condition is met.

```python
for i in range(5):
    if i == 3:
        break
    print(i)
```

<!--
- Explain that the loop stops when `i` equals 3.
- Only numbers 0, 1, 2 are printed.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/break.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# ↪️ Using `continue` in Loops

- The `continue` statement skips the rest of the code in the current iteration.
- Moves to the next iteration of the loop.

```python
for i in range(5):
    if i == 3:
        continue
    print(i)
```

<!--
- Explain that when `i` equals 3, the loop skips to the next iteration.
- The numbers 0, 1, 2, 4 are printed, but not 3.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/continue.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
# ⚙️ Combining break and continue

- You can use both `break` and `continue` in the same loop for complex control flow.

```python
for i in range(10):
    if i == 3:
        continue
    if i == 7:
        break
    print(i)
```

<!--
- Explain that the loop skips printing 3 and stops completely when `i` equals 7.
- The numbers 0, 1, 2, 4, 5, 6 are printed.
-->

---
<!-- _footer: ""  -->
# 🧩 Search for a Value

- Use `break` to stop searching a list once the target value is found.
- Use `continue` to skip invalid or unwanted values.

```python
numbers = [1, 2, 3, -1, 4, 5]
for num in numbers:
    if num < 0:
        continue
    if num == 4:
        print("Found 4!")
        break
    print(num)
```

<!--
- Explain that the loop skips the negative number.
- Stops once the number 4 is found and prints "Found 4!".
-->