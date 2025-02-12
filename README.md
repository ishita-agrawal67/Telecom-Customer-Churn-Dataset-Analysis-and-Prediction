# Telecom-Customer-Churn-Dataset-Analysis-and-Prediction using R Studio
Here is a step-by-step process for **Telecom Customer Churn Analysis and Prediction** based on the document I have uploaded. 

### **Step 1: Data Collection**
- The dataset used is a **Telecom Customer Churn dataset** in an Excel file.
- It contains **7,043 rows and 23 columns** with customer details such as demographics, service subscriptions, account information, and whether they churned or not.

### **Step 2: Data Cleaning**
1. **Loading the Data:**
   - The dataset is read into a variable.
   - The first few rows and dataset dimensions are checked to understand the structure.

2. **Handling Missing Values:**
   - **TotalCharges column** has missing values.
   - The median value of **TotalCharges** is calculated.
   - Missing values are replaced with this median.

3. **Checking for Duplicate Values:**
   - The dataset is checked for duplicate records.
   - No duplicates were found.

4. **Converting Data Types:**
   - Columns with categorical data (e.g., Gender, Contract, Payment Method) are converted to factor type to facilitate analysis.

5. **Removing Unnecessary Columns:**
   - The **customerID column** is removed since it does not contribute to churn prediction.

6. **Checking for Outliers:**
   - A **boxplot** is used to detect and visualize outliers.

### **Step 3: Exploratory Data Analysis (EDA)**
EDA is performed to understand patterns and relationships in the data.

1. **Summary Statistics:**
   - Descriptive statistics are generated to get an overview of numeric and categorical variables.

2. **Correlation Matrix & Heatmap:**
   - A **correlation matrix heatmap** is created to analyze relationships between numerical variables.

3. **Visualizations:**
   - **Bar Charts:**
     - Distribution of **Internet Service types** (Fiber Optic, DSL, No Service).
     - Distribution of **Payment Methods** (Electronic Check, Credit Card, Bank Transfer, Mailed Check).
     - Distribution of **Contract Types** (Month-to-Month, One Year, Two Year).
     - **Gender distribution** of customers.

   - **Insights:**
     - Fiber optic is the most used internet service.
     - Electronic check is the most common payment method.
     - Most customers prefer **month-to-month contracts**.
     - The gender distribution is nearly equal.

### **Step 4: Data Preprocessing for Model Training**
1. **Encoding Categorical Variables:**
   - Convert categorical variables into a format suitable for machine learning (e.g., one-hot encoding or label encoding).

2. **Feature Selection:**
   - Important features that affect churn are identified.

3. **Splitting Data:**
   - The dataset is divided into **training** and **testing** sets.

### **Step 5: Model Training & Prediction**
1. **Selecting a Model:**
   - Different machine learning models are considered, such as:
     - **Logistic Regression**
     - **Decision Tree**
     - **Random Forest**
     - **Support Vector Machine (SVM)**
     - **Gradient Boosting (XGBoost)**

2. **Training the Model:**
   - The chosen model is trained using the training dataset.

3. **Evaluating Model Performance:**
   - The model is tested on the test dataset.
   - Performance metrics are calculated, such as:
     - **Accuracy**
     - **Precision**
     - **Recall**
     - **F1-score**
     - **Confusion Matrix**

### **Step 6: Model Optimization**
- The best-performing model is optimized using techniques like:
  - **Hyperparameter tuning** (adjusting model parameters).
  - **Cross-validation** to prevent overfitting.

### **Step 7: Predictions & Business Insights**
- The final model predicts whether a customer is likely to **churn or stay**.
- Business decisions can be made based on:
  - Which customer segments are more likely to churn.
  - What factors contribute most to churn (e.g., contract type, monthly charges, internet service).
  - Strategies to **reduce churn**, such as offering better contracts or discounts.

### **Conclusion**
This step-by-step process covers everything from **data collection to churn prediction**. 
