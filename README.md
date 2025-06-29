
Diwali Sales Analysis

A comprehensive data analysis project to explore customer buying behavior during the Diwali festival season. The project includes data cleaning, exploratory data analysis (EDA), and insights generation using Python.

Dataset

The dataset contains customer transaction records with the following columns (before cleaning):

['User_ID', 'Cust_name', 'Product_ID', 'Gender', 'Age Group', 'Age', 
 'Marital_Status', 'State', 'Zone', 'Occupation', 'Product_Category', 
 'Orders', 'Amount', 'Status', 'unnamed1']

Data Cleaning

The raw data had inconsistencies such as unnecessary columns, extra whitespaces, missing values, and improper datatypes. Cleaning steps performed:

- Removed irrelevant columns: Cust_name, unnamed1, and Status
- Trimmed whitespace from column names
- Dropped missing (NaN) and duplicate values
- Converted Amount and Orders to numeric for accurate analysis
- Mapped Marital_Status from 0/1 to 'Married'/'Unmarried' for better readability

Final cleaned columns:

['User_ID', 'Product_ID', 'Gender', 'Age Group', 'Age', 'Marital_Status',
 'State', 'Zone', 'Occupation', 'Product_Category', 'Orders', 'Amount']

Exploratory Data Analysis (EDA)

Using Python libraries like Pandas, Matplotlib, and Seaborn, the following visualizations and insights were derived:

Key Visualizations:
- Gender-wise total sales
- Age group distribution of buyers
- State-wise order and sales volume
- Marital status vs purchase amount
- Occupation vs sales
- Product category preferences

Key Insights

- Female customers not only shop more but also spend more on average.
- Majority of buyers are married women aged 26–35 years.
- Most orders and highest sales come from Uttar Pradesh, Maharashtra, and Karnataka.
- Buyers are predominantly from IT, Healthcare, and Aviation sectors.
- Most popular categories include Food, Clothing, and Electronics.
- Customer Persona:
  Married women (26–35 years) from UP, Maharashtra, or Karnataka working in IT, Healthcare, or Aviation are the most likely to purchase during Diwali.

Project Structure

Diwali_Sales_Analysis/
├── data/
│   └── diwali_sales_data.csv
├── Diwali_Sales_Analysis.ipynb
├── README.txt
└── images/
    └── [visualizations & charts]

How to Run

1. Clone the repository:
   git clone https://github.com/your-username/diwali-sales-analysis.git
   cd diwali-sales-analysis

2. Launch the notebook:
   jupyter notebook Diwali_Sales_Analysis.ipynb

Tools & Libraries Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

Acknowledgments

- Dataset: Publicly available Diwali sales dataset
- Inspired by real-world customer behavior and sales analytics
