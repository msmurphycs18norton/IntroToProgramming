# Homework Assignment: Simple Voting Age Checker Application

## Overview

In this assignment, you will create a simple application that checks if a person is eligible to vote based on their age. You will use comparison operators, logical expressions, Boolean math, and if statements to build this application.

## Task

1. Create a Python script that:
   - Prompts the user to enter their age.
   - Checks if the entered age is a valid number (greater than 0).
   - Uses comparison operators to determine if the person is eligible to vote (age >= 18).
   - Displays a message indicating if the person can vote or not.

2. Implement additional logic to handle the following cases:
   - If the entered age is exactly 18, display a message saying "Congratulations on becoming eligible to vote!"
   - If the entered age is less than 18, display how many years are left until they can vote.
   - If the entered age is greater than 100, display a message saying "Wow! You've seen a lot in your lifetime!"

## Requirements

- Use comparison operators (`==`, `!=`, `>`, `<`, `<=`, `>=`) to compare the age.
- Use logical expressions (`and`, `or`, `not`) to handle multiple conditions.
- Apply Boolean math to determine the voting eligibility.
- Use if statements (`if`, `elif`, `else`) to handle different age ranges and conditions.
- Ensure your script handles invalid inputs gracefully.

## Example Output

```
Enter your age: 16
You are not eligible to vote. You can vote in 2 years.

Enter your age: 18
Congratulations on becoming eligible to vote!

Enter your age: 25
You are eligible to vote.

Enter your age: 105
Wow! You've seen a lot in your lifetime! You are eligible to vote.

Enter your age: -5
Invalid age. Please enter a valid age.
```

## Code Template

Here is a template to help you get started:

```python
def main():
    try:
        age = int(input("Enter your age: "))
        if age <= 0:
            print("Invalid age. Please enter a valid age.")
        elif age < 18:
            print(f"You are not eligible to vote. You can vote in {18 - age} years.")
        elif age == 18:
            print("Congratulations on becoming eligible to vote!")
        elif age > 100:
            print("Wow! You've seen a lot in your lifetime! You are eligible to vote.")
        else:
            print("You are eligible to vote.")
    except ValueError:
        print("Invalid input. Please enter a number.")

if __name__ == "__main__":
    main()
```

- **Step-by-step explanation:**
  - `try:` block attempts to convert the input to an integer.
  - The `if` statement checks if the age is less than or equal to 0 and prints an error message if true.
  - The `elif` statement checks if the age is less than 18 and prints how many years are left until voting eligibility.
  - Another `elif` statement checks if the age is exactly 18 and prints a congratulatory message.
  - An additional `elif` statement checks if the age is greater than 100 and prints a special message.
  - The final `else` statement covers the case where the age is between 19 and 100, indicating the person is eligible to vote.
  - The `except` block catches invalid inputs that are not numbers.

## Submission

Submit your Python script file (.py) with the implemented logic as per the requirements. Make sure your code is clean, well-commented, and handles edge cases properly.