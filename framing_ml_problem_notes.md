
## Overview of the Lecture
In this lecture, Nitish Singh explains how to systematically approach and structure a machine learning problem once a business use case is identified. 

---

## Key Steps in Framing a Machine Learning Problem

### 1. Business Problem to ML Problem
* **Objective:** Translate a vague business requirement into a precise, mathematically and computationally solvable machine learning problem.
* **Key Focus:** Understand what the business actually wants to achieve (e.g., increase revenue, reduce churn, automate a manual process) and map it to standard ML objectives.

### 2. Type of Problem
* **Classification:** Predicting a discrete class or category (e.g., Spam vs. Not Spam, Churn vs. No Churn).
* **Regression:** Predicting a continuous numerical value (e.g., House prices, Temperature, Sales forecasting).
* **Clustering / Unsupervised Learning:** Finding hidden patterns or groupings in unlabeled data.
* **Recommendation Systems / Ranking:** Suggesting relevant items to users.

### 3. Current Solution
* **Baseline Identification:** Look at how the problem is currently being solved *before* applying machine learning.
* **Why it matters:** 
  * Helps establish a performance baseline (your ML model must beat this current system/heuristic).
  * Often, a simple rule-based system or heuristic is enough, saving time and resources.

### 4. Getting Data
* **Data Availability:** Identify where the data will come from (internal databases, third-party APIs, web scraping, or public datasets).
* **Data Quality & Quantity:** Assess whether you have enough historical data and if the features collected are relevant to the target variable.

### 5. Metrics to Measure
* **Business Metrics:** Revenue generated, cost saved, conversion rate.
* **ML / Technical Metrics:** 
  * Accuracy, Precision, Recall, F1-Score (for classification).
  * RMSE, MAE, $R^2$ Score (for regression).
* **Alignment:** Ensure the chosen ML metric directly optimizes the business metric.

### 6. Online vs. Batch Learning
* **Batch Learning:** The model is trained offline using all available data at once. Updates happen periodically (e.g., retrained weekly or monthly).
* **Online Learning:** The model is trained incrementally on the fly as new data arrives in real-time (useful for streaming data or rapidly changing environments like stock prices or recommendation feeds).

### 7. Check Assumptions
* **Sanity Checks:** Validate all operational, statistical, and business assumptions before writing code or building models.
* **Risk Mitigation:** Ensure data pipelines are stable, features are realistically obtainable at inference time, and target leakage is avoided.