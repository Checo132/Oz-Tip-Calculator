##  Project Overview

This project is a simple command-line Tip Calculator built with Python. It allows users to input the cost of a meal and their preferred tip percentage in familiar formats like `$50.00` and `15%`, then accurately calculates the amount to tip. The project reinforces core programming concepts such as user input handling, string manipulation, type conversion, and formatted output. Developed as part of a CS50 assignment, it emphasizes precision, usability, and adherence to real-world input expectations. In the United States, it’s customary to leave a tip for your server after dining in a restaurant, typically an amount equal to 15% or more of your meal’s cost.

---
### Key Features:

* Accepts user input for:
* Meal cost (e.g., `$50.00`)
* Tip percentage (e.g., `15%`)
* Cleans and converts input to numerical values:

>  * `"$50.00"` → `50.0`
> * `"15%"` → `0.15`
* Calculates and prints the exact tip to leave.
* Formats the output to two decimal places for currency precision.

---

###  Tech Stack:

* **Language:** Python 3
* **Tools Used:** VS Code for runnina and testing the program

---

###  Learning Objectives:

* Practice with `input()` and type conversion
* String parsing with `.replace()` and `.strip()`
* Basic arithmetic operations
* Output formatting using `f-strings`

---

###  Sample Run:
```
How much was the meal? $100.00  
What percentage would you like to tip? 20%  
Leave $20.00
```

---

### Set-up Instructions
---

### Working on VS Code Locally

### Step 1: Create the Project
1. Open **VS Code**.
2. Create a new folder called `tip`.
3. Inside that folder, create a file named `tip.py`.

### Step 2: Paste and Complete the Code
Paste this into `tip.py`:
```python
def main():
    dollars = dollars_to_float(input("How much was the meal? "))
    percent = percent_to_float(input("What percentage would you like to tip? "))
    tip = dollars * percent
    print(f"Leave ${tip:.2f}")


def dollars_to_float(d):
    return float(d.strip().replace("$", ""))


def percent_to_float(p):
    return float(p.strip().replace("%", "")) / 100


main()
```
---
### Step 3: Test the Program
Open a terminal in VS Code, navigate to the folder, and run:
```bash
python tip.py
```

Try with inputs like:
```
$50.00
15%
```

It should return: `Leave $7.50`

---

### Summary of Tools

| Task                      | Tool                | Required? |
| ------------------------- | ------------------- | ---------  |
| Writing code              | VS Code             | ✅ Yes     |
| Final testing             | VS Code             | ✅ Yes     |

---
