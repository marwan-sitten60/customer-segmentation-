# Customer Segmentation with KMeans Clustering

## Overview

This project performs customer segmentation using the KMeans clustering algorithm on the `Mall_Customers.csv` dataset. It groups customers based on attributes like age, gender, annual income, and spending score using Python, pandas, scikit-learn, matplotlib, and seaborn.

## Dataset

`Mall_Customers.csv` contains:
- **CustomerID**: Unique customer identifier
- **Gender**: Male/Female
- **Age**: Customer age
- **Annual Income (k$)**: Income in thousands
- **Spending Score (1-100)**: Spending behavior score

The dataset has 200 rows with no missing values.

## Repository Structure

- `Untitled-1.ipynb`: Jupyter Notebook with data exploration, preprocessing, clustering, and visualization
- `README.md`: This file
- (Note: `Mall_Customers.csv` is not included; provide your own copy)

## Requirements

Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

Python version: 3.12.7

## Setup and Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/customer-segmentation.git
   cd customer-segmentation
   ```

2. **Add Dataset**:
   Place `Mall_Customers.csv` in the project directory or update the file path in the notebook:
   ```python
   df = pd.read_csv('Mall_Customers.csv')
   ```

3. **Run the Notebook**:
   - Open `Untitled-1.ipynb` in Jupyter Notebook/Lab
   - Execute cells to:
     - Explore data (`head`, `info`, `describe`)
     - Preprocess: Convert Gender to binary, standardize features
     - Cluster: Apply KMeans (9 clusters)
     - Visualize: Pie chart (cluster distribution), box plot (spending scores)

## Code Fixes Needed

- **KMeans Import**: Change `import sklearn.cluster as kmeans` to `from sklearn.cluster import KMeans`
- **Column Name**: Fix `df['k_Meam']` to `df['k_Means']` (ensure `model.labels_` is assigned)
- **File Path**: Update absolute path to relative path
- **Cluster Count**: 9 clusters may not be optimal; consider the elbow method

## Visualizations

- **Pie
