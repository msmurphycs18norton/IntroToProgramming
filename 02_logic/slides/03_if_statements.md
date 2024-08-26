---
marp: true
author: Grader Than Technology LLC
title: "Variables"
theme: uncover
//class: invert
lang: en
size: 16:9
header: ![Grader Than Logo w:40](../media/gt-logo.png)
footer: © [Grader Than Technology LLC](https://www.graderthan.com/)
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

# If Statements in Python 🐍

*Logic 03*

---

## 📚 What will we learn?

- What are if statements?
- How to use `if`, `elif`, and `else`?
- Constructing conditional logic.

---

## 🧠 What are If Statements?

- If statements allow you to execute code based on conditions.
- Syntax:
  - `if`: Executes block if condition is true.
  - `elif`: Executes block if previous conditions are false and condition is true.
  - `else`: Executes block if all previous conditions are false.

<!-- 
- Explain the structure and use of if statements.
- Provide a basic example demonstrating `if`, `elif`, and `else`.
- Highlight how conditions control the flow of a program.
-->

---

## 🔗 Using If Statements with Comparison Operators

- Combine if statements with comparison operators for more complex conditions.

```python
age = 18
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

<!-- 
- Show how to use comparison operators within if statements.
- Provide an example that checks if a person is an adult based on their age.
- Emphasize the use of comparison operators to evaluate conditions.
-->

---

## 🚦 Nested If Statements

- Use nested if statements for multiple layers of conditions.

```python
number = 25
if number > 10:
    if number < 20:
        print("Number is between 10 and 20.")
    else:
        print("Number is greater than or equal to 20.")
else:
    print("Number is 10 or less.")
```

<!-- 
- Explain the concept of nested if statements.
- Provide an example that demonstrates multiple layers of conditions.
- Highlight the importance of indentation for readability and structure.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/if.mp4" controls width="100%"></video>

---

## 🧩 Logical Expressions in If Statements

- Use logical expressions (`and`, `or`, `not`) to combine conditions.

```python
temperature = 22
if temperature > 0 and temperature < 30:
    print("The weather is nice.")
else:
    print("The weather is extreme.")
```

<!-- 
- Show how to use logical expressions within if statements.
- Provide an example that combines conditions using `and`.
- Emphasize how logical expressions can simplify complex conditions.
-->

---
<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/log_exps_if.mp4" controls width="100%"></video>

---
<!-- _footer: ""  -->
## 📝 Example: Grading System

- Implement a grading system using if statements.

```python
score = 85
if score >= 90:
    grade = 'A'
elif score >= 80:
    grade = 'B'
elif score >= 70:
    grade = 'C'
elif score >= 60:
    grade = 'D'
else:
    grade = 'F'
print(f"Your grade is: {grade}")
```

<!-- 
- Provide a practical example of using if statements to implement a grading system.
- Show how to assign grades based on score ranges.
- Highlight the use of `elif` for multiple conditions.
-->

---

## 🛠 Practice: Voting Eligibility Checker

- Create a program that checks if a person is eligible to vote based on their age.

<!-- 
- Encourage students to apply what they've learned by creating a voting eligibility checker.
- Show how to use if statements to check multiple conditions based on user input.
- Emphasize the importance of handling edge cases like invalid input.
-->