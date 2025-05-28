# 🔐 Secure Data Encryption System

A Streamlit-based application for securely storing and retrieving user data using encryption and password protection. It also includes an admin login system for access control and security management.

---

## 📌 Features

- 🔒 AES Encryption (via `cryptography` library)
- 🔑 Passkey-protected data storage
- 🔓 Admin login system (with login attempts limit)
- 📁 Persistent data storage using JSON files
- 📊 Simple, user-friendly Streamlit interface
- 🚫 Lockout mechanism after 3 failed decryption attempts
- ⚡ UV-powered virtual environment for dependency management

---

## 🛠️ Tech Stack

- **Python 3.7+**
- **Streamlit** – For UI and frontend
- **Cryptography** – For secure data encryption/decryption
- **JSON** – For data persistence (can be replaced by a DB later)
-  **Fernet** – For symmetric encryption (part of cryptography)
-  **UV** – Modern Python package installer and project manager

---

## 🧰 Installation & Setup

###  📥 Clone the Repository

```bash
git clone https://github.com/your-username/secure-data-encryption.git
cd secure-data-encryption

```

---
### 🛠️ Alternative Setup (From Scratch)

###  ⚡ Set Up UV Virtual Environment
#### 1. Install UV (if not already installed)
```bash
pip install uv
```

#### 2. Create folder through uv
```bash
uv init foldername
```
This will create these files automatically gitignor , python-version , main.py , readme.md , pyproject.toml (	Defines your project, dependencies, and build system. Required for modern Python packaging..)

#### 3. Create virtual environment
```bash
uv venv venv
```
This will create .venv file automatically
#### 4. Activate environment (Windows)
```bash
.\venv\Scripts\activate
```

#### 5. Install dependencies
```bash
uv pip install streamlit cryptography
```
This will create a uv.loc file that tracks your project's dependencies and environment configuration.

#### 6. Create JSON files manually
- **secure-data.json**  - tracks  user id , encrypted data , passkey .
- **attempts.json** -  tracks failed attempts per user.
 
#### 7.  🚀 Run the Application
```bash
streamlit run main.py
```



