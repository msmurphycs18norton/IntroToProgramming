### Homework Assignment: Create a Simple Text-Based Game

#### Objective:
Create a simple text-based game using loops in Python. The game will involve the user guessing a secret number.

#### Requirements:

1. **Understand and Use While Loops**: The game should run until the user guesses the correct number.
2. **Use If Statements within While Loops**: Provide feedback to the user if the guess is too high or too low.
3. **Understand Loop Syntax**: Properly structure while loops and if statements.
4. **Use For Loops for Iteration**: Allow the user to play multiple rounds of the game, keeping track of the number of attempts in each round.
5. **Use the `range()` Function**: Utilize `range()` to limit the number of attempts in each round.
6. **Iterate Through Strings**: Display a congratulatory message character by character when the user wins.
7. **Iterate Through Lists**: Display a list of the user's guesses after each round.
8. **Circuit Breakers**: Use `break` to exit the loop when the user guesses correctly and `continue` to prompt the user to guess again if their guess is invalid.
9. **REPL Structure**: Use a REPL-like structure for the game where the user is continuously prompted for input until they decide to quit.

#### Instructions:

1. **Define the Main Loop**: Create a `while` loop that continues to run until the user decides to quit the game.
2. **Random Number Generation**: Generate a random number between 1 and 100 at the start of each round.
3. **User Guessing Loop**: Inside the main loop, create another `while` loop to handle user guesses.
4. **Input and Validation**: Prompt the user to guess the number and validate the input.
5. **Feedback**: Provide feedback to the user if the guess is too high or too low.
6. **Limit Attempts**: Allow the user a maximum of 10 attempts per round using a `for` loop and the `range()` function.
7. **Track and Display Guesses**: Use a list to track the user's guesses and display them after each round.
8. **Congratulatory Message**: When the user guesses the correct number, display a congratulatory message character by character.
9. **Play Again Option**: After each round, ask the user if they want to play again or quit.

#### Example Code Structure:

```python
import random

def main():
    while True:
        print("Welcome to the Number Guessing Game!")
        secret_number = random.randint(1, 100)
        attempts = 10
        guesses = []

        print("You have 10 attempts to guess the secret number between 1 and 100.")

        for attempt in range(attempts):
            while True:
                try:
                    guess = int(input("Enter your guess: "))
                    break
                except ValueError:
                    print("Invalid input. Please enter a number.")

            guesses.append(guess)

            if guess == secret_number:
                print("Congratulations! You guessed the correct number.")
                for char in "Well Done! You are a genius!":
                    print(char, end="")
                print("\n")
                break
            elif guess < secret_number:
                print("Too low!")
            else:
                print("Too high!")

            if attempt == attempts - 1:
                print("Sorry, you've used all your attempts. The secret number was:", secret_number)

        print("Your guesses: ", guesses)

        play_again = input("Do you want to play again? (yes/no): ").lower()
        if play_again != 'yes':
            print("Thank you for playing! Goodbye!")
            break

if __name__ == "__main__":
    main()
```

#### Submission:

- Ensure your code is well-commented to explain each part.
- Submit your `.py` file with the implemented game.
- Be prepared to explain how you used loops, conditionals, and other concepts covered in class.