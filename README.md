# ChatApplication
# 📱 QuickChat Console Application

QuickChat is a simple Java-based console chat simulation that allows users to register, log in, and send text messages to other registered users. It supports message storage, basic password security, and input validation, making it a great learning project for Java developers exploring object-oriented design and console-based user interaction.

---

## 🚀 Features

- ✅ User Registration with:
  - Username validation (3–15 characters, alphanumeric or underscore)
  - South African phone number validation (`+27`, `27`, or `0` prefix)
  - Password complexity check (minimum 8 characters with uppercase, lowercase, and digits)

- 🔐 Secure Login for registered users

- 💬 Send messages to other users
  - Validates recipient phone number
  - Limits message length to 250 characters
  - Automatically generates unique message IDs and hashes
  - Options to send, discard, or store messages

- 📄 Store unsent messages in a JSON-like format file (`stored_messages.json`)

- 📜 View recently sent messages during the session

- 🎯 Tracks total messages sent

---

## 🧠 Concepts Used

- Object-Oriented Programming (OOP)
- Java Collections (e.g., `ArrayList`)
- Input validation with regular expressions
- Error handling with `try-catch`
- Message hashing and ID generation
- File writing using `FileWriter`
- Basic GUI interaction using `JOptionPane`

---

## 🛠️ Classes Overview

### `ChatApplication`
The main driver class containing the program loop, user interaction, and core functionality like sending messages and managing users.

### `User`
Handles user data such as username, phone number, password, and received messages.

### `Message`
Represents a message with sender, recipient, content, and status flags (sent, received, read). Also includes utilities like message hashing and printing.

---

## 📝 Message Hash Example

The message hash format:

---

## 📂 Output File

Stored messages are saved in a file named `stored_messages.json` in a simple JSON-style format, allowing future extension for proper JSON handling or integration with APIs or databases.

---

## 📦 Requirements

- Java 8 or later
- No external dependencies

---

## ▶️ Running the Application

1. Compile the Java files:
```bash
javac ChatApplication.java
java ChatApplication
+27821234567
27821234567
0821234567

