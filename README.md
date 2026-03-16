# Python Data Analysis Workflow

## Overview

This repository contains a Python-based data analysis workflow implemented in a Jupyter Notebook.
The notebook demonstrates how Python libraries can be used to load, inspect, visualize, and preprocess a structured dataset.

The project is written step-by-step to show how Python tools such as **pandas, numpy, matplotlib, seaborn, and scikit-learn utilities** can be used to work with tabular data efficiently.

---

## Project Structure

project-folder/

├── churn_analysis.ipynb
├── customer_data.csv
├── README.md
└── requirements.txt

* **churn_analysis.ipynb** – Main notebook containing all Python code
* **customer_data.csv** – Dataset used in the analysis
* **README.md** – Project documentation
* **requirements.txt** – List of Python dependencies

---

## Python Libraries Used

The notebook uses the following Python libraries:

* pandas – data manipulation and analysis
* numpy – numerical operations
* matplotlib – data visualization
* seaborn – statistical visualizations
* scikit-learn – preprocessing utilities and pipelines
* joblib – saving Python objects

---

## Code Workflow

### 1. Importing Libraries

The notebook begins by importing required Python libraries for data manipulation, visualization, preprocessing utilities, and configuration settings.

It also sets visualization themes and display settings to improve readability of tables and plots.

---

### 2. Loading the Dataset

The dataset is loaded using pandas.

Example:

df = pd.read_csv("customer_data.csv")

Basic information such as dataset shape and preview rows are displayed.

---

### 3. Initial Data Inspection

Basic inspection is performed using pandas functions including:

* df.info() to view column data types
* df.describe() to view statistical summaries
* df.isnull().sum() to check missing values
* value_counts() to inspect categorical distributions

This step helps understand the structure of the dataset before further processing.

---

### 4. Data Visualization

The notebook uses **matplotlib** and **seaborn** to visualize the data.

Visualization techniques used include:

* Kernel density distribution plots
* Pair plots for numeric relationships
* Violin plots for distribution comparison
* Count plots for categorical features
* Pie charts for proportional comparisons
* Correlation heatmaps
* Scatter plots
* Bar charts for grouped statistics

These visualizations help explore patterns and relationships in the dataset.

---

### 5. Feature Creation Using Python

Additional columns are created using pandas operations to enrich the dataset.

Examples include:

* balance_per_product
* salary_balance_ratio
* age_group categories
* tenure_bucket categories
* high_balance indicator

These features are generated using arithmetic operations, conditional logic, and pandas transformation functions.

---

### 6. Data Preprocessing

Preprocessing is implemented using utilities from scikit-learn.

Steps include:

* Handling missing values using SimpleImputer
* Scaling numeric columns using StandardScaler
* Encoding categorical variables using OneHotEncoder
* Combining transformations using ColumnTransformer
* Organizing transformations using Pipeline

This structure helps keep the data preparation workflow organized and reusable.

---






