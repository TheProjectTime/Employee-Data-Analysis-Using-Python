# Employee Data Analysis Project

## 📌 Project Description

The **Employee Data Analysis Project** is a Python-based data analysis project using the **Pandas** library.

The project uses an employee dataset stored in a CSV file and performs basic analysis such as calculating the average salary, counting employees by department, filtering employees based on a salary threshold, and exporting the results to new CSV files.

## ✨ Features

* Load employee data from a CSV file
* Display basic dataset information
* Calculate average employee salary
* Count employees in each department
* Filter employees above a specified salary
* Export filtered employee data to a CSV file
* Export department-wise employee count to a CSV file

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **CSV File Handling**
* **Google Colab** (optional)

## 📂 Project Structure

```text
Employee-Data-Analysis/
│
├── employee_analysis.py
├── Employee.csv
├── employee_analysis_results.csv
├── department_count.csv
└── README.md
```

## 📊 Dataset

The project uses an employee dataset containing information such as:

* Employee ID
* Employee Name
* Department
* Salary

Example:

```text
Employee ID,Name,Department,Salary
101,Anurag,IT,60000
102,Rahul,HR,45000
103,Priya,Finance,55000
104,Amit,IT,75000
105,Sneha,Marketing,50000
```

## ▶️ How to Run

### Using Google Colab

1. Open Google Colab.
2. Create a new notebook.
3. Copy the Python code into a cell.
4. Run the code.
5. Upload `Employee.csv` when prompted.
6. Enter the salary threshold when requested.

Example:

```text
Enter salary threshold: 60000
```

### Using Python

Place the following files in the same folder:

```text
employee_analysis.py
Employee.csv
```

Then run:

```bash
python employee_analysis.py
```

## 🔍 Analysis Performed

### 1. Load CSV

The employee dataset is loaded using Pandas:

```python
df = pd.read_csv("Employee.csv")
```

### 2. Average Salary

The average salary of all employees is calculated using:

```python
df["Salary"].mean()
```

### 3. Department Count

The number of employees in each department is calculated using:

```python
df["Department"].value_counts()
```

### 4. Salary Filtering

Employees earning more than the entered salary threshold are filtered.

For example, if the threshold is `60000`, employees earning more than ₹60,000 are displayed.

### 5. Export Results

The filtered employee records are saved as:

```text
employee_analysis_results.csv
```

The department-wise employee count is saved as:

```text
department_count.csv
```

## 📁 Output Files

### `employee_analysis_results.csv`

Contains employees whose salary is above the specified threshold.

### `department_count.csv`

Contains the number of employees in each department.

## 🎯 Objective

The objective of this project is to demonstrate basic **data analysis using Python and Pandas**, including CSV data loading, statistical calculations, filtering, grouping, and exporting processed data.

## 👨‍💻 Author

**Anurag Kumar Rana**
