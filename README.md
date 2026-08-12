# Sales_Performance_Forecasting
# Sales Performance & Forecasting Analysis

## Internship Assessment Project — Python & Data Science

This project performs an end-to-end analysis of a retail sales dataset to understand sales performance, identify important sales patterns, visualize business trends, and forecast future monthly sales using a machine learning regression model.

The project was completed as part of a Python & Data Science internship assessment.

---

## 📌 Project Overview

The main objective of this project is to analyze retail sales data and understand how sales vary across different time periods, product categories, regions, customer segments, sub-categories, and products.

The project also uses **Linear Regression** to forecast future monthly sales.

### Main Project Workflow

```text
Data Collection
       ↓
Data Loading
       ↓
Data Inspection
       ↓
Data Cleaning
       ↓
Statistical Analysis
       ↓
Exploratory Data Analysis
       ↓
Data Visualization
       ↓
Monthly Sales Analysis
       ↓
Linear Regression Model
       ↓
Model Evaluation
       ↓
Future Sales Forecast
       ↓
Business Insights
       ↓
Business Recommendations
```

---

## 🎯 Objectives

The main objectives of this project are:

* Load and inspect the retail sales dataset.
* Identify and handle missing values.
* Identify and remove duplicate records.
* Correct inappropriate data types.
* Convert order and shipping dates into proper date formats.
* Perform statistical analysis of sales.
* Analyze sales trends over time.
* Analyze sales by category and sub-category.
* Analyze sales performance by region.
* Analyze customer segment performance.
* Identify the top-performing products.
* Build a monthly sales forecasting model.
* Use Linear Regression for sales prediction.
* Evaluate the model using RMSE and R².
* Forecast future monthly sales.
* Generate business insights and recommendations.

---

## 📊 Dataset

The project uses a retail **Superstore Sales Dataset**.

The dataset contains information about orders, customers, products, locations, categories, dates, and sales.

### Dataset Source

The dataset was provided as part of the internship assessment and is based on the Superstore Sales Dataset available through Kaggle.

---

## 📋 Dataset Columns

The dataset used in this project contains the following columns:

| Column        | Description                         |
| ------------- | ----------------------------------- |
| Row ID        | Unique row identifier               |
| Order ID      | Unique order identifier             |
| Order Date    | Date on which the order was placed  |
| Ship Date     | Date on which the order was shipped |
| Ship Mode     | Shipping method used                |
| Customer ID   | Unique customer identifier          |
| Customer Name | Name of the customer                |
| Segment       | Customer segment                    |
| Country       | Country of the customer             |
| City          | Customer city                       |
| State         | Customer state                      |
| Postal Code   | Postal code of the customer         |
| Region        | Sales region                        |
| Product ID    | Unique product identifier           |
| Category      | Product category                    |
| Sub-Category  | Product sub-category                |
| Product Name  | Name of the product                 |
| Sales         | Sales amount                        |

---

## 🛠️ Technologies and Tools

The following technologies and Python libraries were used:

* **Python 3**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**

---

## 🧹 Data Cleaning

The following data-cleaning activities were performed:

### 1. Dataset Inspection

The dataset was inspected to understand:

* Number of rows
* Number of columns
* Column names
* Data types
* First few records

### 2. Missing Values

Missing values were checked using:

```python
df.isnull().sum()
```

Missing values, where applicable, were handled appropriately.

### 3. Duplicate Records

Duplicate records were identified using:

```python
df.duplicated().sum()
```

Duplicate rows were removed using:

```python
df = df.drop_duplicates()
```

### 4. Date Conversion

The `Order Date` and `Ship Date` columns were converted into proper datetime format.

The dataset contains dates in day/month/year format, so `dayfirst=True` was used where required.

### 5. Date Features

Additional time-related information was extracted from `Order Date`, including:

* Year
* Month
* Month Name
* Monthly sales period

---

# 📈 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the sales performance of the business.

The project contains more than five different visualizations.

---

## 1. Monthly Sales Trend

A line chart was created to analyze how total sales changed over time.

### Purpose

The monthly sales trend helps identify:

* Sales growth
* Sales decline
* High-sales periods
* Low-sales periods
* Possible seasonal patterns

---

## 2. Sales by Category

A bar chart was created to compare sales across product categories.

### Purpose

This analysis helps identify the product categories generating the highest and lowest sales.

---

## 3. Sales by Region

Sales were grouped by region and visualized using a bar chart.

### Purpose

This analysis helps identify:

* High-performing regions
* Low-performing regions
* Regional sales differences

---

## 4. Sales by Customer Segment

Sales were analyzed according to customer segment.

### Purpose

This helps understand which customer segments contribute the most to overall sales.

---

## 5. Sales by Sub-Category

Sales were grouped by product sub-category.

### Purpose

This analysis helps identify the strongest and weakest product sub-categories.

---

## 6. Top 10 Products by Sales

The top 10 products were identified based on total sales.

### Purpose

This analysis helps identify the products that contribute most to revenue.

---

# 📊 Statistical Analysis

Statistical analysis was performed on the `Sales` column.

The following statistical measures were calculated:

* Mean
* Median
* Standard deviation
* Minimum
* Maximum
* Quartiles

Example:

```python
df['Sales'].describe()
```

### Key Statistical Measures

The final values are available in the Jupyter Notebook generated for this project.

---

# 🤖 Machine Learning — Sales Forecasting

## Model Used

**Linear Regression**

The project uses Linear Regression to forecast monthly sales.

The monthly sales dataset was created by aggregating sales according to the order date.

### Input Variable

```text
Month Number
```

### Target Variable

```text
Sales
```

The data was divided chronologically into:

```text
80% → Training Data
20% → Testing Data
```

The model was trained using the training data and then used to predict sales for the testing period.

---

# 📏 Model Evaluation

The regression model was evaluated using the following metrics:

## RMSE

**Root Mean Squared Error (RMSE)** measures the average magnitude of prediction errors.

A lower RMSE generally indicates smaller prediction errors.

## R² Score

**R² Score** measures how well the model explains the variation in the target variable.

A value closer to 1 indicates a stronger model fit.

The actual RMSE and R² values generated from the dataset are available in the Jupyter Notebook.

---

# 🔮 Future Sales Forecast

After training the Linear Regression model, the model was used to forecast sales for the next six months.

The forecast output contains:

| Month          |   Forecasted Sales |
| -------------- | -----------------: |
| Future Month 1 | Generated by model |
| Future Month 2 | Generated by model |
| Future Month 3 | Generated by model |
| Future Month 4 | Generated by model |
| Future Month 5 | Generated by model |
| Future Month 6 | Generated by model |

The exact forecast values are available in the Jupyter Notebook.

---

# 💡 Key Insights

The following insights were obtained from the exploratory analysis:

### Insight 1 — Sales Trend

Monthly sales were analyzed to identify changes in sales performance over time and understand periods of higher and lower demand.

### Insight 2 — Product Performance

Category and sub-category analysis helps identify which product groups contribute most to overall sales.

### Insight 3 — Regional Performance

Sales vary across regions, providing opportunities to develop targeted strategies for lower-performing regions.

> **Note:** The specific numerical findings and rankings should be taken from the final outputs of the Jupyter Notebook.

---

# 💼 Business Recommendations

Based on the analysis, the following recommendations can be considered:

### 1. Focus on High-Performing Categories

Marketing and inventory planning should prioritize categories and sub-categories that generate higher sales.

### 2. Improve Lower-Performing Regions

Regions with comparatively lower sales can be targeted with region-specific promotions and marketing campaigns.

### 3. Improve Inventory Planning

Monthly sales trends and forecasts can be used to plan inventory levels before periods of expected higher demand.

### 4. Promote High-Performing Products

The top-performing products can receive greater promotional attention to maintain strong sales performance.

### 5. Use Forecasting for Sales Planning

The sales forecasting model can be used as a supporting tool for future sales and inventory planning.

---

# 📁 Project Structure

```text
sales-performance-forecasting/
│
├── Sales_Performance_Forecasting.ipynb
│
├── README.md
│
└── screenshots/
    ├── dataset.png
    ├── data_cleaning.png
    ├── monthly_sales.png
    ├── category_sales.png
    ├── region_sales.png
    ├── segment_sales.png
    ├── subcategory_sales.png
    ├── top_products.png
    └── model_evaluation.png
```

---

# ▶️ How to Run the Project

## Step 1 — Clone the Repository

Clone or download this GitHub repository.

## Step 2 — Install Required Libraries

Open Command Prompt or Anaconda Prompt and run:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Step 3 — Open Jupyter Notebook

Run:

```bash
jupyter notebook
```

## Step 4 — Open the Notebook

Open:

```text
Sales_Performance_Forecasting.ipynb
```

## Step 5 — Add the Dataset

Place the required CSV dataset in the appropriate location used by the notebook.

## Step 6 — Run the Notebook

Run the notebook cells sequentially from beginning to end.

---

# 📌 Project Results

The project provides:

* Cleaned retail sales data
* Statistical sales analysis
* Multiple sales visualizations
* Category analysis
* Regional analysis
* Customer segment analysis
* Product performance analysis
* Monthly sales analysis
* Linear Regression model
* RMSE evaluation
* R² evaluation
* Future sales forecasts
* Business insights
* Business recommendations

---

# 📷 Screenshots

Screenshots of the following outputs can be added to the repository:

* Dataset preview
* Data cleaning
* Statistical summary
* Monthly sales trend
* Category sales
* Region sales
* Customer segment sales
* Sub-category sales
* Top 10 products
* Model evaluation
* Future sales forecast

---

# 📄 Internship Submission

The internship assessment requires a PDF report containing:

* Project Description
* Screenshots of Code
* Charts and Output
* Key Insights
* Business Recommendations
* GitHub Repository Link

The completed project is submitted according to the internship assessment instructions.

---

# 👨‍💻 Author

**Abhijit Ramchandra Pawar**

MSc Data Science

---

## ⭐ Conclusion

This project demonstrates an end-to-end Python and Data Science workflow for retail sales analysis and forecasting. It combines data cleaning, statistical analysis, exploratory data analysis, visualization, machine learning, model evaluation, and business recommendations to support data-driven sales planning.
