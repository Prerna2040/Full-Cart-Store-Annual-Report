# Full-Cart-Store-Annual-Report

**Project Description:**
This project involves analyzing the annual sales report for the Full Cart Store. The analysis includes data cleaning, transformation, and visualization to provide insights into various aspects of the store's performance in 2022.

**Data Cleaning:**
Spelling Corrections: Corrected spelling mistakes in the Channel column (e.g., "AMenazon" to "Amazon", "menyntra" to "Myntra", "Meneesho" to "Meesho").

Quantity: Standardized the 'Qty' column to ensure all quantities are numeric.

**Data Transformation:**
Age Group Classification: Created a new column 'Age-Group'to categorize customers into "Senior", "Adult", and "Teenager" based on their age:
  Formula: =IF(E2>50,"Senior",IF(E2>=30,"Adult","Teenager"))

Month Extraction: Created a 'Month' column to extract the month from the Date column:
  Formula: =TEXT(G2,"MMMM")

State Identification: Created a 'State' column to identify the state where the order was delivered using a VLOOKUP with a separate sheet containing city and state information:
  Formula: =VLOOKUP(Q2,LOCATION!$A$2:$B$1906,2,0)

**Visualizations:**
Using pivot tables and charts, the following key insights were visualized:

Order vs Sale: Sum of amount and count of order IDs over the months.
Sales by Gender: Comparison of sales between men and women.
Order Status: Distribution of order statuses (delivered, returned, refunded, canceled).
Orders by Channel: Distribution of orders across different sales channels (Amazon, Myntra, Flipkart, etc.).
Sales by State: Top 10 states by sales amount.
Orders by Age and Gender: Distribution of orders across different age groups and genders.

**Report:** 
![image](https://github.com/user-attachments/assets/639a81c8-64d9-4a10-9b30-1b290a25aca2)

Key Results:
Total Sales: The total sales amount for 2022 was significantly higher in the first half of the year, peaking in April.
Gender Distribution: Women accounted for 64% of the total sales, while men accounted for 36%.
Order Status: 92% of the orders were successfully delivered, with only 8% being returned, refunded, or canceled.
Top Channels: Amazon was the leading sales channel, followed by Flipkart and Myntra.
Top States: Maharashtra, Karnataka, and Uttar Pradesh were the top-performing states in terms of sales.

**Conclusion:**
The analysis provides a comprehensive overview of the Full Cart Store's performance in 2022, highlighting key areas such as sales trends, customer demographics, and order distribution across different channels and states.
