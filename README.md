# Countdown Solver

This Python script solves the arithmetic game "Countdown" where the goal is to find a mathematical expression using a set of six numbers and four arithmetic operations (addition, subtraction, multiplication, and division) to reach a target number.

## Usage

```python
python countdown_solver.py
```
Upon running the script, you will be prompted to input the six numbers (separated by spaces) and the target number. The solver will find and display the unique solutions that reach the target number or the closest solution if no exact solutions are found.

## Example

Input:
```Enter the six numbers, separated by spaces: 1 2 3 4 5 6
Enter the target number: 42
```
Output:
```The following unique solutions were found: 
6*4*2-3*5+1
6*4*2-5*3+1
6*4*2+1-3*5
6*4*2+1-5*3
```
## How It Works

The solver uses the itertools library to generate permutations of the input numbers and combinations of the arithmetic operators. It then evaluates each expression to see if the target number is reached. The solver also accounts for division by zero and non-integer division results.
Functions

  *  `evaluate_expression(exp, target)`: Evaluates a given expression and checks if the result is equal to the target. If it is, the function returns the result; otherwise, it returns None.
  *  `countdown()`: Main function that takes user input, generates expressions, and finds solutions. Returns the unique solutions, closest solution, or a message indicating that no solution was found.

## Dependencies

  *  Python 3.x
  *  itertools
