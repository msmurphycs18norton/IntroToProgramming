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

# Casting in Python 🐍

*Python Basics 02*

*Special thank you to Kerri Murphy*

---

## 📚 What will we cover today?

- Review printing stings
- Data types, string, integers, and decimals
- Change numbers into stings
- Changing the color of our text

---

## 🖨️ Review: Printing Strings

- Remember, we use `print()` to display text.
- Text must be inside quotes: `"Hello, world!"`

```python
print("Hello, Python learners!")
```

- This prints: `Hello, Python learners!`

<!-- 
- This slide reviews the basics of printing strings in Python, reinforcing the use of the `print()` function.
- It's important to recall that strings must be enclosed in quotes to be recognized as text.
- Encourage students to experiment with printing different strings to see the output.
-->

---

## 🧐 Review Combining Strings and Variables

```python
name = "Woman"
print("Wonder", name)
```

- What does it do? It prints: `Wonder Woman`
- Using a comma between items in `print()` automatically adds a space between them.

<!-- 
- This slide focuses on a simple yet fundamental concept of combining string literals and variables in a print statement.
- The use of a comma within the `print()` function to seamlessly join strings and variables with a space is highlighted.
- Encourage students to experiment with combining different strings and variables to see how Python handles spacing and concatenation.
-->

---

## 🧐 Review String Concatenation


```python
name = "Bat"
print(name + "man")
```

- What's the result? It prints: `Batman`
- The `+` concatenates the variable `name` with the string `"man"` without any spaces.

<!-- 
- This slide delves into the concept of string concatenation using the `+` operator, a key technique in Python programming.
- It points out the direct joining of strings without automatic space insertion, contrasting it with the behavior seen when using commas in print statements.
- Encourage exploration of string concatenation with different variables and strings to understand its versatility and application in forming new strings or messages.
-->

---

## 🔢 Data Types

| Data Type | Description                             | Example |
|:-----------|:-----------------------------------------|---------|
| String<br>(`str`) | Text enclosed in quotes.            | `"Hello"` |
| Integer<br>(`int`) | Whole numbers without a decimal.  | `5`      |
| Decimal<br>(`float`) | Numbers with a decimal point.     | `3.14`   |

<!-- 
- This slide introduces the basic data types in Python, focusing on strings, integers, and decimals (floats).
- Use examples to illustrate each type, helping students to differentiate between them.
- Emphasize that understanding these types is crucial for performing different operations in Python.
-->

---

## 🤔 Understanding Variable Types

- String variables are defined with their values inside quotes, like `"Hello"`.
- Integer and decimal (float) variables are specified without quotes, for example, `5` and `3.14`.

```py
x = "7"
```
So, what type of variable is `x`?


<!-- 
- This slide clarifies how to distinguish between string, integer, and float variables based on the presence or absence of quotes.
- It emphasizes the importance of quote usage in defining the type of a variable.
- The question about `x = "5"` serves as a practical example to apply this understanding, reinforcing the concept that the type of a variable is determined by how it's defined.
-->

---

## 🍩 Printing with Numbers

- Want to include numbers in your print statements?

- Imagine you have a variable for donuts:
  - `donuts = 10` (It's an **integer** variable.)

- Goal: Print "I would buy 10 donuts if I had money!" using the `donuts` variable.

<!-- 
- This slide simplifies the concept of printing a sentence that includes the value of an integer or float variable.
- It sets a clear task for students to incorporate a numeric variable into a string output, encouraging practical application of variable printing.
- Encourage experimentation with different sentences and numeric variables to explore the flexibility of print statements.
-->

---


<!-- _footer: ""  -->
<!-- _header: "" -->

<video src="../media/string_concatenation_casting.mp4" controls width="100%"></video>

<!-- 
[video]{../media/01_printing/string_concatenation_casting.mp4}
-->

---

## 🧩 Why Doesn't This Work?

- Trying to print a sentence with a number:

```python
donuts = 10
print("I would buy " + donuts + " donuts if I had money!")
```

- **Problem:** It results in an error. Why?
  - Because you can't concatenate strings and integers directly in Python.

<!-- 
- This slide addresses a common error when attempting to concatenate strings with integers directly.
- It highlights the type mismatch between strings and integers as the cause of the error, setting the stage for discussing type conversion.
- Encourage critical thinking about data types and the importance of converting integers to strings for successful concatenation.
-->

---

## 🎭 The Need for Casting in Concatenation

- When using `+` to combine text with numbers, you must match their types.

- **Casting** is converting one data type to another, like turning integers into strings with `str()`.

- **Why?** Python requires the same data type for concatenation to prevent errors.

<!-- 
- This slide explains the concept of casting and its importance in string concatenation involving numbers.
- It clarifies that casting is necessary to convert numeric values into strings to concatenate them with other strings.
- Highlight the practicality of casting in avoiding type mismatch errors and ensuring smooth code execution.
-->
---

## 🔄 Simplifying Casting

- **Casting** temporarily changes a variable's type to fit the operation.

- For printing with numbers:
  - `donuts = 10` (Python sees this as an integer, not a string.)

- To include `donuts` in a print statement, convert it to a string:
  - `str(donuts)`

<!-- 
- This slide streamlines the explanation of casting, focusing on its role in enabling variables to be used in print statements.
- It poses a rhetorical question about Python's type recognition to engage students in thinking about data types.
- The solution, using `str()` for conversion, is presented clearly to emphasize the utility of casting in mixed-type operations.
-->

---

## 🤹 Combining Strings and Numbers

- To include numbers in a sentence, use `str()` and `+`:

```python
donuts = 10
print("I would buy " + str(donuts) + " donuts if I had money!")
```

- This technique ensures numbers are correctly formatted as part of the text.

<!-- 
- This slide offers a concise example of how to use `str()` to convert a number to a string for concatenation with other strings using the `+` operator.
- It emphasizes the practical application of these concepts to form complete, coherent sentences that include numeric variables.
- Encourage students to practice this method with different variables and sentences to build confidence in combining data types.
-->

---

## 🍫 Crafting a Sweet Print Statement

- In Grader Than IDE, create a new Python file to begin your program.
- Create a variable for the number of candy bars.
- Create another variable for the type of candy bar.
- Combine these variables in a print statement, along with additional text, to create a full sentence.

<!-- 
- This slide guides students through creating variables for numeric and string data and then using these variables in a print statement.
- Encourage experimentation with different values and text, emphasizing the flexibility of Python in handling data types and string concatenation.
-->

---

<!-- _footer: "" -->

## 🛠 Common Mistakes to Avoid

- **Always** enclose your string variables in quotes. Example: `type_of_candy = "Snickers"`
- Don't forget to use `+` or `,` to concatenate or separate variables in print statements.
- Enclose any standalone text in your print statements within quotes.
- Remember to convert numeric variables to strings using `str()` when combining them with text.

<!-- 
- This slide outlines common mistakes beginners might make when writing Python code in the Grader Than IDE, focusing on string and variable handling in print statements.
- It provides clear guidelines on the correct use of quotes for strings, concatenation techniques, and type conversion for numeric variables.
- Encourage students to review their code for these common errors to enhance their debugging skills and code quality.
-->

---

## 🌈 Adding Color to Text

- To colorize your text in print statements:
  - Begin with `\033[`, then add the color code, and end with `m`.
  - Example for blue: 
  
  ```py
  print("\033[34m" + "This text will be blue.")
  ```

<!-- 
- This slide provides a clear format for using these codes, highlighting the structure and an example for applying a blue color to text.
- Encourage exploration of different color codes to see how they change the appearance of the text output.
-->

---
<!-- _footer: "" -->

```py
print("\033[<COLOR CODE>m"+"colorful text")
```
<table>
<tr>
<td style="font-size:65%">

| Color     | Color Code |
|-----------|------------|
| Black     | `30` |
| Red       | `31` |
| Green     | `32` |
| Yellow    | `33` |
| Blue      | `34` |
| Magenta   | `35` |
| Cyan      | `36` |
| White     | `37` |
| Stop Coloring     | `0` |
    
</td>
</tr>
</table>

<!-- 
- This slide provides a handy reference table for ANSI color codes, allowing students to easily find and apply different colors to text output in their Python print statements.
- Encourage experimentation with these color codes to enhance the visual appeal of console output and to distinguish different types of information or messages.
-->

---

## 🎨 Resetting Text Color

- To revert text color back to default after coloring:
  - Use `\033[0m` immediately following the colored text.

```python
print("\033[34m" + name + "\033[0m", "this story is about you!")
```

- In this example, only `name` will appear in blue, and the rest of the text will be in the default color.

<!-- 
- This slide explains how to stop text color changes using ANSI escape codes, ensuring that only specific parts of the text are colored.
- It provides a practical example of how to apply color to a variable and then reset to default color for the following text.
- Encourage students to use this technique to emphasize important parts of their output or to make their printouts more visually engaging.
-->
