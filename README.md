
# Nexus Financial Hub
### Dashboard Link: Available soon
## Problem Statement
This dashboard helps this financial institution understand their customers better, it helps the institution know the loan amount they issue per year by monthly basis, the grand total of loan issued and percentage interest rate by these loan transactions. It also lets them know the top customers by location, and identify risks associated by their transaction; thus by risk grades, the hub is attracting creditworthy borrowers and there is a lower likelihood of defaults.

Since the average number of high risk customers (almost 18% ) are lower than low risk customers (almost 78%), this financial loan hub should offer competitive interest rates to attract more low-risk customers while expanding lending to medium-risk customers with controlled exposure.


### Steps Followed
- Step 1 : Load data into Power BI desktop, dataset is xlsx file.
- Step 2 : Open Power Query editor & in view tab under Data preview section, check "column distribution", "column quality" &"column profile" options.
- Step 3 : It was observed that all columns were valid.
- Step 4 : A new dataset was added, which led to the creation of a "bridge table" where relationship was created between the new and already existing dataset.
- Step 5 : In the report view, under the view tab, theme was selected.
- Step 6 : Visualization was carried out on the report design area and visuals formatted accordingly.
- Step 7 : Visual filters(slicers) were added for four fields named "loan status", "home ownership", "loan amount" & "employment length".
- Step 8 : A bar chart was also added to the report design area representing the purpose of loan by customers.

For creating new column the following DAX expressions was written,

Month Name = FORMAT(Sheet1[issue_date],"mmmm")


A card visual was used to represent count of customers(Loan Applications)


![Image](https://github.com/user-attachments/assets/fec7082f-5a77-4024-a892-b5b63bda8aea)

- Step 9 : A "BridgeTable" was created to form a relationship between the two sheets used in the analysis.

The following DAX expression was written,

BridgeTable = DISTINCT(SELECTCOLUMNS(Sheet1, "member_id", Sheet1[member_id]))

A card visual was used to represent the percentage interest rate generated from the loan transactions.

![Image](https://github.com/user-attachments/assets/4d38afe8-aa75-4f88-b196-a39eee9eb333)


A card visual was used to represent the total loan amount issued.

![Image](https://github.com/user-attachments/assets/7be7aaa2-e31e-4e20-b396-3e37ff853bb5)

Snap of Loan Status by customers

![Image](https://github.com/user-attachments/assets/5a0037ff-fd06-46c3-bac5-dda3c5b0bdc3)

- Step 10 : The report was then published to Power BI Service.

## Snapshot of Dashboard (Power BI Desktop)

![Image](https://github.com/user-attachments/assets/5eeaed11-639c-4611-91c0-543362471183)

### Loan Application Type
- 100% customers applied for individual loans
### Customers by housing Type
- Top - Rent 
- Second - mortgage
- Least - Own
### Loan status by Customers
- 82.07% Fully paid
- 14.12% Charged off
- 3.81%  Current 
### Top 3 Customers by Address
- California
- New York 
- Texas
### Top 3 Months by Loan issued
- September 
- October
- November
### Risk Grades Range
- 77.7% AVG Low risks(A, B, C)
- 48.91% Medium risks(D)
- 17.4% AVG High risks(E, F, G)
### Top 3 Purpose for Loan
- Debt consolidation
- Credit card
- Home improvement

