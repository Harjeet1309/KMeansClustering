# Customer Segmentation using K-Means Clustering


## Dataset Description

The dataset `Mall_Customers.csv` contains the following columns:

| Column                   | Description                              |
|--------------------------|------------------------------------------|
| `CustomerID`             | Unique identifier for each customer      |
| `Gender`                 | Gender of the customer (Male/Female)     |
| `Age`                    | Age of the customer                      |
| `Annual Income (k$)`     | Annual income in thousands of dollars    |
| `Spending Score (1-100)` | Score assigned based on behavior         |

---

## Tools & Libraries Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Steps Performed

1. **Data Loading & Exploration**
   - Loaded the dataset
   - Dropped unnecessary columns (`CustomerID`)
   - Converted categorical variable (`Gender`) into numerical using Label Encoding

2. **Data Visualization**
   - Used pair plots and scatter plots to understand distribution

3. **Elbow Method**
   - Used to determine the optimal number of clusters (K)
   - Based on inertia (WCSS)

4. **K-Means Clustering**
   - Applied KMeans with the optimal K (chosen = 5)
   - Assigned each data point to a cluster

5. **Cluster Visualization**
   - Plotted clusters using spending score and income
   - Clearly visualized the segmentation of customer groups

6. **Model Evaluation**
   - Used **Silhouette Score** to validate clustering performance

---

## Key Observations

- Customers were successfully segmented into **5 distinct groups**.
- Groupings reflect various spending behaviors:
  - Low income, high spending
  - High income, low spending
  - Average income and average spending, etc.
- Can help businesses in **targeted marketing and personalization**.

---

## Results

- **Optimal K (Clusters)**: 5
- **Silhouette Score**: _~0.55_ (indicating good clustering separation)
- **Visual Insights**: Each cluster represents a unique customer segment

