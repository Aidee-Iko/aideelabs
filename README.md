
# Financial Hub Loan Analysis
### Dashboard Link:![Image](https://github.com/user-attachments/assets/6138a8f4-a939-4431-b432-a5d8429ec92a)
## Problem Statement
This dashboard helps this financial institution understand their customers better, it helps the institution know the loan amount they issue per year by monthly basis, the grand total of loan issued and percentage interest rate by these loan transactions. It also lets them know the top customers by location, loan verification status and identify risks associated by their transaction; thus by risk grades, the hub is attracting creditworthy borrowers and there is a lower likelihood of defaults.

Since the average number of high risk customers (1.38%) are LOWER THAN low risk customers (almost 63%), this financial loan hub should offer competitive interest rates to attract more low-risk customers while expanding lending to medium-risk customers with controlled exposure.

Aditionally, since a higher percentage status verification of borrower(customers) information is not verified, loan approval for "not verified" applicants should be limited, "source verified" applicants should be encouraged to complete verification AND "verified" applicants should be rewarded with lowest interest rates as a form of motivation for lagging customers to complete their verification process.

### Steps Followed
- Step 1 : Load data into Power BI desktop, dataset is xlsx file.
- Step 2 : Open Power Query editor & in view tab under Data preview section, check "column distribution", "column quality" &"column profile" options.
- Step 3 : It was observed that all columns were valid.
- Step 4 : A new column was created for issue_date
- Step 5 : In the report view, under the view tab, theme was selected.
- Step 6 : Visualization was carried out on the report design area and visuals formatted accordingly.
- Step 7 : Visual filters(slicers) were added for four fields named "loan status", "issue_date monthly", "loan amount" & "employment length".
- Step 8 : A bar chart was also added to the report design area representing the debt-to-income ratio of loan by customers verification status.

For creating new column the following DAX expressions was written,

Month Name = FORMAT(nexus[issue_date],"mmmm")


A card visual was used to represent count of customers(Loan Applications)

![Image](https://github.com/user-attachments/assets/e129ef81-e9f5-4724-8e8a-15952164f656)

A card visual was used to represent the percentage interest rate generated from the loan transactions.

![Image](https://github.com/user-attachments/assets/de76e8f3-65b1-44b0-9b0e-df1b6f6c70df)
A card visual was used to represent the total loan amount issued.

![Image](https://github.com/user-attachments/assets/6b4bc277-4a78-476e-b391-989f12e040df)

Snap of Loan Status by customers

![Image](https://github.com/user-attachments/assets/eebb7ca4-b793-480d-9eef-ddccc6f0abef)

## Snapshot of Dashboard (Power BI Desktop)

![Image](https://github.com/user-attachments/assets/b117df54-696a-4eb3-bf1d-58245f9ec769)

### Loan Application Type
- 100% customers applied for individual loans
### Customers by housing Type
- Top - Mortgage
- Second - Rent
- Third - Own
- Least - Other
### Loan status by Customers
- 90.38% Fully paid
- 9.62% Charged off 
### Top 3 Customers by Address
- California
- Florida 
- Texas
### Top 3 Months by Loan issued
- November 
- October
- Septenber
### Risk Grades Range
- 62.53% AVG Low risks(A, B, C)
- 11.03% Medium risks(D)
- 1.38% AVG High risks(E, F)

