# Myntra-Analysis
Data analysis on Myntra sales trend using python pandas seaborn.includes visualization ,daa preprocessing

# Myntra Sales Data Analysis

## Project Overview
This project analyzes Myntra's sales data using Python and Pandas. The dataset consists of three key tables:
1. **dim_products** - Contains product details such as category, sub-category, brand, size, color, and ratings.
2. **dim_customers** - Stores customer information including age, city, and state.
3. **fact_orders** - Contains order details such as order ID, customer ID, product ID, date, original price, and discount percentage.

## Data Preprocessing
- Loaded the dataset from an Excel file.
- Checked for missing values and data types using `.info()`.
- Verified the dataset for duplicate records using `.duplicated().sum()`.
- Extracted the month from the `Date` column and added a new column `Month`.
- Calculated the total price after applying discounts and added a new column `Total Price`.

## Data Analysis
- Aggregated total sales per month using `groupby()`.
- Merged the `orders` dataset with `products` dataset to include product details in the order data.
- Created a bar plot using `seaborn` to visualize monthly sales performance.

## Key Insights
- Sales are highest in **January, February, and March**, suggesting seasonal trends.
- Certain brands and categories contribute more to overall sales.
- Discounted products significantly impact total revenue.

## Visualization
- Used `seaborn` to generate a bar plot showing total sales by month.
- Used `matplotlib` for additional data exploration.

## Next Steps
- Perform customer segmentation based on purchasing behavior.
- Analyze top-selling product categories and brands.
- Investigate the impact of discounts on customer purchasing decisions.

## Technologies Used
- **Python** (Pandas, NumPy, Seaborn, Matplotlib)
- **Jupyter Notebook**
- **Excel** (for data storage and retrieval)

## How to Run
1. Ensure you have Python installed along with Pandas, NumPy, Seaborn, and Matplotlib.
2. Load the dataset using Pandas' `read_excel()` function.
3. Execute the provided scripts to analyze and visualize the data.


