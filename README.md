# College Student Performance Analysis

## Overview

This project analyzes a college student performance dataset using Python, Pandas, Matplotlib, and Seaborn. The notebook explores academic performance, student characteristics, backlogs, CGPA distribution, and placement outcomes.

The analysis is performed in the Jupyter/Google Colab notebook:

- `college_student_performance.ipynb`

The notebook loads the dataset from:

- `student_performance_dataset.csv`

## Dataset

The dataset contains **3,000 student records** and **15 columns**.

### Features

| Column | Description |
|---|---|
| `student_id` | Unique student identifier |
| `gender` | Student gender |
| `age` | Student age |
| `department` | Academic department |
| `semester` | Current semester |
| `study_hours_per_day` | Average daily study hours |
| `attendance_percentage` | Attendance percentage |
| `sleep_hours_per_day` | Average daily sleep |
| `backlogs` | Number of academic backlogs |
| `extracurricular_activity` | Participation in extracurricular activities |
| `internet_access_at_home` | Whether the student has internet access at home |
| `part_time_job` | Whether the student has a part-time job |
| `family_income_level` | Family income category |
| `cgpa` | Student CGPA |
| `placed` | Whether the student was placed |

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Analysis Performed

### 1. Data Loading
The notebook reads the student performance CSV file using Pandas and displays the first few records.

### 2. Data Quality Check
Missing values are checked using `isnull()` and `isnull().sum()`. The notebook output shows **0 missing values for every column**.

### 3. Dataset Exploration
Basic dataset information is explored using:

- Dataset shape
- Descriptive statistics
- Department-wise counts
- CGPA-related frequency analysis

The dataset shape is **3000 × 15**.

### 4. Academic Performance Analysis
The notebook investigates students with a **10.00 CGPA**, including:

- Department-wise count
- Department and semester-wise count
- Department and semester-wise count of students who achieved 10.00 CGPA and were placed

The notebook reports **68 students with a CGPA of 10.00**.

### 5. Placement Analysis
The overall placement rate is calculated from the `placed` column.

**Placement Percentage Rate: 71.50%**

### 6. Data Visualization
The notebook uses Matplotlib and Seaborn to visualize the data, including:

- Pair plot of dataset variables
- Backlog distribution
- CGPA distribution
- Gender vs. placement
- Department and gender placement rates
- Placement-rate heatmap

### 7. Backlog Analysis
The distribution of the number of backlogs is examined. The notebook notes that students with **3 or 4 backlogs are relatively less common**.

### 8. CGPA Distribution
CGPA values are grouped into ranges:

- 4–5
- 5–6
- 6–7
- 7–8
- 8–9
- 9–10

A count plot is used to visualize the number of students in each CGPA range.

### 9. Placement by Gender
Placement outcomes are compared across genders using a count plot.

### 10. Department and Gender Placement Analysis
Placement percentages are calculated for each combination of department and gender. A heatmap is then used to make these differences easier to compare.

The notebook's final observation notes that male placement rates are generally higher across departments, with a reported **11.9 percentage-point gender gap in Civil Engineering**, while Computer Science and IT show slightly higher placement rates for females.

## How to Run

### Option 1: Google Colab

1. Upload `college_student_performance.ipynb`.
2. Upload `student_performance_dataset.csv`.
3. Open the notebook in Google Colab.
4. Run the cells from top to bottom.

### Option 2: Local Jupyter Notebook

Install the required packages:

```bash
pip install pandas matplotlib seaborn jupyter
```

Keep the notebook and CSV dataset available, then start Jupyter:

```bash
jupyter notebook
```

Open `college_student_performance.ipynb` and run all cells.

## Project Structure

```text
college-student-performance/
│
├── college_student_performance.ipynb
├── student_performance_dataset.csv
└── README.md
```

## Key Results

- **Students analyzed:** 3,000
- **Features:** 15
- **Missing values:** 0
- **Overall placement rate:** 71.50%
- **Students with 10.00 CGPA:** 68
- **Departments:** Civil, Computer Science, Electrical, Electronics, IT, Mechanical
- **Semesters covered:** 1–8

## Purpose

The project provides an exploratory view of how academic and student-related factors are distributed in the dataset and how placement outcomes vary across groups such as department and gender.

## Notes

This README describes the analysis implemented in the supplied notebook. It does not claim predictive machine-learning performance because the notebook primarily performs exploratory data analysis and visualization rather than training and evaluating a predictive model.
