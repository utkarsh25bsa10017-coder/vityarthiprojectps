1. The Functions (Core Math)
def add(x, y): Returns the sum of x and y.
def subtract(x, y): Returns the difference of x and y.
def multiply(x, y): Returns the product of x and y.
def divide(x, y): Returns the quotient of x and y. It includes an important check: if y is 0, it returns the error message "Error! Division by zero." instead of crashing.

2. The calculator() Function (User Interaction)
This function manages the calculator's entire flow:
Initial Setup: Prints a title and a menu listing the four options (1, 2, 3, 4) and the option to quit ('q').
Main Loop (while True): The program enters a loop to keep running until the user decides to exit.
Quit Check: It checks if the user inputs 'q'. If so, it prints "Exiting calculator. Goodbye!" and stops the loop.
Operation Selection: If the choice is 1, 2, 3, or 4:
Input Numbers: It asks the user to enter two numbers. These are converted to floating-point numbers (allowing decimals).
Input Error Handling (try/except): It is wrapped in a 'try...except ValueError' block. If the user types non-numeric text (like "hello"), it catches the error, prints an error message, and restarts the loop.
Execution: Based on the choice, it calls the corresponding function (add, subtract, multiply, or divide) and prints the result.
Division Check: Specifically for choice 4 (divide), it checks the result for the "Error! Division by zero." string before printing to avoid displaying a calculation if the error occurred.
Invalid Input: If the choice is not a valid option or 'q', it prints "Invalid Input" and prompts again.

3. Program Start
if name == "main": This standard line makes sure the calculator() function is called and the program starts only when the script file is run directly.
