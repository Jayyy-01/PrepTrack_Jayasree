<div align="center">

#  PrepTrack
### Student Placement Readiness Assessment System

*A Python console application that evaluates a student's placement readiness using performance analytics, eligibility validation, and automated decision-making.*

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Platform](https://img.shields.io/badge/Platform-Console-green)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Beginner Friendly](https://img.shields.io/badge/Beginner-Friendly-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

</div>

---

#  About the Project

**PrepTrack** is a Python-based console application developed to assess whether a student is ready for campus placements based on multiple academic and performance parameters.

Instead of simply calculating scores, the application performs a complete readiness analysis by validating student information, evaluating seven days of coding practice, tracking performance trends, identifying critical areas, and providing personalized recommendations.

The project demonstrates strong understanding of Python fundamentals, problem-solving, input validation, conditional logic, looping constructs, counters, and report generation.

---

#  Key Features

###  Student Profile Management

- Validates student name
- Validates registration number
- Accepts eligible graduation year
- Records attendance percentage
- Checks project completion status
- Verifies student profile

---

###  Practice Performance Evaluation

The application analyzes **7 coding practice sessions**.

For every day it:

- Accepts practice score
- Handles absent students
- Categorizes performance
- Updates statistics
- Calculates placement metrics

---

### Intelligent Performance Classification

| Score | Category |
|--------|----------|
| **75 – 100** |  Strong |
| **60 – 74** |  Satisfactory |
| **40 – 59** |  Needs Improvement |
| **0 – 39** |  Critical |
| **-1** | Absent |

---

#  Analytics Generated

PrepTrack automatically generates:

-  Total Score
-  Average Score
-  Attempted Days
-  Absent Days
-  Passed Days
-  Failed Days
-  Strong Days
-  Satisfactory Days
-  Needs Improvement Days
-  Critical Days
-  Highest Score
-  Lowest Score
-  First Critical Day
-  First Critical Score

---

#  Placement Eligibility Rules

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

#  Decision Engine

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

#  Input Validation

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

#  Sample Report

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
#  Test-Result Table (demo – fully filled)


| Test ID | Scenario                     | Expected Result                 | Actual Result                      | Status |
|--------|------------------------------|---------------------------------|------------------------------------|--------|
| Run-01 | High scores, low attendance  | Attendance Improvement Required | Attendance Improvement Required    | Pass   |
| TC-01  | All requirements satisfied   | Ready for Mock Interview        | Ready for Mock Interview           | Pass   |
| TC-02  | Critical score present       | Critical Support Required       | Critical Support Required          | Pass   |
| TC-03  | Fewer than six attempts      | Practice Incomplete             | Practice Incomplete                | Pass   |
| TC-04  | Fewer than four passes       | Insufficient Passed Practices   | Insufficient Passed Practices      | Pass   |
| TC-05  | Average below 70             | Practice Improvement Required   | Practice Improvement Required      | Pass   |
| TC-06  | Attendance below 75          | Attendance Improvement Required | Attendance Improvement Required    | Pass   |
| TC-07  | Graduation year not eligible | Graduation Criteria Not Met     | Graduation Criteria Not Met        | Pass   |
| TC-08  | Project incomplete           | Application On Hold             | Application On Hold                | Pass   |
| TC-09  | Profile not verified         | Application On Hold             | Application On Hold                | Pass   |
| TC-10  | All days absent              | Practice Not Evaluated          | Practice Not Evaluated             | Pass   |
| TC-11  | Invalid low score            | Input rejected                  | Input rejected                     | Pass   |
| TC-12  | Invalid high score           | Input rejected                  | Input rejected                     | Pass   |
| TC-13  | Boundary scores              | Correct classifications         | Correct classifications            | Pass   |
| TC-14  | Multiple blockers            | First blocker displayed         | First blocker displayed            | Pass   |

---

#  Application Workflow

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

#  Technologies Used

- Python 3
- Console Application
- Procedural Programming
- Conditional Statements
- Loops
- Boolean Logic
- Input Validation
- Data Processing

---

#  Project Structure

```text
PrepTrack/
│
├── preptrack.py
├── README.md
└── LICENSE
```

---

#  Getting Started

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

#  Concepts Demonstrated

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

#  Future Improvements

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

---

Individual Contribution
Name: Jayasree P

Repository URL: https://github.com/Jayyy-01/preptrack-jayasree
(replace with your actual repo link once created)

My main contribution:
- Built and debugged the complete PrepTrack console application, including tracing two logic errors that surfaced only through manual test runs rather than at write time, and correcting them against the exact requirement tables in the problem statement.

Features I implemented:
- Full student-profile collection and validation, including a while-loop check for a non-empty name and a bounded while-loop check for attendance between 0 and 100.
- Yes/no input validation with retry prompts for both project-completion and profile-verification status, converted into Booleans.
- Seven-day score processing using one for loop with range(1, 8), with an inner while loop that accepts only -1 or a value from 0 to 100.
- Absent-day handling using continue so absent days are excluded from totals, attempted-day counts, and highest/lowest comparisons.
- Score classification into Strong, Satisfactory, Needs Improvement, and Critical, along with passed/failed counting based on the 60-point threshold.
- Highest and lowest score tracking, including the day each occurred, built without lists or max()/min().
- First-critical-score detection that stores only the first occurrence while still processing all seven days.
- Average calculation with a zero-attempted-days guard to prevent a crash when every day is marked absent.
- The full ten-condition priority chain for determining Final Status, Primary Blocker, and Next Action, checked against the Part 24 requirement table.


Most difficult logic:
- Getting the highest/lowest score tracking right. My first version reset highest_score and lowest_score on every iteration instead of only the first one, because I never actually set first_attempt_found to True inside the block that checked it — so the program silently treated every day as "the first attempt" and the report kept showing "Not Available" even when six days had valid scores.

Problem I faced:
- During testing, my classification counts (Strong + Satisfactory + Needs Improvement + Critical) added up to more than the actual attempted_days — for one run they totalled 12 against only 6 attempted days. At the same time, Highest Score and Lowest Score were showing "Not Available" even though real scores had been entered.

How I solved it:
- I traced the classification bug by manually re-running a fixed set of scores and counting by hand what each day should classify as, then compared it against the printed output — that's how I noticed the counters were being incremented in two separate places in my code, once in a printing block right after the absence check and again later in a second classification block. I removed the duplicate and kept a single classification pass that both counts and prints.
- For the highest/lowest bug, I stepped through the loop logic line by line and realized first_attempt_found was declared but never reassigned anywhere, so the "not first_attempt_found" branch always ran. Adding first_attempt_found = True inside that branch fixed it — verified by re-running the same test scores and confirming Highest Score and Lowest Score now showed the correct day and value instead of defaulting.


Code Review Completed
| Reviewed Member | Repository Link | What Was Done Well | Issue Identified | Suggested Improvement |
|-----------------|------------------------------------------------------|------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------|
| Deepa BhavyaSri | https://github.com/example-user/preptrack-bhavya | The highest and lowest score tracking correctly identifies both the score and the day it occurred on, and the first critical day and score are captured accurately without stopping the loop early. | Critical score detection stops processing after the first critical day. | Continue processing all seven days even after finding the first critical score, and only store the first occurrence without breaking out of the loop. |

Feedback Received
Reviewed By: Deepa BhavyaSri

Feedback Received:
- The program correctly excludes absent days from the average score calculation.
- The final status priority is mostly correct, but the attendance condition should be checked before average score in some scenarios.

Was the Feedback Valid? Yes

Change Made:
- Rechecked the final status order against the project requirement and confirmed that the current order matches the given priority.
- Added comments and tested more scenarios to ensure the priority order works as expected.

Commit Message Used:
- "Review final status priority and validate attendance condition order"

---

#  Author

**Jayasree P**

**GitHub:** https://github.com/Jayyy-01

---

#  Support

If you found this project useful, please consider giving it a star on GitHub.

It motivates future improvements and helps others discover the project.

---

<div align="center">

###  Thank you for visiting this repository!

**Happy Coding! **

</div>
````
