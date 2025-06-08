
# 📘 PostgreSQL Basics – Quick Guide

Beginner-friendly PostgreSQL reference with common database and table commands. Useful for quick review while learning.

---

## 📂 DATABASE COMMANDS

### 🔍 List All Databases
```sql
\l
```
Shows all databases available on your PostgreSQL server.

---

### 🆕 Create a Database
```sql
CREATE DATABASE mydb;
```
Creates a new database named `mydb`.

---

### 🔄 Connect/Switch to a Database
```sql
\c mydb
```
Connects to the specified database (`mydb`) for performing operations.

---

### ❌ Drop/Delete a Database
```sql
DROP DATABASE mydb;
```
Permanently deletes the database `mydb`.

---

## 🧱 TABLE COMMANDS

### 🆕 Create a Table
```sql
CREATE TABLE students (
  id SERIAL PRIMARY KEY,
  name TEXT,
  age INT
);
```
Creates a `students` table with `id`, `name`, and `age` columns.

---

### 📋 Show Tables
```sql
\dt
```
Displays all tables in the currently connected database.

---

## ✍️ CRUD OPERATIONS

### 📥 INSERT Data
```sql
INSERT INTO students (name, age) VALUES ('Sharwan', 20);
```
Adds a new row to the `students` table.

---

### ➕ Multi Data Entry
```sql
INSERT INTO students (name, age) VALUES 
('Ram', 21),
('Sita', 22),
('Hari', 23);
```
Adds multiple records in one command.

---

### ✏️ Short Form Insert (all columns)
```sql
INSERT INTO students VALUES (1, 'Sharwan', 20);
```
Insert data directly by values if you know the order of columns.

---

### 📖 READ/View Data
```sql
SELECT * FROM students;
```
Displays all rows from the `students` table.

---

### 🛠️ UPDATE Data
```sql
UPDATE students SET age = 25 WHERE name = 'Sharwan';
```
Updates the `age` of the student where `name` is 'Sharwan'.

---

### 🗑️ DELETE Data
```sql
DELETE FROM students WHERE name = 'Ram';
```
Deletes the row where `name` is 'Ram'.

---

## 🚀 TIPS
- Use `\?` to list all `psql` meta-commands.
- Use `\q` to quit the PostgreSQL shell.

---

## 📌 Author
**Sharwan Jung Kunwar**  
Learning PostgreSQL, one command at a time.
