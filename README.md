# Mall-Customer-Segmentation

## Project Overview
This project focuses on **Exploratory Data Analysis (EDA)** and **Clustering** using a dataset containing mall customer data. The goal is to analyze customer demographics, spending behavior, and segment customers into distinct groups using clustering techniques.

## Dataset Information
The dataset includes the following fields:
- `CustomerID`: Unique identifier for each customer
- `Gender`: Customer gender (Male/Female)
- `Age`: Age of the customer
- `Annual Income (k$)`: Annual income of the customer in thousand dollars
- `Spending Score (1-100)`: A score assigned by the mall based on customer spending behavior

## Exploratory Data Analysis (EDA)
### **1. Data Distributions**
- Used **distribution plots (Displots)** to visualize the distribution of `Age`, `Annual Income (k$)`, and `Spending Score (1-100)`.
- **Kernel Density Estimation (KDE) plots** were created to compare distributions by gender.
- **Boxplots** were used to analyze variations in `Age`, `Annual Income`, and `Spending Score` based on gender.

### **2. Correlation Analysis**
- A **heatmap** was generated to understand relationships between numerical features.
- Observations:
  - A slight negative correlation between `Age` and `Spending Score`.
  - Minimal correlation between `Annual Income` and `Spending Score`.

## Clustering Approaches
### **1. Univariate Clustering**
- Used **K-Means clustering** on `Annual Income (k$)`.
- Determined optimal clusters using the **elbow method** (inertia scores).

### **2. Bivariate Clustering**
- Applied **K-Means clustering** with 5 clusters using `Annual Income (k$)` and `Spending Score (1-100)`.
- Visualized results using a **scatter plot** and marked cluster centers.
- Created **cross-tabulations** to analyze cluster distributions by gender.

### **3. Multivariate Clustering**
- Converted categorical features into numerical values using **one-hot encoding**.
- Standardized the dataset using **StandardScaler**.
- Applied **K-Means clustering** to all numerical variables.
- Used the **elbow method** to determine the optimal number of clusters.

## Visualizations
- **Distribution Plots**: Show customer data distributions.
- **KDE Plots**: Compare gender-based distributions.
- **Boxplots**: Display gender-wise variations.
- **Heatmaps**: Illustrate correlations.
- **Scatter Plots**: Visualize clustered customer segments.

## Key Insights
- Female customers generally have **higher spending scores** than male customers.
- Customers with **higher annual incomes do not necessarily have higher spending scores**.
- Younger customers tend to have **higher spending scores**.

## Tools & Libraries Used
- **Python**
- **Pandas, NumPy** (Data Manipulation)
- **Seaborn, Matplotlib** (Data Visualization)
- **Scikit-learn** (K-Means Clustering, StandardScaler)

## Conclusion
This project successfully explores mall customer data using **EDA and clustering techniques**. The analysis provides valuable insights into customer spending behavior, helping businesses identify key customer segments for targeted marketing strategies.

## Future Improvements
- Experimenting with **other clustering algorithms** like DBSCAN or Hierarchical Clustering.
- Using **PCA (Principal Component Analysis)** for dimensionality reduction.
- Enhancing data preprocessing by considering **outliers and feature engineering**.