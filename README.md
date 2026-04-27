# OnlineBankingSystem
# 🏦 Online Banking System (Java + MySQL)

## 📌 Overview

This project is a console-based **Online Banking System** developed using Java and MySQL. It simulates real-world banking operations such as user registration, login, account management, and financial transactions.

The system is designed using Object-Oriented Programming principles and demonstrates backend development with database integration.

---

## 🚀 Features

* User Registration & Login (Authentication)
* Account Creation
* Deposit & Withdraw Money
* Balance Inquiry
* Secure Database Integration using JDBC
* Menu-driven Console Application

---

## 🧠 Tech Stack

* **Language:** Java
* **Database:** MySQL
* **Concepts:** OOP, JDBC, DBMS

---

## ⚙️ Project Structure

```text
OnlineBankingSystem/
│── Main.java
│── DBConnection.java
│── User.java
│── Account.java
│── BankingService.java
│── schema.sql
```

---

## 🗄️ Database Setup

1. Open MySQL
2. Run the following script:

```sql
CREATE DATABASE bank_db;
USE bank_db;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50),
    password VARCHAR(50)
);

CREATE TABLE accounts (
    id INT AUTO_INCREMENT PRIMARY KEY,
    user_id INT,
    balance DOUBLE,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/online-banking-system.git
```

2. Navigate to the project folder:

```bash
cd online-banking-system
```

3. Update database credentials in `DBConnection.java`

4. Compile the code:

```bash
javac Main.java
```

5. Run the program:

```bash
java Main
```

---

## 🧪 Example

```text
1. Register
2. Login
3. Exit

Enter choice: 1
Enter name: user
Enter password: 123

Login Successful!

1. Deposit
2. Withdraw
3. Check Balance
```

---

## 🌍 Real-World Applications

* Banking systems
* Financial transaction systems
* Backend service applications
* Account management systems

---

## 📈 Key Learnings

* Database integration using JDBC
* Implementation of OOP concepts
* Handling real-world transaction logic
* Writing efficient backend code

---

## 🔮 Future Enhancements

* Fund Transfer between accounts
* Transaction history tracking
* Password encryption
* GUI / Web-based interface

---

## 🤝 Contributing

Feel free to fork this repository and enhance the project.

---

## 📬 Contact

For queries or collaboration, connect via GitHub or LinkedIn.

---

⭐ If you found this project useful, give it a star!
