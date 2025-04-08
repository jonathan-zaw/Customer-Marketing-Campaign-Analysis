# Customer-Marketing-Campaign-Analysis
This project involves exploratory data analysis (EDA) of a marketing campaign dataset using Python (Pandas, NumPy, Seaborn, Matplotlib). The goal was to analyze customer demographics, purchasing behavior, and campaign responses to uncover meaningful insights that could help optimize future marketing strategies.



## Dataset Overview

The dataset consists of 2,240 records and 29 columns related to customer information, purchases, and marketing campaign responses. It includes:

- **Demographics**: Year of birth, education, marital status, income, household size
- **Purchase Behavior**: Amount spent on various product categories
- **Campaign Interaction**: Response to multiple marketing campaigns
- **Engagement Metrics**: Web, catalog, and store purchases, website visits

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Steps Performed

### 1. **Data Loading and Initial Inspection**
- Loaded the dataset (`marketing_campaign.csv`) using `pandas.read_csv()`
- Checked dataset shape, column info, and missing values
- Found 24 missing values in the `Income` column and imputed them using the median

### 2. **Data Cleaning**
- Dropped irrelevant columns: `Z_CostContact` and `Z_Revenue`
- Standardized `Education` values:
  - Merged: `'PhD'`, `'2n Cycle'`, `'Graduation'`, `'Master'` → `'Post Graduate'`
  - `'Basic'` → `'Under Graduate'`
- Cleaned `Marital_Status` values:
  - Merged: `'Married'`, `'Together'` → `'Relationship'`
  - Merged: `'Divorced'`, `'Widow'`, `'Alone'`, `'YOLO'`, `'Absurd'` → `'Single'`

### 3. **Univariate Analysis**
Conducted detailed distribution analysis of:
- **Year_Birth**: Examined birth years to understand customer age distribution
- **Education**: Categorized and visualized education levels
- **Marital_Status**: Analyzed relationship status of customers
- **Income**: Explored income distribution with descriptive statistics and plots

Used bar plots and count plots to visualize distributions and identify potential outliers or skewness in individual variables.

---

##  Key Visualizations

- Bar plot of customer count by `Education`
- Count plot for `Marital_Status`
- Histogram of `Income` to check skewness
- Bar chart of customer distribution by `Year_Birth`

---

##  Insights Gained

- Majority of the customers are in a relationship and hold a postgraduate degree
- Income distribution is right-skewed, indicating a few high-income customers
- The dataset is clean and well-structured, suitable for segmentation or clustering models
