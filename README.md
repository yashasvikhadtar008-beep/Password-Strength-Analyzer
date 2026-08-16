# 🔐 Password Strength Analyzer

A simple and beginner-friendly **Python Password Strength Analyzer** that checks whether a password satisfies important security requirements. The program evaluates the password based on its length, uppercase and lowercase letters, numbers, special characters, and spaces.

This project was created to practice fundamental Python concepts such as **functions, loops, conditional statements, string methods, Boolean values, and user input**.

## 📌 Features

* Checks whether the password contains at least **8 characters**
* Checks for **uppercase letters**
* Checks for **lowercase letters**
* Checks for **digits/numbers**
* Checks for **special characters**
* Checks that the password does **not contain spaces**
* Gives a clear result based on the password criteria

## 🛠️ Technologies Used

* **Python 3**
* No external libraries are required.

## 📂 Project Structure

```text
Password-Strength-Analyzer/
│
├── password checker.py
└── README.md
```

## ⚙️ How the Code Works

The program is divided into simple steps:

### 1. Define the Function

The `check_password()` function is created to analyze the password.

```python
def check_password(password):
```

The password entered by the user is passed to this function.

### 2. Check Password Length

```python
length_check = len(password) >= 8
```

The `len()` function counts the number of characters in the password.

The condition returns `True` if the password contains **8 or more characters**.

### 3. Create Check Variables

The program creates Boolean variables for different requirements:

```python
uppercase_check = False
lowercase_check = False
digit_check = False
special_check = False
```

Initially, all values are set to `False`. They become `True` when the required character is found.

### 4. Check Every Character

A `for` loop is used to examine each character of the password:

```python
for character in password:
```

The loop goes through the password one character at a time.

### 5. Check Uppercase and Lowercase Letters

Python string methods are used to identify letters:

```python
if character.isupper():
    uppercase_check = True

elif character.islower():
    lowercase_check = True
```

* `isupper()` checks for uppercase letters such as `A`, `B`, `C`.
* `islower()` checks for lowercase letters such as `a`, `b`, `c`.

### 6. Check for Digits

The program checks whether a character is a number:

```python
if character.isdigit():
    digit_check = True
```

For example: `1`, `5`, `8`, `9`.

### 7. Check for Special Characters

The program checks whether the password contains a special character such as:

```text
@ # $ % ! *
```

This helps make the password more complex.

### 8. Check for Spaces

The program also checks that the password does not contain a space:

```python
space_check = " " not in password
```

If there is no space in the password, the result is `True`.

### 9. Return the Result

After checking all the requirements, the function returns the results so that the main program can determine whether the password meets the required conditions.

## ▶️ How to Run

### Step 1: Install Python

Make sure Python 3 is installed on your computer.

### Step 2: Clone the Repository

```bash
git clone https://github.com/yashasvikhadtar008-beep/Password-Strength-Analyzer.git
```

### Step 3: Open the Project

Open the project folder in **VS Code** or any Python-supported editor.

### Step 4: Run the Program

```bash
python "password checker.py"
```

Enter a password when prompted and the program will analyze it.

## 💡 Python Concepts Used

This project demonstrates the following Python concepts:

* Functions
* `if-elif-else` conditional statements
* `for` loops
* Boolean variables
* User input
* String methods
* Comparison operators
* Logical operators
* `len()` function
* `return` statement

## 🎯 Learning Objective

The main purpose of this project is to understand how basic Python concepts can be combined to create a practical application. It also provides an introduction to the idea of **password security and validation**.

## 🚀 Future Improvements

Some possible improvements for future versions include:

* Adding different strength levels such as **Weak, Medium, and Strong**
* Providing a score for each password
* Adding a password generator
* Creating a graphical user interface
* Checking passwords against commonly used passwords
* Improving the password validation rules

## 👩‍💻 Author

**Yashasvi Khadtar**

---

⭐ If you find this project useful, consider giving the repository a star!
