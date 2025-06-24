# Cyber Security Breaches Analysis Dashboard

This Power BI dashboard provides comprehensive analysis of cybersecurity breaches within an organization, tracking key metrics, employee performance, and departmental/branch vulnerabilities.

**Key Features:**

**Dashboard Pages**

Home: High-level KPI overview with navigation to sub-pages

![Capture1](https://github.com/user-attachments/assets/d864d97b-5abc-46c4-8258-3503d017a7b3)

Employee Ranking: Leaderboard of top-performing employees in breach resolution

![Capture2](https://github.com/user-attachments/assets/d8c11ec5-8207-4909-ad90-4842f92e1423)

Department Analysis: Breach trends by department

![Capture3](https://github.com/user-attachments/assets/f8e59ce4-cbd2-4071-82e2-52ce2529b4f1)

Branch Analysis: Geographic distribution of breaches

![Capture4](https://github.com/user-attachments/assets/46515315-9403-48a1-8ea1-e46a3031b878)

Summary: Consolidated breach statistics

![Capture5](https://github.com/user-attachments/assets/4d064c61-78f2-4f77-ab30-52cecd9ad118)

**Key Performance Indicators (KPIs)**

   - Total Breaches
   - Open Breaches
   - Closed Breaches
   - Employee Strength
   - Average Breach Resolution Time
   - Estimated Stolen Data
   - Affected Employees
   - Secured Employees
   - Employees Identifying Breaches

**Table Relationships Overview**

The data model for this dashboard follows a star schema design (everything connects to the center) with fact and dimension tables. Here's how the tables relate to each other:

![Capture6](https://github.com/user-attachments/assets/db65f816-2636-4a21-b05e-aa976234d911)

- Main Breaches Table (FactCSB) - This is the center that holds all the actual breach records
- Each breach is linked to:
     - Which department it happened in
     - Which office location (branch)
     - What type of breach it was
     - Which employee found it
- Supporting Tables describe the details:
     - Department: Marketing, IT, HR etc.
     - Branch: New York, London, Tokyo offices
     - BreachType: Hacking, Lost Device, Insider Threat etc.
     - Employees: Who discovered each breach
     - Calculated Numbers (DAX Measures) - These do the math to create the dashboard numbers:
  

**NOTE: Counts open vs closed breaches**

Calculates how long breaches stay open

Works out percentages of affected employees

**Why This project Matters?**

Easy Filtering: Click a department to see only their breaches

Accurate Numbers: All calculations update automatically

Fast Performance: Designed to handle lots of data quickly

Consistent Reporting: Everyone sees the same numbers

**How to Run this Project?**

1- Download and install Power BI Desktop.

2- Open the Power BI project file: CarsSalesDashboard.pbix.

3- Go to Transform Data and update the file path to correctly point to the Excel data source on your local machine.

