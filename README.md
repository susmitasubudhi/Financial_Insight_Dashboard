# Financial_Insight_Dashboard
## Project Objective
  A financial organization wants to develop an interactive Finance Analytics Dashboard using Power BI to monitor and analyze transaction performance, customer 
  behavior, revenue generation, and financial trends
  The management team requires a centralized dashboard to gain insights into:
  - Overall transaction growth and financial performance 
  - Monthly trends in transaction amounts
  - Successful vs failed transactions
  - Customer segment contribution
  - State-wise financial performance 
  - Transaction type profitability 
  - Gender-based customer analysis 
  - Year-over-Year (YoY) performance changes
### The dashboard will help stakeholders identify business trends, improve decision-making, optimize transaction strategies, and monitor financial health.
  - Monitor KPIs in real time. 
  - Identify high-performing customer segments and states. 
  - Analyze transaction patterns and trends.
  - Track operational fees and taxes 
  - Understand customer demographics .
  - Improve financial decision-making and business strategy.

### The dashboard should allow users to dynamically filter data by:
  -	Year 
  -	Dynamic Measure 
  -	Occupation 
  -	Category 
## Questions(KPI)
  - What is the total transaction amount generated across different years?
  - How many transactions were completed and how does the transaction volume change over time?
  - What is the total fee generated from transactions?
  - What is the total tax collected from financial transactions?
  - What is the average transaction value and how does it vary yearly?
  - How does the current year’s financial performance compare with the previous year (YoY growth/decline)?
  - Dynamic Year Filter.
  - Dynamic Measures.
## Process
### Data Collection
  - The Finance Analytics dataset used for this project was obtained from publicly available learning resources.
### Data Cleaning and Preparations
  - Removing Duplicates, Handling Missing Values.
  - Converted Date fields to proper date/time format.
  - Created a dedicated Calendar Table from the transaction date column to enable time-based analysis.
    - Date
    - Year
    - Month
    - Month Number
 - Created Different Measures.
### Data Modelling
  - Modeled Data in a Star Schema ,Relationship between Fact Table(Finance_transaction) and Dimension Taable (Customers) and (Calender Table).
  - Established a one-to-many relationship between the Calendar table and Finance transaction table.
### Dashboard Creation
  - Use a BI tool to create a vizualization
  - Built a 2 Page Report
    - Same Period Last year Comparision
    - Breakdown By States,Gender, Transaction_status, Customer_segment.
    - Added drill-through functionality to provide detailed insights from summary visuals.
    - Users can select any data point and navigate to a detailed view showing related transaction-level information.
### Testing and Validations
  - Verified DAX measures and dashboard visuals for data accuracy and consistency.
  - Tested report interactions, filters, and slicers to ensure proper functionality.
### Data Model Architecture
  The project uses a star schema data model with a Finance fact table connected to Customer and Date dimension tables for efficient analysis and reporting.
       <img width="1097" height="588" alt="Data Model" src="https://github.com/user-attachments/assets/6cc18e58-186a-4051-8206-d269edfb29ed" />

## Dashboard
 - Overview Analysis
   - Total Amount, total Tax, total fees, total Transactions By month.
   - Total Amount, Tax,Fees, Transactions by transaction status.
   - Total amount,tax,fees,transactions by customer segment.
   - Total Amount, Tax,Fees, Transactions by State.
   - Transaction Type Analysis
   - Total Amount, Tax,Fees, Transactions by gender.
   - Dynamic Slicers (Year,Metrics)
   - Dynamic metrics(Total Amount,Total Tax, Total Fees, Total Transaction)
   - Slicers (Occupations, Category)
   - Added page navigation buttons to allow users to switch between different report sections easily.
   - Cards(Total Amount,Total tax, Total Fees, Total Transactions, Avg Transaction).
   - Implemented previous year comparison using DAX time intelligence.
   - Displays percentage growth or decline against the previous year's performance.
 - Transactions
   - Created a dedicated transaction detail page displaying complete transaction-level information.
   - Added drill-through functionality to allow users to navigate from summary visuals to detailed records.
   - Users can select a specific data point and view related transaction details based on applied filters.
   - Implemented slicer synchronization across multiple report pages.


 (For Example):
     
<img width="1367" height="725" alt="Overview Analysis" src="https://github.com/user-attachments/assets/7b095f7c-52f5-40fb-a3b2-94835b17a0c9" />

<img width="1360" height="731" alt="Transactions" src="https://github.com/user-attachments/assets/0ee9e73b-afd3-4a50-a474-5bbb5b7f2df3" />

