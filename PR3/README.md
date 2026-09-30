# Spread Locator: Statistical Distributions and Fitting Analysis

Welcome to the Spread Locator project repository! This project provides a comprehensive practical and theoretical exploration of fundamental statistical distributions, data fitting, probability computations, and normal-quantile transformations.

---

## Project Overview

This project is divided into two core parts:
1. Theoretical Foundation (Part A): Detailed theoretical concepts covering statistical distributions, Q-Q plots, discrete vs continuous distributions, probability density or mass functions, power law, log normal, Poisson, Z scores, and Box Cox transformations with real world e-commerce use cases.
2. Practical Implementation (Part B or Task 1): Python based implementation notebook demonstrating how to fit empirical data to Bernoulli and Binomial distributions and analyze parameters using statistical estimations.

---

## Table of Contents

- Key Concepts Covered
  - 1. Statistical Distributions
  - 2. Q-Q Plots (Normality Checking)
  - 3. Discrete vs Continuous Distributions
  - 4. Bernoulli Distribution
  - 5. Binomial Distribution
  - 6. Log Normal and Power Law Distributions
  - 7. Poisson Distribution
  - 8. Z Score Probability and Box Cox Transformation
  - 9. PDF vs CDF
- Hands-on Code Implementation
- Tech Stack and Dependencies
- How to Run the Notebook

---

## Key Concepts Covered

### 1. Statistical Distributions
A statistical distribution describes how dataset values are spread, providing insights into central tendency, variability, skewness, and frequency of occurrences. In e-commerce, this helps analyze customer purchase amounts and order frequencies.

### 2. Q-Q Plots (Normality Checking)
A Quantile-Quantile (Q-Q) plot compares empirical data quantiles against theoretical normal distribution quantiles along a 45 degree reference line to visually assess normality before performing parametric statistical tests.

### 3. Discrete vs Continuous Distributions

| Feature | Discrete Distribution | Continuous Distribution |
| :--- | :--- | :--- |
| Definition | Countable distinct outcomes | Infinite possible values in a range |
| Values | Whole numbers (0, 1, 2, ...) | Decimal or real numbers |
| Function | Probability Mass Function (PMF) | Probability Density Function (PDF) |
| Example | Weekly transaction count | Money spent per transaction |

### 4. Bernoulli Distribution
Models a single trial with two possible outcomes: Success (1) with probability p, and Failure (0) with probability q = 1 - p.
- PMF: P(X = k) = p^k * (1 - p)^(1 - k), where k belongs to {0, 1}
- E-commerce Example: Whether a website visitor completes a purchase (1) or leaves without buying (0).

### 5. Binomial Distribution
Models the number of successes (k) in n independent, fixed Bernoulli trials.
- PMF: P(X = k) = C(n, k) * p^k * (1 - p)^(n - k)
- E-commerce Example: Out of 100 website visitors, calculating how many will buy a product given a conversion rate p.

### 6. Log Normal and Power Law Distributions
- Log Normal: Continuous distribution where ln(X) is normally distributed. Highly applicable to right skewed revenue or transaction amount data. E-commerce application: Customer order total amounts where most purchases are small, but a few buyers spend large amounts.
- Power Law: Models heavy tailed behavior where a few extreme values dominate. E-commerce application: Pareto 80/20 principle where top 20 percent customers generate 80 percent of total revenue.

### 7. Poisson Distribution
Measures the number of independent events occurring in a fixed interval of time or space given a constant mean rate.
- PMF: P(X = k) = (lambda^k * e^-lambda) / k!
- E-commerce Example: Modeling the number of customer support tickets or orders received per hour during a sale event.

### 8. Z Score Probability and Box Cox Transformation
- Z Score: Measures standard deviations from the mean: Z = (x - mean) / standard deviation.
- Box Cox Transformation: Stabilizes variance and normalizes skewed positive data to make non normal e-commerce data (like user session times) follow a Gaussian shape.

### 9. PDF vs CDF
- Probability Density Function (PDF): Gives density at a specific continuous value x.
- Cumulative Distribution Function (CDF): Gives cumulative probability P(X <= x) up to value x. E-commerce application: Finding the probability that a customer spends less than or equal to a target amount.

---

## Hands-on Code Implementation

The included Jupyter Notebook executes distribution fitting on sample dataset tasks:

- Bernoulli Fit: Estimated probability parameter p = 0.7120.
- Binomial Fit: Estimated success probability p = 0.6771 across n = 7 trials.
- Data Visualizations: Plots generated to visually inspect PMF fits and compare theoretical against empirical frequencies.

---

## Tech Stack and Dependencies

- Python 3
- Jupyter Notebook or JupyterLab
- Libraries:
  - numpy
  - pandas
  - scipy
  - matplotlib
  - seaborn

---

## How to Run the Notebook

1. Clone the Repository:
   git clone https://github.com/your-username/spread-locator.git
   cd spread-locator

2. Install Required Packages:
   pip install numpy pandas scipy matplotlib seaborn jupyter

3. Launch Jupyter Notebook:
   jupyter notebook

4. Open and Run:
   Navigate to the notebook file and run all cells sequentially to view execution outputs and generated distribution plots.
