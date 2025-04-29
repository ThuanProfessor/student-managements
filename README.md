# 🎓 Student Management System

A robust and extensible web-based student management application built with **Python Flask** and **MySQL**. This project aims to provide a foundational solution for managing student records efficiently, including operations like creation, viewing, editing, and deletion (CRUD).

> ✅ Designed for schools, academic projects, and educational institutions seeking a lightweight, easy-to-deploy management solution.

---

## 🧩 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Screenshots](#-screenshots)
- [Getting Started](#-getting-started)
- [Database Schema](#-database-schema)
- [Project Structure](#-project-structure)
- [Contribution](#-contribution)
- [License](#-license)

---

## ✨ Features

- 🔹 Add, edit, delete, and view student profiles.
- 🔹 Store student data securely in a MySQL database.
- 🔹 Clean, user-friendly UI built with HTML/CSS (and optional JS).
- 🔹 Flask-based MVC architecture with modular code structure.
- 🔹 Easily extensible for new features such as attendance, grades, or class assignment.

---

## 🛠️ Tech Stack

| Layer       | Technology       |
|-------------|------------------|
| Backend     | Python 3, Flask  |
| Frontend    | HTML5, CSS3, Jinja2 |
| Database    | MySQL            |
| Web Server  | Flask's development server (or compatible WSGI server) |
| Environment | Virtualenv       |

---

## 🖼️ Screenshots

> _Screenshots coming soon. Please update this section with images from `/templates` interface._

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- MySQL Server
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/ThuanProfessor/student-managements.git
cd student-managements
```
### 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
```
### 3. Install Dependencies

```bash
pip install -r requirements.txt
```
### 4. Setup MySQL Database
- Open MySQL and create a database:
```bash
CREATE DATABASE student_management;
```
- Update DB credentials in app.py:
```bash
app.config['MYSQL_HOST'] = 'localhost'
app.config['MYSQL_USER'] = 'your_username'
app.config['MYSQL_PASSWORD'] = 'your_password'
app.config['MYSQL_DB'] = 'student_management'
```
### 5. Run the Application
```bash
python app.py
```
## 🗂️ Project Structure
```php
student-managements/
├── app.py                  # Main Flask app entry point
├── templates/              # HTML templates (Jinja2)
│   ├── index.html
│   ├── add_student.html
│   └── edit_student.html
├── static/                 # Static files (CSS, JS, images)
│   ├── css/
│   └── js/
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```
## 🧮 Database Schema (Minimal)
```sql
CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    class VARCHAR(10),
    email VARCHAR(100)
);
```
## 🤝 Contribution
Contributions are welcome! Please follow these steps:

- Fork the repository

- Create a new branch: git checkout -b feature/your-feature-name

- Commit your changes: git commit -m 'Add your message'

- Push to the branch: git push origin feature/your-feature-name

- Submit a pull request
## 📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
## 🙋‍♂️ Author
ThuanProfessor
## 📫 Visit GitHub Profile

Feel free to reach out if you have any suggestions or improvements!

