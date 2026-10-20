# Password Strength Checker

**DecodeLabs Industrial Training Kit - Cyber Security, Project 1 (Batch 2026)**

A Python command-line tool that rates a password as **Weak**, **Medium** or **Strong**.

## Features
- Length check (fewer than 8 characters is an immediate fail)
- Checks for uppercase letters, lowercase letters, numbers and symbols
- Rejects common / leaked passwords
- Gives tips on how to improve the password
- Hidden input using `getpass` so the password is not shown on screen
- Single linear scan, so validation time grows linearly with password length

## How to run
```bash
python password_checker.py
```
Requires Python 3.9+. No external libraries needed.

## Rating rules
| Condition | Result |
|---|---|
| Less than 8 characters | Weak |
| In the common-password list | Weak |
| Score 5 or more | Strong |
| Score 3 or 4 | Medium |
| Score below 3 | Weak |

Score = number of character types used (upper, lower, digit, symbol) + 1 bonus point if length is 12 or more.

## Example
```
Enter password:
Strength: Medium
  - Add a symbol (e.g. ! @ # $ %).
  - Use 12+ characters for extra strength.
```

## Skills demonstrated
String handling, conditional logic, input validation, security basics.

## Author
Your Name -Aditya Dubey, DecodeLabs Cyber Security Intern, Batch 2026
