# K-Means Clustering: Mall Customer Segmentation

This project uses the K-Means algorithm to group customers from the "Mall Customers" dataset into different segments based on their income and spending habits.

## What it Does

1.  **Loads Data**: Reads customer data from `Mall_Customers.csv`.
2.  **Prepares Data**: Selects 'Annual Income (k$)' and 'Spending Score (1-100)', scales them, and uses PCA to help visualize in 2D.
3.  **Finds Best K**: Uses the Elbow Method and Silhouette Score to determine the optimal number of customer groups (K). K=5 was found to be the best.
4.  **Clusters Customers**: Applies K-Means with K=5 to assign each customer to a group.
5.  **Visualizes Results**: Shows a scatter plot where each point is a customer, colored according to their assigned cluster.

## Dataset

*   File: `Mall_Customers.csv`
*   Key columns used: `Annual Income (k$)`, `Spending Score (1-100)`

## Libraries Needed

*   `pandas` (for data handling)
*   `numpy` (for numerical operations)
*   `scikit-learn` (for StandardScaler, PCA, KMeans, silhouette_score)
*   `matplotlib` (for plotting)
*   `seaborn` (for enhanced plotting)

## Main Result

The analysis identified **5 distinct customer segments** based on income and spending score, which are clearly visible in the final plot.

## How to Run

1.  Make sure you have Python and the libraries above installed (`pip install pandas numpy scikit-learn matplotlib seaborn`).
2.  Have the `Mall_Customers.csv` file in the same folder.
3.  Run the Jupyter Notebook `Task_8_Clustering_with_K_Means.ipynb`.
