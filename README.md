# 📊 Student Attendance & Shortage Predictor

A web-based application that helps students **track their attendance, identify attendance shortages, and predict the number of classes they need to attend to reach the required attendance percentage**.

The project is designed to solve a common problem faced by college students: keeping track of attendance across multiple subjects and knowing how future attendance will affect their eligibility.

---

## 🎯 Project Objective

The main objective of this project is to provide students with a simple and interactive platform to:

- Track attendance for multiple subjects
- Calculate attendance percentage automatically
- Identify subjects with attendance shortage
- Calculate the number of classes required to reach a target percentage
- Calculate how many classes can be safely missed
- Predict future attendance using a **"What If?" calculator**
- View attendance information through a centralized dashboard

---

## ✨ Features

### 📚 Subject-wise Attendance
Add and manage attendance information for different subjects.

### 📈 Automatic Attendance Calculation
The system automatically calculates attendance based on:

```text
Attendance % = (Classes Attended / Classes Conducted) × 100
```

### ⚠️ Shortage Detection
The application identifies subjects where attendance is below the required percentage.

### 🎯 Attendance Predictor
Calculate how many consecutive classes a student needs to attend to reach the target attendance percentage.

### ❓ What-If Calculator
Students can check scenarios such as:

- What happens if I miss the next 2 classes?
- What happens if I attend the next 5 classes?
- How many classes can I miss while maintaining 75% attendance?

### 📊 Dashboard
Display overall and subject-wise attendance using a clean dashboard with visual indicators and charts.

### 💾 Database Storage
Student, subject, and attendance information is stored in a MySQL database.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML | Structure of the web pages |
| CSS | Styling and responsive UI |
| JavaScript | Frontend interactions and calculations |
| Python | Backend programming |
| Flask | Web application framework |
| MySQL | Database management |

---

## 🏗️ Project Architecture

```text
                 ┌─────────────────────┐
                 │       Student       │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   HTML / CSS / JS   │
                 │      Frontend       │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │    Python Flask     │
                 │       Backend       │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │        MySQL        │
                 │      Database       │
                 └─────────────────────┘
```

---

## 📁 Project Structure

```text
Attendance-Predictor/
│
├── app.py
├── database.py
├── requirements.txt
│
├── templates/
│   └── index.html
│
├── static/
│   ├── style.css
│   └── script.js
│
├── database/
│   └── schema.sql
│
└── README.md
```

---

## 🧮 Attendance Calculation

The basic attendance percentage is calculated using:

```text
Attendance Percentage =
(Classes Attended / Classes Conducted) × 100
```

### Example

If a student attended 30 out of 40 classes:

```text
(30 / 40) × 100 = 75%
```

The application can then determine whether the student meets the required attendance percentage.

---

## 🔮 Future Attendance Prediction

The system can calculate the number of classes required to reach a target percentage.

For example:

```text
Current attendance:
30 / 45 = 66.67%

Target:
75%

The system calculates how many consecutive classes
the student needs to attend to reach 75%.
```

It can also calculate the maximum number of classes a student can miss without falling below the required percentage.

---

## 📊 Dashboard

The dashboard is planned to provide an overview such as:

```text
Overall Attendance: 78.5%

-----------------------------------
Subject       Attendance    Status
-----------------------------------
DBMS             82%       🟢 Good
OS               76%       🟢 Good
Networks         68%       🔴 Shortage
Python           85%       🟢 Good
-----------------------------------
```

Visual charts can be used to make attendance trends easier to understand.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/attendance-predictor.git
```

### 2. Navigate to the Project

```bash
cd attendance-predictor
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

### 4. Configure MySQL

Create the required database and tables using:

```text
database/schema.sql
```

Update the database credentials in the Python configuration file.

### 5. Run the Application

```bash
python app.py
```

### 6. Open in Browser

```text
http://127.0.0.1:5000
```

---

## 🔐 Planned Improvements

Future versions may include:

- 🔑 User authentication and login
- 👨‍🎓 Multiple student profiles
- 📱 Responsive mobile-friendly design
- 📊 Advanced attendance analytics
- 📅 Attendance history
- 🔔 Low-attendance alerts
- 📧 Email notifications
- 📈 Attendance trend analysis
- ☁️ Cloud deployment
- 👨‍🏫 Faculty/admin dashboard

---

## 🎓 Learning Outcomes

Through this project, the following concepts will be practiced:

- Frontend web development
- Backend development with Python Flask
- MySQL database design
- SQL queries
- Connecting frontend, backend, and database
- Form handling
- Data validation
- Basic data visualization
- Problem-solving and business logic
- Web application development

---

## 👨‍💻 Author

**Ishtiaq Hussain**

B.Tech — Computer Science Engineering

---

## ⭐ Project Status

🚧 **Currently in Development**

The project is being developed as a mini-project to gain practical experience in **web development, Python, SQL, and database-driven applications**.
