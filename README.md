# PROJECT-4-Machine-learning-CUSTOMER-SEGMENATATION-BASED-ON-SPENDING


#### **Introduction**
Customer segmentation is a crucial task in marketing analytics, allowing businesses to categorize customers based on purchasing behavior. This project applies **K-Means clustering** to segment mall customers based on their **Annual Income** and **Spending Score**, helping businesses target different customer groups effectively.

---

### **Dataset Overview**
The dataset used is **Mall_Customers.csv**, containing the following features:
- **CustomerID** – Unique customer identifier.
- **Gender** – Male/Female.
- **Age** – Customer's age.
- **Annual Income (k$)** – The customer’s yearly income.
- **Spending Score (1-100)** – A score assigned based on customer behavior.

---

### **Data Preprocessing**
1. **Data Loading**: The dataset is uploaded and read using `pandas`.
2. **Basic Exploration**:
   - `df.head()`, `df.shape()`, `df.describe()`, `df.info()` to understand dataset structure.
   - Checking for missing values using `df.isnull().sum()`.
3. **Feature Selection**: Extracting **Annual Income** and **Spending Score** as input variables (`X`).

---

### **K-Means Clustering**
1. **Elbow Method for Optimal Clusters**:
   - The **WCSS (Within-Cluster Sum of Squares)** is calculated for different cluster values (1 to 10).
   - The **Elbow Point Graph** helps determine the optimal number of clusters.

2. **Applying K-Means**:
   - The optimal cluster count is chosen (here, **5 clusters**).
   - The K-Means algorithm groups customers into clusters.

---

### **Visualization**
1. **Elbow Point Graph**:
   - A **line plot** of WCSS vs. the number of clusters to find the ideal cluster count.

2. **Customer Clusters**:
   - A **scatter plot** with different colors representing distinct customer segments.
   - **Centroids of clusters** are marked to show the center of each group.

---

### **Conclusion**
This project successfully clusters customers based on their spending behavior and annual income. Businesses can use these insights to **personalize marketing strategies**, **offer targeted promotions**, and **improve customer retention**. The **K-Means model** effectively groups customers into meaningful categories, helping businesses understand their audience better.

