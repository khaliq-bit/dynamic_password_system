# Dynamic Password Authentication System
-----------------------------------------------------------------------------------------
## NOTE:

This project uses the RockYou common password list for validation.  
Due to size constraints, it is not included in the repository.

Download it from the following source:
https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt

Place the file in the project root directory as `rockyou.txt`.
-----------------------------------------------------------------------------------------

This project is a Flask-based web application that demonstrates a secure authentication system with dynamic password generation, password validation, and account recovery features.  
It combines password strength checking with multiple dynamic update algorithms to improve security.

## Features
- User registration with:
  - Strong password validation
  - Common password detection (via rocku_dynamic_passwd)
  - Security questions for recovery
- Dynamic passwords that change:
  - Every minute
  - Every hour
  - Every day of the week
- User login with dynamic password validation
- Password reset via security questions
- Account management (signup, login, logout, reset)
- Lock and unlock API (simulated IoT device control)
- SQLite database for user storage
- Session management for secure logins

## Tech Stack
- Backend: Flask (Python)
- Database: SQLite
- Frontend: HTML templates (Jinja2)
- Security: SHA-256 hashing, session handling, dynamic password algorithm

## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/khaliq-bit/dynamic-password-auth.git
cd dynamic-password-auth

2. Install dependencies
pip install flask requests

3. Run the server
python flask_server.py

The app will start on:
http://127.0.0.1:5000

#NOTE
run the database.py file to create a database file in the project repo , next run the flask_app to start the project


