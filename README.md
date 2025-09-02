# Customer Segmentation using K-Means Clustering

## Objective
Perform customer segmentation based on income and spending behavior using **K-Means clustering**.  
The goal is to identify groups of customers that share similar characteristics, enabling targeted marketing strategies.

## Dataset
- **Source**: Mall Customers Dataset (Kaggle or similar)  
- **Features Used**:  
  - `Annual Income (k$)`  
  - `Spending Score (1-100)`  

## Tools & Libraries
- **Python**  
- **Pandas**: Data manipulation  
- **Scikit-learn**: Standardization & Clustering  
- **Matplotlib**: Visualization  

---

## Steps

### 1. Data Preparation
- Loaded dataset with `pandas.read_csv()`  
- Dropped missing values with `df.dropna()`  
- Explored dataset using `.describe()`  

### 2. Feature Selection & Scaling
- Selected key features: `Annual Income (k$)`, `Spending Score (1-100)`  
- Standardized features using `StandardScaler`  

### 3. Finding Optimal Number of Clusters
- Used **Elbow Method** by plotting inertia values for `k = 1 to 8`  
- Chose **k = 5** as the optimal number of clusters  

### 4. K-Means Clustering
- Applied **KMeans** with 5 clusters  
- Assigned cluster labels to each customer  

### 5. Cluster Profiling
Defined customer segments based on income and spending patterns:  
- **High Value**: High income, high spending  
- **Conservative**: High income, low spending  
- **Aspirational**: Low income, high spending  
- **Constrained**: Low income, low spending  
- **Balanced**: Middle range customers  

### 6. Visualization
- Plotted customer segments with scatter plots  
- Colored points by cluster categories  
- Added labels for interpretation  

---

## Results
- Successfully segmented customers into **5 distinct groups**  
- Provided interpretable labels for business insights  
- Final visualization clearly highlights differences in income vs. spending behavior  

---

## How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/yourusername/customer-segmentation.git
   cd customer-segmentation
