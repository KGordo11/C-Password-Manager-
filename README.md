# C++ Password Manager

A secure, password manager built in C++. Designed as a command-line application for learning object-oriented design, file I/O, encryption, and user interaction.

---

## Project Summary

This project simulates a fully offline password manager where users can:

- Secure their data with a master password
- Add, view, delete, and search login credentials
- Automatically save/load encrypted data from files
- Track password creation dates and expiration status

> Built to reflect core software engineering principles taught in CS215 and CS216.

---

## Features

### Master Password Login
- First-time users are prompted to create a master password
- All future access requires this password
- Option to reset the password while keeping existing data

### Encrypted Storage
- Entries are encrypted using a basic XOR cipher before being saved
- Prevents raw exposure of usernames, passwords, and websites

### Entry Management
- Add new entries (website, username, password)
- Auto-records the timestamp for creation
- View entries in a clean, formatted table
- Mark entries as "Expired" after 180 days

### Search Functionality
- Search by **website** or **username**
- Friendly prompts and formatted output
- Handles invalid input with error correction

### Auto-Save and Auto-Load
- Automatically loads saved data at startup
- Automatically saves after adding or deleting entries
- Users never have to remember to save manually

---

## Key Concepts & Skills Demonstrated

| Concept                        | Demonstrated In                         |
|-------------------------------|------------------------------------------|
| Object-Oriented Programming   | `PasswordManager` class and `Entry` struct |
| File I/O                      | `ifstream` and `ofstream` for data handling |
| Encryption & Security         | XOR cipher, master password protection    |
| User Interaction              | Menus, prompts, error handling, input validation |
| Time Handling                 | Timestamping with `ctime`, `mktime`, and `difftime` |
| Input Validation              | Graceful handling of invalid input using `cin.fail()` and `limits` |
| Code Organization             | Header/source split, meaningful comments, structured logic |

---

## Technologies Used

- Language: C++
- IDE: Visual Studio Code 
- Standard: C++11/C++17
- Compiler: g++



