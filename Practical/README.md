# Employee Performance & Promotion Analysis

## Project Overview
This project performs an end-to-end exploratory and statistical data analysis on an employee dataset (`employee_performance.csv`) containing approximately 4,000 records. The goal is to evaluate key employee attributes—such as working hours, completed projects, salary, and performance scores—to analyze their influence on employee performance and promotional probability.

The project is structured into two main parts:
1. **Part A – Theoretical Fundamentals**: Concise explanations of key statistical concepts, probability distributions, linear algebra, and data science principles.
2. **Part B – Practical Python Analysis**: Hands-on exploratory data analysis (EDA), hypothesis testing, probability calculation, data visualization, and vector algebra applications using standard Data Science libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`).

---

## Dataset Description
The dataset `employee_performance.csv` contains the following fields:

| Field Name | Description | Data Type |
| :--- | :--- | :--- |
| **Employee_ID** | Unique identifier for each employee | Categorical / String |
| **Department** | Department name (Sales, IT, HR, Finance, Marketing) | Categorical |
| **Age** | Age of the employee in years | Integer |
| **Salary** | Annual salary of the employee ($) | Continuous Numerical |
| **Projects_Completed** | Total count of completed projects | Discrete Numerical |
| **Working_Hours** | Weekly working hours | Continuous Numerical |
| **Performance_Score**| Employee evaluation score (Range: 0–100) | Continuous Numerical |
| **Promotion_Status** | Promotion result ('Yes' or 'No') | Binary Categorical |

---

## Project Structure & Key Execution Steps

### Part A: Theoretical Topics Covered
* **Central Tendency:** Mean, Median, and Mode in salary distribution.
* **Dispersion Measures:** Differences between Range and Variance.
* **Distributions:** Normal vs. Poisson Distributions.
* **Shape of Data:** Positive vs. Negative Skewness with workplace examples.
* **Probability Concepts:** Conditional Probability, Independent vs. Mutually Exclusive Events.
* **Inference & Decision Making:** Real-world applications of Bayes' Theorem in HR Analytics.
* **Dimensionality Reduction:** Overview and significance of Principal Component Analysis (PCA).

---

### Part B: Practical Python Tasks

#### Step 1: Central Tendency & Dispersion
* Computed Mean, Median, and Mode for **Salary**.
* Calculated Variance and Standard Deviation for **Projects_Completed**.

#### Step 2: Probability & Events
* Evaluated overall promotional probability $P(\text{Promotion} = \text{'Yes'})$.
* Constructed a Contingency Table comparing **Department** vs. **Promotion_Status**.
* Computed Conditional Probability $P(\text{Promotion} \mid \text{Performance\_Score} > 80)$.

#### Step 3: Distributions & Visualization
* Plotted a **Histogram** of `Performance_Score` overlayed with a fitted Gaussian (Normal) curve.
* Calculated **Skewness** and **Kurtosis** for `Salary`.
* Generated a **Q-Q Plot** for `Projects_Completed` to inspect normality.

#### Step 4: Linear Algebra Application
* Represented employee metrics `[Projects_Completed, Working_Hours]` as 2D Vectors.
* Performed **Dot Product** between two employee vectors.
* Calculated **$L_1$ Norm (Manhattan)** and **$L_2$ Norm (Euclidean)** distances.
* Computed the **Angle ($\theta$)** in radians and degrees between two employee vectors.

---

## Key Insights & Business Recommendations

1. **High Performance Drives Promotions:** Employees with a `Performance_Score > 80` have a significantly higher conditional probability of getting promoted compared to the overall average promotion rate.
2. **Right-Skewed Compensation Structure:** The `Salary` metric exhibits positive skewness ($\text{Mean} > \text{Median}$), indicating that a majority of employees earn baseline-to-mid-tier salaries, while a few senior roles pull the average upward.
3. **Discrete Work Outputs:** The distribution of `Projects_Completed` aligns closely with discrete count-based models (Poisson distribution), showing bounded variance around project outcomes.

---

## Tech Stack & Dependencies
* **Python 3.x**
* **Pandas** – Data manipulation & structured analysis
* **NumPy** – Linear algebra & numerical vector operations
* **Matplotlib & Seaborn** – Data visualization & statistical plotting
* **SciPy** – Statistical distributions, density fitting & Q-Q plotting
