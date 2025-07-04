# 📚 Library Management System (MySQL-Based)

A simple SQL project to manage a library’s books, authors, members, and borrow/return records using **MySQL**. This project demonstrates how to design a normalized relational database with basic to intermediate SQL operations and apply security principles like **PoLP (Principle of Least Privilege)**.

---

## 🚀 Features

- Create and manage authors, books, members
- Track which member borrowed which book and when
- Show available books and overdue records
- List books by genre, author, or popularity
- Apply **PoLP** by assigning restricted user access (admin vs member)
- Perform real-world queries using JOIN, GROUP BY, WHERE, etc.

---

## 🛠️ Technologies Used

- 💾 **MySQL** – Database engine
- 🖥️ **XAMPP/phpMyAdmin** (or MySQL CLI) – Query execution
- 🧱 SQL operations – DDL, DML, Joins, Aggregates

---

## 📁 Database Design (Tables)

| Table      | Description                          |
|------------|--------------------------------------|
| `Authors`  | Stores author info (first & last name) |
| `Books`    | Book details, linked to authors       |
| `Members`  | Registered users of the library       |
| `Borrowing`| Tracks book borrow/return activity    |

---

## ⚙️ How to Run

1. Open MySQL or phpMyAdmin.
2. Run the full SQL script in this repo (`librarymanagement.sql`).
3. Execute the queries listed in `queries.sql` to explore data.

---

## 🔐 Principle of Least Privilege (PoLP)

Two example users created:

- 🔑 `librarian` – Full access (`SELECT`, `INSERT`, `UPDATE`, `DELETE`)
- 🔒 `memberuser` – Read-only access (`SELECT` on `books`, `authors`)

This helps simulate real-world security where regular users can’t modify data.

---

## 📊 Sample Queries Included

- Books borrowed by a specific user
- Most borrowed books
- Members who haven't borrowed any book
- Average books borrowed per member
- Overdue books (borrowed over 30 days ago)
- Books by specific author or genre
- Most popular genre

---

## 🎯 Learning Outcomes

- Hands-on practice with relational database design
- Use of foreign keys, normalization
- Writing effective SQL queries for real-world needs
- Understanding of user roles and access control using MySQL

---

## ✅ Future Enhancements

- Add frontend using HTML/CSS/React
- Add fine calculation logic for late returns
- Implement login system using PHP/Python
- Generate PDF reports for borrowing history


