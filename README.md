# User Authentication System (CLI-Based)

This is a simple **User Authentication System** built using **Core Python** and **SQLite**. It allows users to register, login, and verify authentication using **JWT tokens**.

## Features
✅ **User Registration** – Stores usernames and hashed passwords in SQLite.
✅ **User Login** – Validates credentials and generates a JWT token.
✅ **Token Verification** – Checks if the JWT token is valid or expired.
✅ **CLI-Based Interface** – Simple command-line interaction.

## Prerequisites
Make sure you have **Python 3.6+** installed. If you don't have the required libraries, install them using:

```bash
pip install PyJWT
```

## How to Run

1. Clone or download the project.
2. Open a terminal and navigate to the project directory.
3. Run the script:

```bash
python user.py
```

## Usage

1. **Register a User**
   - Enter `1` to register a new user.
   - Provide a username and password.
   - The system stores the user with a **SHA-256 hashed password**.

2. **Login**
   - Enter `2` to log in.
   - Provide your username and password.
   - If credentials are valid, a **JWT token** is generated.

3. **Verify Token**
   - The token is verified for authenticity and expiration.

4. **Exit**
   - Enter `3` to exit the program.

## Checking the Database
You can check registered users in the SQLite database (`users.db`) using:

```bash
sqlite3 users.db
```
Inside the SQLite shell, run:

```sql
SELECT * FROM users;
```

## Future Improvements
- Add **password reset functionality**
- Implement **role-based access control**
- Create a **GUI-based version** using Tkinter or PyQt

## License
This project is open-source and free to use under the MIT License.

--

