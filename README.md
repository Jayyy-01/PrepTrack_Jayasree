<div align="center">

# 🚀 PrepTrack
### Student Placement Readiness Assessment System

*A Python console application that evaluates a student's placement readiness using performance analytics, eligibility validation, and automated decision-making.*

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Platform](https://img.shields.io/badge/Platform-Console-green)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Beginner Friendly](https://img.shields.io/badge/Beginner-Friendly-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

</div>

---

# 📖 About the Project

**PrepTrack** is a Python-based console application developed to assess whether a student is ready for campus placements based on multiple academic and performance parameters.

Instead of simply calculating scores, the application performs a complete readiness analysis by validating student information, evaluating seven days of coding practice, tracking performance trends, identifying critical areas, and providing personalized recommendations.

The project demonstrates strong understanding of Python fundamentals, problem-solving, input validation, conditional logic, looping constructs, counters, and report generation.

---

# ✨ Key Features

### 👤 Student Profile Management

- Validates student name
- Validates registration number
- Accepts eligible graduation year
- Records attendance percentage
- Checks project completion status
- Verifies student profile

---

### 📊 Practice Performance Evaluation

The application analyzes **7 coding practice sessions**.

For every day it:

- Accepts practice score
- Handles absent students
- Categorizes performance
- Updates statistics
- Calculates placement metrics

---

### 🎯 Intelligent Performance Classification

| Score | Category |
|--------|----------|
| **75 – 100** | ⭐ Strong |
| **60 – 74** | ✅ Satisfactory |
| **40 – 59** | ⚠ Needs Improvement |
| **0 – 39** | ❌ Critical |
| **-1** | Absent |

---

# 📈 Analytics Generated

PrepTrack automatically generates:

- ✅ Total Score
- ✅ Average Score
- ✅ Attempted Days
- ✅ Absent Days
- ✅ Passed Days
- ✅ Failed Days
- ✅ Strong Days
- ✅ Satisfactory Days
- ✅ Needs Improvement Days
- ✅ Critical Days
- ✅ Highest Score
- ✅ Lowest Score
- ✅ First Critical Day
- ✅ First Critical Score

---

# ✅ Placement Eligibility Rules

A student is considered **Placement Ready** only when **all** of the following conditions are satisfied.

| Requirement | Eligibility |
|--------------|------------|
| Graduation Year | 2025–2027 |
| Attendance | ≥ 75% |
| Practice Attempts | ≥ 6 |
| Average Score | ≥ 70 |
| Passed Days | ≥ 4 |
| Critical Scores | None |
| Project Completed | Yes |
| Profile Verified | Yes |

---

# 🧠 Decision Engine

PrepTrack evaluates the student's readiness using the following priority:

1. No practice attempted
2. Critical score detected
3. Less than six attempts
4. Less than four passed practices
5. Average below 70
6. Attendance below 75%
7. Graduation year not eligible
8. Project incomplete
9. Profile not verified
10. Ready for Mock Interview

---

# 🔒 Input Validation

The application validates every user input.

| Input | Validation |
|-------|------------|
| Student Name | Cannot be empty |
| Registration Number | Cannot be empty |
| Graduation Year | Between 2025–2027 |
| Attendance | 0–100 |
| Practice Score | -1 or 0–100 |
| Project Status | yes / no |
| Profile Status | yes / no |

---

# 📋 Sample Report

```text
==================================================
              PREPTRACK REPORT
==================================================

Student Name           : Jayasree
Registration Number    : 21MT1A0456
Graduation Year        : 2026
Attendance             : 87%

Attempted Days         : 7
Absent Days            : 0
Passed Days            : 6
Failed Days            : 1

Strong Days            : 4
Satisfactory Days      : 2
Needs Improvement Days : 1
Critical Days          : 0

Average Score          : 81.43

Final Status           : Ready for Mock Interview
Primary Blocker        : None
Next Action            : Proceed to placement mock interviews
```

---

# 🔄 Application Workflow

```text
Start
   │
   ▼
Collect Student Details
   │
   ▼
Validate Inputs
   │
   ▼
Collect Practice Scores
   │
   ▼
Analyze Performance
   │
   ▼
Calculate Statistics
   │
   ▼
Check Eligibility Rules
   │
   ▼
Generate Final Report
   │
   ▼
End
```

---

# 🛠 Technologies Used

- Python 3
- Console Application
- Procedural Programming
- Conditional Statements
- Loops
- Boolean Logic
- Input Validation
- Data Processing

---

# 📂 Project Structure

```text
PrepTrack/
│
├── preptrack.py
├── README.md
└── LICENSE
```

---

# ▶️ Getting Started

## Clone the repository

```bash
git clone https://github.com/Jayyy-01/PrepTrack.git
```

## Navigate to the project

```bash
cd PrepTrack
```

## Run the application

```bash
python preptrack.py
```

---

# 💡 Concepts Demonstrated

Python concepts I used:
- Input handling with `input()`, `int()`, and `float()`.
- Conditional statements (`if`, `elif`, `else`) and boolean expressions.
- `while` loops for validating student name, attendance, and yes/no inputs.
- `for` loops with `range()` for repeating logic over seven practice days.
- `break` for exiting validation loops after valid input.
- `continue` for skipping logic on absent practice days.
- Counters and accumulator variables for tracking days and scores.
- Defensive programming patterns such as preventing division by zero and initializing highest/lowest scores without lists.

---

# 🚀 Future Improvements

Some possible enhancements include:

- Store records using MySQL or SQLite
- Export reports as PDF
- Export reports to Excel
- User authentication
- GUI with Tkinter
- Web application using Django or Flask
- Performance dashboards
- Graphical analytics
- Multiple student management
- Email report generation

---

# 📸 Screenshots

> Add screenshots of your application here after uploading them to GitHub.

```
assets/
├── home.png
├── input.png
├── report.png
```

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push the branch
5. Open a Pull Request

---

# 👩‍💻 Author

**Jayasree P**

**Electronics and Communication Engineering Student**

Passionate about Python, Backend Development, AI, and Problem Solving.

**GitHub:** https://github.com/Jayyy-01

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

It motivates future improvements and helps others discover the project.

---

<div align="center">

### 🚀 Thank you for visiting this repository!

**Happy Coding! 💙**

</div>
````
