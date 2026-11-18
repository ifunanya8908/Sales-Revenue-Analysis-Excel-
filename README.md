Sales Revenue Analysis (Excel)

An Excel data cleaning, modelling and visualization project. It takes a customer sales dataset of 17,422 records and answers: Where does the revenue come from, and who generates it?

Dataset

Each row is one customer order, with these columns:

CustomerID, Gender, MaritalStatus, YearlyIncome, Revenue, OrderDate, Country, BirthDate, Firstname, Lastname

What I Did

Stage 1: Data Exploration

Used COUNTA, MIN, MAX, SUM and AVERAGE to profile the data.

Question	Answer
Columns (variables)	10
Rows (records)	17,422
Minimum revenue	2.53
Maximum revenue	5,398.35
Total revenue	£21,764,629
Average revenue	1,249.26


Stage 2: Data Preparation

Added six new columns to the data table:

Year and YearMonth (from OrderDate) using YEAR and TEXT
Weekday using TEXT
CustomerName (first and last name merged, lowercase) using LOWER
CustomerAge (age at the time of order) using DATEDIF
AgeBand using IFS: Teenager (13-19), Young Adult (20-34), Adult (35-49), Seniors (50-64), Elderly (65+)
CustomerValue using IFS: Casual Buyers (up to 1,500), Brand Seekers (1,501-2,500), Convinced Seekers (above 2,500)


Stage 3: Analysis

Built a summary table of total revenue by country and gender using SUMIFS, with totals and a grand total.


Stage 4: Data Visualization Revenue by Country: 

column chart Proportion of Revenue by Age Band: pie chart
Revenue by Male and Female in each Country: clustered column chart
Key Findings
Australia generates the most revenue (about £7.1M, roughly a third of the total), followed by Southwest (£3.6M) and the United Kingdom (£2.9M).
Adults (35-49) are the biggest age band at about 47% of revenue, followed by Seniors (35%).
Male customers contributed £11.7M and female customers £10.0M.
Northeast, Southeast and Central contribute very little revenue.
Tools and Skills
Microsoft Excel
Functions: YEAR, TEXT, LOWER, DATEDIF, IFS, SUMIFS, SUM, MIN, MAX, AVERAGE
Excel Tables, data cleaning, summary tables, charts
Files
Sales-Revenue-Analysis-Excel.xlsx: the full workbook
Excel project sheet: the dataset with the new columns, and the Stage 3 summary table
Project Answer sheet: Stage 1 answers and Stage 4 charts



Author

Ifunanya F. Onyekwelu
