# 🔐 Password Generator

A simple yet powerful command-line password generator built with Python. Instantly create strong, customizable passwords with full control over character types and length.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Sample Output](#sample-output)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## 🧠 Overview

This is a lightweight Python CLI tool that generates secure random passwords based on user preferences. Users can choose the password length and select which character types to include — lowercase, uppercase, digits, and/or symbols.

---

## ✨ Features

- ✅ Customizable password length
- ✅ Choose from 4 character types: lowercase, uppercase, digits, symbols
- ✅ Guarantees at least one character from each selected type
- ✅ Randomly shuffled output for true randomness
- ✅ Input validation with friendly error messages
- ✅ No external dependencies — uses Python standard library only

---

## 📁 Project Structure

```
password-generator/
│
├── password_generator.py   # Main script
└── README.md               # Project documentation
```

---

## ⚙️ Installation

### Prerequisites

- **Python 3.x** — No additional packages required

### 1. Clone the repository

```bash
git clone https://github.com/your-username/password-generator.git
cd password-generator
```

### 2. Run directly — no installation needed!

```bash
python password_generator.py
```

---

## 🚀 Usage

Run the script and follow the interactive prompts:

```bash
python password_generator.py
```

You will be asked:
1. **Password length** — must be at least 4
2. **Include lowercase letters?** (y/n)
3. **Include uppercase letters?** (y/n)
4. **Include numbers?** (y/n)
5. **Include symbols?** (y/n)

> ⚠️ At least one character type must be selected, otherwise the tool will show an error.

---

## 🔍 How It Works

1. User provides a desired password length and selects character types
2. The generator **guarantees** at least one character from each selected type is included
3. Remaining characters are filled randomly from the combined character pool
4. The final password is **shuffled** to eliminate any predictable patterns
5. The password is displayed in the terminal

### Character Sets Used

| Type | Characters |
|---|---|
| Lowercase | `a-z` |
| Uppercase | `A-Z` |
| Digits | `0-9` |
| Symbols | `! " # $ % & ' ( ) * + , - . / : ; < = > ? @ [ \ ] ^ _ \` { \| } ~` |

---

## 📋 Sample Output

```
Enter password length: 12

Select character types (y/n):
Include lowercase letters? (y/n): y
Include uppercase letters? (y/n): y
Include numbers? (y/n): y
Include symbols? (y/n): n

Generated password: aB3kLm9XqR2p
```

```
Enter password length: 3

Password length should be at least 4.
```

```
Enter password length: 16

Select character types (y/n):
Include lowercase letters? (y/n): n
Include uppercase letters? (y/n): n
Include numbers? (y/n): n
Include symbols? (y/n): n

Error: you must select at least one character type.
```

---

## 🔮 Future Improvements

- [ ] Add option to generate multiple passwords at once
- [ ] Exclude ambiguous characters (e.g., `0`, `O`, `l`, `1`)
- [ ] Add password strength indicator (Weak / Medium / Strong)
- [ ] Save generated passwords to a file
- [ ] Build a GUI version using Tkinter or a web app using Flask
- [ ] Add a `--cli` argument mode for scripting use (e.g., `python generator.py --length 16 --all`)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Your Name**  
GitHub: [Mousam-gift](https://github.com/Mousam-gift)

---

⭐ If you found this useful, consider giving it a star!
