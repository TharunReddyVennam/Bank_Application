# 🏦 Simple Banking Web Application

## 📌 Objective

This project is a **minimalist web-based banking system** designed using Python and Flask. It aims to simulate core banking functionalities such as:

* Creating bank accounts
* Depositing and withdrawing money
* Checking account balances
* Viewing transaction history

It is ideal for educational purposes, showcasing CRUD operations with a relational database and a basic user interface without the need for frontend frameworks.

---

## 🛠️ Tech Stack

* **Backend**: Python (Flask)
* **Database**: SQLite (lightweight, serverless SQL database)
* **Frontend**: HTML, CSS (rendered using Flask's `render_template_string`)
* **Web Server**: Flask's built-in development server

---

## 🧾 Key Features / Steps Included

### 1. **Database Initialization**

* Automatically creates `accounts` and `transactions` tables in `bank.db`.

### 2. **Routes and Functionalities**

* `/create`: Create new user account with name and initial balance.
* `/balance`: Enter account ID to view current balance.
* `/deposit`: Deposit money to a specified account.
* `/withdraw`: Withdraw money (with balance check).
* `/statement`: View transaction history for an account.

### 3. **Transaction Logging**

* All deposits and withdrawals are logged with a timestamp.

### 4. **Simple UI**

* Built-in layout with HTML + CSS, rendered directly from strings.

---

## 🔍 Key Insights

* Demonstrates use of **Flask routing**, **form handling**, and **template rendering**.
* Efficient use of **SQLite** for data persistence without external dependencies.
* Application logic is kept clean and organized for readability.
* Good practice of **handling user input**, **validating accounts**, and **logging financial operations**.

---

## 🚀 How to Run the Application

### 🐳 Run with Docker

#### 1. Build and Run

```bash
# Using Docker CLI
docker build -t banking-app .
docker run -p 5005:5005 banking-app
```

#### 2. Access the App

Go to `http://localhost:5005` in your browser.
