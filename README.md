# 🛍️ Retail Sales Dataset Summary

This dataset, titled **Retail Sales Dataset - Master**, provides detailed transactional data for a retail business, including customer demographics, product categories, sales figures, and commission data. It is structured to support analysis across multiple dimensions such as age group, gender, product category, and generation.

## 📁 Dataset Overview

- **Customer Demographics**: Includes `Customer ID`, `Gender`, `Age`, and `Generation`.
- **Sales Data**: Captures `Transaction ID`, `Product Category`, `Quantity`, `Price per Unit`, and `Total Sales`.
- **Commission Data**: Contains commission rates for 2023 and 2024.
- **Temporal Data**: Includes `Day`, `Month`, `Year`, and full `Date` of transaction.

## 📊 Key Metrics and Aggregates

- **Average Total Sales by Generation and Product Category**:
  - Highest average sales observed in **Young Adults** for **Clothing**.
  - **Seniors** show strong performance in **Electronics**.

- **Total Sales by Gender and Product Category**:
  - Sales are nearly evenly split between **Male** and **Female** customers.
  - **Electronics** has the highest contribution to total sales.

## 🧠 Key Insights and Learnings

Through analysis of this dataset, I learned:

- **Generational Preferences**: Different age groups have distinct purchasing behaviors. For example, Young Adults tend to spend more on Clothing, while Seniors prefer Electronics.
- **Gender-Based Trends**: Both genders contribute almost equally to total sales, but their preferences vary slightly across product categories.
- **Product Category Performance**: Electronics consistently shows high sales and profit margins, making it a key category for revenue generation.
- **Commission Impact**: The inclusion of commission data allows for deeper analysis of profitability and sales incentives over time.

## 🧮 Excel Features and Formulas Used

To analyze and visualize the data, I applied several Excel features and formulas:

- **Pivot Tables**: Used to summarize total and average sales by `Generation`, and `Product Category`.

 ![Screenshot 2025-06-10 at 15 03 08](https://github.com/user-attachments/assets/8f687226-8ede-486f-b055-ad9709997bdb)
  
- **Sorting and Filtering**: Applied to identify top-performing students and products.

![Screenshot 2025-06-10 at 15 06 27](https://github.com/user-attachments/assets/cc04e281-30a4-471a-813b-73b601324154)
![Screenshot 2025-06-10 at 15 12 23](https://github.com/user-attachments/assets/92aff582-32ab-4398-ade1-45f5e2865fb5)

  
- **Formulas**:
  - `=AVERAGE(B2:D2)` – Calculated average scores for students.
  - `=MAX(B2:D2)` – Identified highest subject scores.
  - `=SUM(Quantity * Price per Unit)` – Computed total sales per transaction.
- **Conditional Formatting**: Highlighted highest and lowest average scores in the student performance table.
- **Data Validation**: Ensured clean input for fields like `Product Category` and `Generation`.

### 🔍 VLOOKUP Usage

I used the `VLOOKUP` function to:

- **Match Commission Rates**: Automatically retrieve the correct commission percentage for each transaction based on the year using a lookup table.
  - Example:  
    ```excel
    =VLOOKUP([@Year], CommissionTable, 2, FALSE)
    ```
- **Enrich Data**: Pull in additional customer or product details from reference tables to enhance the dataset for analysis.

This helped streamline data preparation and ensured consistency across the dataset.

## 🔍 Suggested Analyses

- Sales trends by **generation** and **product category**.
- Gender-based purchasing behavior.
- Commission impact on sales performance.
- Identifying top-performing students using Excel functions.

---
