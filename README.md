# C# Console Password Manager

## Overview
This is a simple yet secure **password manager** written in C#.  
It allows you to:
- **Generate random passwords** with customizable length and complexity.
- **Store passwords securely** in a local SQLite database.
- **Encrypt and decrypt** stored passwords using AES encryption.
- **Retrieve, update, and delete** existing passwords.
- **Protect access** with a master login system.

---

## Features
1. **Random Password Generator**
   - Customizable length (6–32 characters).
   - Choose whether to include uppercase, lowercase, numbers, and/or symbols.

2. **Secure Storage**
   - Stores credentials (Website, Username, Password) in a local SQLite database (`passwords.db`).
   - Passwords are encrypted with AES-256 before saving.

3. **Master Login System**
   - Requires creating a master username and password on first run.
   - Master credentials are hashed using SHA-256 for secure authentication.

4. **Password Management**
   - Add new passwords.
   - Retrieve and view stored passwords (decrypted in console).
   - Update existing passwords.
   - Delete credentials for specific websites/usernames.

---

## Requirements
- **.NET 6.0+** (or compatible C# compiler/runtime).
- **System.Data.SQLite** NuGet package.

Install SQLite package:
```bash
dotnet add package System.Data.SQLite
```
Notes*
This was a group project, but the part that I focused on was the SQL database intagration.
