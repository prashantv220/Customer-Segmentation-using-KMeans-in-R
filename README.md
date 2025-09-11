# 🛍️ Customer Segmentation using K-Means Clustering (Mall Customers Dataset)

This project applies **K-Means Clustering** to segment mall customers into distinct groups based on their **Age**, **Annual Income**, and **Spending Score**.  
It includes **data preprocessing, exploratory data analysis (EDA), visualization, and clustering**.

---

## 📂 Dataset

The dataset used is **Mall_Customers.csv**, which typically has the following columns:

| Column Name                | Description                                     |
|-----------------------------|-------------------------------------------------|
| `CustomerID`               | Unique ID assigned to each customer             |
| `Genre` (or `Gender`)      | Gender of the customer (Male/Female)            |
| `Age`                      | Age of the customer                             |
| `Annual Income (k$)`       | Annual income of the customer in thousands ($k) |
| `Spending Score (1-100)`   | Spending score assigned by the mall             |

---

## ⚙️ Project Workflow

### 1. **Data Preprocessing**
- Load dataset using `read.csv()`.
- Check summary statistics, missing values, and duplicates.
- Explore gender distribution.
- Extract numeric columns (`Age`, `Annual Income`, `Spending Score`) for clustering.

### 2. **Exploratory Data Analysis (EDA)**
- Gender distribution using **bar plot** and **pie chart**.
- Age, Annual Income, and Spending Score distributions using **histograms**.
- Relationship between **Age and Annual Income** using scatter plot.

### 3. **Clustering**
- Apply **K-Means Clustering** on numerical features.
- Use the **Elbow Method** to determine optimal number of clusters (`k=5`).
- Perform clustering with `k=5` and assign cluster labels to customers.

### 4. **Visualization**
- Plot clusters in 2D: **Annual Income vs Spending Score**.
- Optional: Visualize clusters in **3D (Age, Income, Spending Score)**.

---

## 📊 Key Results

- The Elbow Method suggested **5 clusters** as optimal.
- Customers were segmented into **5 groups** based on spending habits and income:
  - **C1:** Low income, low spending
  - **C2:** High income, low spending
  - **C3:** Low income, high spending
  - **C4:** High income, high spending
  - **C5:** Average income & spending (middle group)

---

## 🛠️ Tech Stack

- **R** (for analysis and clustering)
- Libraries:
  - `ggplot2` – visualization
  - `purrr` – mapping functions
  - `factoextra` – clustering visualization (optional)
  
---


