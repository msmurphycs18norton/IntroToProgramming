## Functions

This module provides an introduction to functions, emphasizing the DRY (Don't Repeat Yourself) principle. It covers the basic structure of functions, how to define and call them, and their components such as parameters and return statements.

### Key Concepts:

- **DRY - Don't Repeat Yourself:** Why is it important?
- **What is a function?** Understanding the concept.
- **Basic Function:** Define and use a simple function without arguments and return values.
- **Calling Functions:** How to execute a function in your code.
- **Components of a Function:** Name, parameters, body, and return statement.
- **Parameters/Arguments:** Basics of positional and keyword arguments.
- **Positional Arguments:** Order matters.
- **Keyword Arguments:** Flexibility in argument order.
- **Default Values for Arguments:** Setting default parameter values.
- **Type Hinting:** Specifying argument and return types.
- **Documenting Functions:** Writing clear and helpful docstrings.

### Outcomes:

Upon completion of this module, students will be able to:

- Define and use basic functions in their code.
- Understand and implement positional and keyword arguments.
- Use return statements to get values from functions.
- Set default values for function parameters.
- Implement type hinting for function arguments and return types.
- Document their functions using docstrings.

### Guiding Questions:

Consider the following questions as you review the learning resources this week:

1. Why is the DRY principle important when writing functions?
2. How do positional and keyword arguments affect the way we call functions?
3. How can we ensure our functions are flexible and well-documented?

### Possible Lessons:

- **Create a Function:** Write a function that prompts the user to enter a number and returns it as a float. If the input is not a number, ask the user to try again using `str.isdigit()`.

```python
def get_number():
    while True:
        num_str = input("Please enter a number: ")
        if num_str.isdigit():
            return float(num_str)
        else:
            print("That's not a number. Try again.")

number = get_number()
print(f"You entered the number: {number}")
```

- **Using Functions to Reduce Code:** Integrate the `get_number()` function into a number calculator program to simplify the code and demonstrate the DRY principle.