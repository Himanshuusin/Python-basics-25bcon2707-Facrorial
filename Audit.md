# README Audit: `factorial.py`

**Code source:** [factorial.py on GitHub](https://github.com/Himanshuusin/Python-basics-25bcon2707-Facrorial/blob/main/factorial.py)

The audit below compares each README claim with the actual Python code.

| No. | README Claim                                                                  | Verdict           | Evidence from the Code                                                                                                                                                                                       |
| --: | ----------------------------------------------------------------------------- | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|   1 | The project contains a beginner-level Python program to calculate factorials. | **Supported**     | The program uses a `for` loop and multiplication to calculate the factorial, making it suitable for beginners.                                                                                               |
|   2 | The program calculates the factorial of a non-negative integer.               | **Supported**     | `n = int(input("Enter a number: "))` accepts an integer, and `for i in range(1, n + 1):` calculates the factorial for non-negative inputs. However, the program does not validate or reject negative inputs. |
|   3 | Python must be installed on the computer to run the program.                  | **Supported**     | The file contains Python code that must be executed by a Python interpreter.                                                                                                                                 |
|   4 | The user should open a terminal in the folder containing `factorial.py`.      | **Supported**     | The program is a standalone Python script, so it can be executed from a terminal when Python is installed and the file is accessible.                                                                        |
|   5 | The command `python factorial.py` runs the program.                           | **Supported**     | The file contains executable Python statements and requires no additional libraries. The command works where `python` is configured to invoke the Python interpreter.                                        |
Supported — The code uses input("Enter a number: ") to take user input and int() to convert it into an integer. However, the program does not explicitly validate whether the integer is non-negative.                                                                     |
|   7 | The program demonstrates Python variables.                                    | **Supported**     | The variables `n`, `factorial`, and `i` are used to store the input, factorial result, and loop counter.                                                                                                     |
|   8 | The program demonstrates how to take user input.                              | **Supported**     | The statement `n = int(input("Enter a number: "))` reads input and converts it to an integer.                                                                                                                |
|   9 | The program demonstrates loops and multiplication.                            | **Supported**     | The `for` loop iterates through `range(1, n + 1)`, while `factorial = factorial * i` multiplies the numbers to calculate the result.                                                                         |
|  10 | The program demonstrates displaying output using `print()`.                   | **Supported**     | The statement `print("Factorial =", factorial)` displays the calculated result.                                                                                                                              |

## Audit Summary

* **Total claims audited:** 10
* **Supported:** 9
* **Not Supported:** 1

**Main finding:** The README accurately describes the program's basic functionality and learning objectives. However, the claim that the program prompts users to enter a *non-negative integer* is not fully supported because the code does not validate the input.

**Additional observation:** Negative integers are accepted by `int(input(...))`, but the loop does not execute for negative values. As a result, the program prints `Factorial = 1` instead of reporting invalid input.

**Conclusion:** The README is mostly accurate, with one claim requiring attention regarding input validation. No README changes have been made.
