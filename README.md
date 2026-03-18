# 📊 Data Manipulation with Pandas

👨‍🏫 Instructor: **Sohail Ahmed**
📚 Course: **Introduction to Data Science**

---

## 📌 Project Overview

This project is designed to teach students the fundamentals of **Data Manipulation using Python and Pandas**.

Students will learn how to:

* Load data from CSV files
* Explore and understand datasets
* Handle missing values
* Filter and sort data
* Create new columns
* Prepare clean data for analysis

---

## 🧠 Key Concept

> **“Data Manipulation is the foundation of Data Science.
> Before AI, Machine Learning, or dashboards — we must clean and organize data.”**

---

## 📁 Project Structure

```
data-manipulation-pandas
│
├── data_manipulation_dataset.csv
├── Data_Manipulation_Pandas_Advanced_Lecture.docx
└── README.md
```

---

## ⚙️ Requirements

Make sure you have installed:

* Python (>= 3.8)
* Anaconda (Recommended)
* Jupyter Notebook

---

## 🚀 How to Run the Project

### Step 1: Open Anaconda Navigator

Launch **Jupyter Notebook**

---

### Step 2: Open Project Folder

Navigate to your project directory

---

### Step 3: Create New Notebook

Click:

```
New → Python 3
```

---

### Step 4: Run the Code

Paste and run the following code:

```python
import pandas as pd

# Load dataset
df = pd.read_csv("data_manipulation_dataset.csv")

# Show data
df.head()
```

---

## 🔍 Data Exploration

```python
df.info()
df.describe()
df.isnull().sum()
```

---

## 🧹 Data Cleaning

```python
df["Price"].fillna(df["Price"].mean(), inplace=True)
df["Quantity"].fillna(1, inplace=True)
df["City"].fillna("Unknown", inplace=True)
```

---

## 🔍 Filtering Data

```python
df[df["City"] == "Karachi"]
```

---

## 📊 Sorting Data

```python
df.sort_values(by="Price")
df.sort_values(by="Price", ascending=False)
```

---

## ➕ Create New Column

```python
df["Total"] = df["Price"] * df["Quantity"]
```

---

## 💾 Save Clean Data

```python
df.to_csv("clean_data.csv", index=False)
```

---

## 🎓 Student Tasks

Students should:

1. Load the dataset
2. Find missing values
3. Clean missing values
4. Filter Karachi data
5. Sort by highest price
6. Create Total column
7. Find average price

---

## 🌍 Real-World Use Case

This project simulates real-world scenarios where companies need to:

* Clean messy datasets
* Analyze business data
* Generate insights
* Prepare data for Machine Learning

---

## 🏆 Skills Gained

* Python Programming
* Pandas Library
* Data Cleaning
* Data Analysis
* Data Manipulation
* Problem Solving

---

## 📌 Author

**Sohail Ahmed**
Senior Full Stack Blockchain Engineer & Instructor

---
