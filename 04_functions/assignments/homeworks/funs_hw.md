## Homework Assignment: Create a Simple Number Conversion Application

### Overview

In this assignment, you will create a simple application that converts a number from one unit to another (e.g., kilometers to miles, Celsius to Fahrenheit). You will use the principles of DRY (Don't Repeat Yourself) by creating reusable functions. This assignment will help you understand the importance of functions, how to define and call them, and how to use parameters, keyword arguments, default values, type hinting, and documentation.

### Instructions

1. **Define Conversion Functions:**
    - Create a function `km_to_miles` that converts kilometers to miles.
    - Create a function `celsius_to_fahrenheit` that converts Celsius to Fahrenheit.
    - Ensure these functions take a single argument, the value to be converted, and return the converted value.

2. **Define a Main Function:**
    - Create a main function called `main` that:
      - Prompts the user to choose a conversion type (kilometers to miles or Celsius to Fahrenheit).
      - Prompts the user to enter the value to be converted.
      - Calls the appropriate conversion function and displays the result.

3. **Use Default Values and Keyword Arguments:**
    - Allow the user to specify the conversion type as a keyword argument in the `main` function with a default value.

4. **Type Hinting:**
    - Use type hinting for function arguments and return types in all functions.

5. **Documentation:**
    - Add docstrings to all functions explaining what they do, their parameters, and their return values.

### Additional Task

- Modify the `main` function to allow the user to specify the conversion type through an input prompt instead of a keyword argument.

### Submission

Submit your Python script file containing the defined functions and the main function. Ensure your code is well-documented with docstrings and follows the DRY principle.