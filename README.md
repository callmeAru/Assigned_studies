# NumPy Case Studies

## Overview
Three practical NumPy case studies for learning array operations and basic data analysis.

### Case Studies
1. Employee Performance & Salary Analytics
2. Retail Sales Performance Analysis
3. Student Performance Analytics

---

# Case Study 1 — Employee Performance & Salary Analytics

## Business Scenario
A company wants to analyze employee performance across four quarters. The HR analytics team needs employee totals, averages, rankings, growth rates, and performance filtering.

## Dataset

```python
employees = ["Arun", "Bhavana", "Charan", "Divya", "Eshan", "Fathima"]

performance = np.array([
    [78, 82, 85, 88],
    [65, 70, 68, 74],
    [92, 89, 95, 91],
    [55, 62, 60, 67],
    [81, 79, 84, 87],
    [72, 75, 78, 80]
])

quarters = ["Q1", "Q2", "Q3", "Q4"]
```

## Questions
1. Calculate the total performance score for every employee.
2. Calculate the average quarterly performance for every employee.
3. Calculate the average performance for each quarter.
4. Identify the employee with the highest total performance score.
5. Rank all employees based on total performance score.
6. Calculate quarter-over-quarter percentage growth from Q1 to Q4.
7. Identify employees whose average performance is greater than or equal to 80.
8. Count employees whose average performance is below 70.
9. Find the highest performance score in the entire dataset.
10. Identify the employee and quarter where the highest score occurred.

---

# Case Study 2 — Retail Sales Performance Analysis

## Business Scenario
A retail company has quarterly sales for five stores across four quarters. The analytics team needs store totals, quarter totals, averages, rankings, and performance flags.

## Dataset

```python
stores = ["Store_A", "Store_B", "Store_C", "Store_D", "Store_E"]

sales = np.array([
    [120000, 135000, 142000, 155000],
    [98000, 105000, 110000, 108000],
    [150000, 148000, 160000, 172000],
    [87000, 92000, 99000, 115000],
    [130000, 138000, 141000, 149000]
])
```

## Questions
1. Calculate total sales for every store.
2. Calculate average quarterly sales for every store.
3. Calculate total sales for every quarter.
4. Identify the store with the highest annual sales.
5. Rank stores by annual sales.
6. Calculate quarter-over-quarter percentage change for each store.
7. Flag stores whose annual sales exceed the overall average.

---

# Case Study 3 — Student Performance Analytics

## Business Scenario
An academic analytics team wants to identify subject-level performance, student averages, pass/fail status, top performers, and students requiring support.

## Dataset

```python
students = ["Anu", "Binu", "Cathy", "Deepa", "Ebin", "Fahad"]

marks = np.array([
    [82, 75, 91, 88],
    [61, 68, 70, 65],
    [45, 52, 48, 55],
    [90, 94, 89, 92],
    [72, 80, 76, 85],
    [38, 42, 49, 44]
])

subjects = ["Python", "SQL", "Excel", "Statistics"]
```

## Questions
1. Calculate total and average marks for each student.
2. Calculate subject averages.
3. Find the highest mark in each subject.
4. Create a pass/fail status using 50 as the threshold.
5. Identify students who passed every subject.
6. Identify students whose average is below 60.
7. Assign grades using A >= 80, B >= 60, C >= 50, otherwise F.

---

# NumPy Concepts Practiced

- `np.array()`
- `np.sum()`
- `np.mean()`
- `np.max()`
- `np.argmax()`
- `np.argsort()`
- `np.round()`
- `np.where()`
- `np.all()`
- Boolean indexing
- Indexing and slicing
- `axis=0` and `axis=1`
- Percentage calculations
- Ranking and sorting
- Conditional filtering

## Important `axis` Concept

```python
# Row-wise
np.sum(array, axis=1)
np.mean(array, axis=1)

# Column-wise
np.sum(array, axis=0)
np.mean(array, axis=0)
```

# Requirements

```bash
pip install numpy
```

Then:

```python
import numpy as np
```

# Suggested Project Structure

```text
numpy-case-studies/
├── README.md
├── case_study_1_employee.py
├── case_study_2_retail.py
└── case_study_3_student.py
```

## Learning Objective
Build practical NumPy skills by solving realistic data-analysis problems using arrays, aggregation, filtering, ranking, slicing, and conditional operations.
