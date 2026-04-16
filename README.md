# 👥 HR Analytics Dashboard — Tableau

An interactive HR analytics dashboard built with Tableau, powered by a synthetically generated dataset of **8,950 employee records** across 7 departments and 8 US states. The dashboard enables HR teams and business stakeholders to explore workforce composition, attrition trends, salary distribution, and performance insights.

---

## 📊 Dashboard Overview

The dashboard is structured around four core analytical areas:

| Area | Description |
|------|-------------|
| **Workforce Overview** | Headcount by department, gender, education level, and geography |
| **Attrition Analysis** | Termination trends over time (2015–2024), attrition rate (~11.2%) |
| **Salary Insights** | Salary distribution by role, department, education, and gender |
| **Performance Metrics** | Performance ratings breakdown across departments and job titles |

---

## 🗂️ Repository Structure

```
hr-analytics-tableau/
│
├── HR_Dashboard.twbx          # Packaged Tableau workbook (includes data)
├── dataset.csv                # Cleaned HR dataset (8,950 records)
├── generate_data.py           # Python script used to generate synthetic data
└── README.md
```

---

## 📁 Dataset

The dataset was synthetically generated using Python (`Faker`, `NumPy`, `Pandas`) with realistic distributions.

**Fields:**

| Column | Description |
|--------|-------------|
| `Employee_ID` | Unique employee identifier |
| `First Name / Last Name` | Employee name |
| `Gender` | Male (54%) / Female (46%) |
| `State / City` | Location across 8 US states (New York-heavy distribution) |
| `Education Level` | High School, Bachelor, Master, PhD |
| `Birthdate / Hiredate` | Date of birth and hire date (2015–2024) |
| `Termdate` | Termination date (NULL if still active) |
| `Department` | HR, IT, Sales, Marketing, Finance, Operations, Customer Service |
| `Job Title` | Role within department (4 per department) |
| `Salary` | Adjusted for education level, gender multiplier, and age |
| `Performance Rating` | Excellent, Good, Satisfactory, Needs Improvement |

**Key Stats:**
- **Total Records:** 8,950
- **Attrition Rate:** ~11.2%
- **Salary Range:** $50,000 – $120,000+ (role and education dependent)
- **Date Range:** Hire dates from 2015 to 2024

---

## 🛠️ Tools & Technologies

- **Tableau Desktop / Tableau Public** — Dashboard design and visualisation
- **Python 3.x** — Synthetic data generation
  - `pandas` — Data manipulation
  - `numpy` — Statistical distributions
  - `faker` — Realistic name and date generation

---


## 📌 Key Insights Surfaced

- **Operations** is the largest department (~30% of workforce), followed by Customer Service (~19%) and Sales (~21%)
- Salary gaps exist by education level and show a slight gender-based multiplier built into the data model
- Attrition peaked in **2021**, aligning with broader "Great Resignation" trends modelled in the data
- **PhD holders** and **Managers** skew older (30–65), reflecting realistic career progression

---

## 📄 License

This project uses a **synthetically generated dataset** — no real employee data is included. Free to use for portfolio, learning, and non-commercial purposes.

---

## 🙋 Author

Built as a portfolio project to demonstrate HR analytics, data storytelling, and Tableau dashboard development skills.
