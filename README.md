# Fun Fact

> **A bcrypt-hashed password with 10 salt rounds would take roughly 20,000 to 30,000 years to crack on a typical personal computer — basically stronger than a grandma’s secret cookie recipe!**


# Secrets Authentication App

A simple Node.js web application that allows users to register and log in securely. After logging in, users can view a secret message. Passwords are securely hashed using bcrypt and stored in a PostgreSQL database.

## Features
- User registration with email and password
- Secure password hashing with bcrypt
- User login with password verification
- PostgreSQL database integration
- EJS templating and Bootstrap styling

## Setup
1. **Clone the repository**
2. **Install dependencies:**
   ```bash
   npm install
   ```
3. **Configure PostgreSQL:**
   - Create a database named `secrets`.
   - Create a `users` table with columns `email` (text) and `password` (text).
4. **Update database credentials** in `index.js` if needed.
5. **Start the server:**
   ```bash
   node index.js
   ```
6. **Visit** `http://localhost:3000` in your browser.

## Usage
- Register a new account with your email and password.
- Log in to view the secret message.

## Dependencies
- express
- ejs
- body-parser
- pg
- bcrypt

---
This project mainly focuses on the procedure of how the passwords are hashed and to what extent it could be pushed apart from salting to just 10 rounds.
