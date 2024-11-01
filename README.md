# 🔐 Password Generator Project

Welcome to the **PyPassword Generator!** This project is a Python-based random password generator that allows users to create strong and customizable passwords with ease. You can specify the number of letters, symbols, and numbers to include in your password, and the program will generate a unique password that meets your criteria.

---

## 📜 Features

- **Randomized Passwords**: Generate secure, randomized passwords that combine letters, numbers, and symbols.
- **Customizable Length**: Choose the number of letters, numbers, and symbols you want in your password.
- **Simple and Interactive**: User-friendly input prompts guide you through creating a custom password.

---

## 🛠️ How It Works

The program uses the `random` library to select random characters from predefined lists of letters, numbers, and symbols. The user enters the desired number of each character type, and the generator outputs a password string containing the specified components.

### Code Overview

```python
import random

letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z',
           'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

print("Welcome to the PyPassword Generator!")
nr_letters= int(input("How many letters would you like in your password?\n"))
nr_symbols = int(input("How many symbols would you like?\n"))
nr_numbers = int(input("How many numbers would you like?\n"))

password = ""

for char in range(0, nr_letters):
    password += random.choice(letters)

for char in range(0, nr_symbols):
    password += random.choice(symbols)

for char in range(0, nr_numbers):
    password += random.choice(numbers)

print(password)
```

## 📋 Usage Instructions
1. Clone the Repository:
```bash
git clone https://github.com/your-username/password-generator
cd password-generator
```
2. Run the Script: Run the script in a Python environment:
```bash
python password_generator.py
```
3. Follow the Prompts:
  Enter the number of letters, symbols, and numbers you want in your password.
  The program will display your customized, secure password.

## ⚙️ Customization
  You can easily modify the lists of letters, numbers, and symbols to include or exclude specific characters based on your security needs or preferences.

## Example Output
```bash
Welcome to the PyPassword Generator!
How many letters would you like in your password?
5
How many symbols would you like?
3
How many numbers would you like?
2
Your generated password is: A$3b!7Cd@
```

## 📝 License
  This project is licensed under the MIT License. See the LICENSE file for details.


Happy password generating! 💪🔒

