## Homework Assignment: Simple Command Line Calculator

### Objective:
Create a simple command line calculator that performs basic arithmetic operations. The calculator will accept user input, perform calculations, and display the results using print statements. You will practice using variables, data types, casting, F-strings, arithmetic operations, compound assignment operators, and input statements.

### Instructions:

1. **Accept User Input:**
   - Prompt the user to enter two numbers. 
   - Prompt the user to choose an arithmetic operation (addition, subtraction, multiplication, division, exponentiation).

2. **Convert Input:**
   - Convert the user input for numbers from strings to floats.
   
3. **Perform Calculations:**
   - Perform the chosen arithmetic operation on the two numbers.
   
4. **Display Results:**
   - Use F-strings to format and display the result of the calculation.

5. **Include Error Handling:**
   - Handle possible division by zero errors gracefully.

### Requirements:

1. **Prompt and Input:**
   ```python
   num1 = input("Enter the first number: ")
   num2 = input("Enter the second number: ")
   operation = input("Choose an operation (+, -, *, /, **): ")
   ```

2. **Type Casting:**
   ```python
   num1 = float(num1)
   num2 = float(num2)
   ```

3. **Arithmetic Operations:**
   - Use if-elif-else statements to perform the chosen operation.
   ```python
   if operation == "+":
       result = num1 + num2
   elif operation == "-":
       result = num1 - num2
   elif operation == "*":
       result = num1 * num2
   elif operation == "/":
       if num2 != 0:
           result = num1 / num2
       else:
           result = "Error: Division by zero"
   elif operation == "**":
       result = num1 ** num2
   else:
       result = "Invalid operation"
   ```

4. **Display the Result:**
   ```python
   if isinstance(result, float):
       print(f"The result of {num1} {operation} {num2} is {result}")
   else:
       print(result)
   ```

### Example Output:

```
Enter the first number: 10
Enter the second number: 5
Choose an operation (+, -, *, /, **): *
The result of 10.0 * 5.0 is 50.0
```

### Bonus Challenge:
Enhance the calculator to allow the user to continue performing calculations until they decide to exit. Add a loop to repeatedly ask for input and perform calculations.

```python
while True:
    num1 = input("Enter the first number (or 'exit' to quit): ")
    if num1.lower() == 'exit':
        break
    num2 = input("Enter the second number: ")
    operation = input("Choose an operation (+, -, *, /, **): ")
    
    num1 = float(num1)
    num2 = float(num2)
    
    if operation == "+":
        result = num1 + num2
    elif operation == "-":
        result = num1 - num2
    elif operation == "*":
        result = num1 * num2
    elif operation == "/":
        if num2 != 0:
            result = num1 / num2
        else:
            result = "Error: Division by zero"
    elif operation == "**":
        result = num1 ** num2
    else:
        result = "Invalid operation"
    
    if isinstance(result, float):
        print(f"The result of {num1} {operation} {num2} is {result}")
    else:
        print(result)
```