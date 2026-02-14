# ✅ Data Integrity Validator

![Java](https://img.shields.io/badge/Java-17-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)
![Regex](https://img.shields.io/badge/Regex-Validation-blue)

A **Java console application** that validates user input with strict rules to ensure **data integrity**.  
Ideal for form validation, registration systems, or any scenario requiring clean, verified data before processing.

---

## 🎯 Features

- ✅ **Email validation** (regex: must contain @ and valid domain format).
- ✅ **Age validation** (18–99 years range).
- ✅ **Phone number validation** (7–15 digits, accepts +, spaces, and hyphens).
- ✅ **ZIP code validation** (exactly 5 digits).
- ✅ **Name validation** (cannot be empty or just spaces).
- ✅ **Clear, user-friendly error messages** for each invalid field.
- ✅ **Builder pattern** for safe object creation.
- ✅ Stores **only valid registrations** in memory.
- ✅ **List view** of all successfully registered participants.

---

## 🧠 Logic & Concepts Applied

- **Regular Expressions (Regex)** for pattern matching and validation.
- **Builder Pattern** (ensures objects are only created with valid data).
- **Exception handling** (`NumberFormatException`, input validation).
- **Collections** (`ArrayList<Registro>` for data storage).
- **Separation of concerns** (Validator class, Registro class, Main class).
- **User experience design** (clear error messages, input retry logic).

---

## 🏗️ Project Structure

data-integrity-validator/
├── src/
│   ├── Main.java # Application entry point with menu
│   ├── Validator.java # Static validation methods (regex)
│   └── Registro.java # Entity class with Builder pattern
├── screenshots/ # Screenshots for documentation
│   ├── menu.png
│   ├── validation-errors.png
│   ├── success.png
│   └── registrations-list.png
└── README.md # This file

---

## 📋 Validation Rules

| Field | Validation Rule | Example |
|-------|----------------|---------|
| **Name** | Cannot be empty or only spaces | "Juan Pérez" ✅ <br> "   " ❌ |
| **Email** | Must contain @ and valid format | "usuario@dominio.com" ✅ <br> "usuario.com" ❌ |
| **Age** | Integer between 18 and 99 | 25 ✅ <br> 15 ❌ <br> 100 ❌ |
| **Phone** | 7–15 digits, accepts +, spaces, hyphens | "+57 123 4567" ✅ <br> "abc" ❌ |
| **ZIP Code** | Exactly 5 digits | "12345" ✅ <br> "1234" ❌ <br> "ABCDE" ❌ |

---

## ▶️ How to Run

### Prerequisites
- Java JDK 17 or higher
- Any Java IDE (IntelliJ, VS Code, Eclipse) or terminal

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/data-integrity-validator.git
