📊 Credit Risk Automation & Insight Dashboard (Power BI + Automation)

Overview: This project aims to fully automate the end-to-end workflow of credit data processing, analysis, and insight generation using Power BI and modern automation tools. 
It removes manual effort from repetitive tasks like downloading daily data, cleaning, combining, and dashboard refreshing — enabling real-time insights and smarter business decisions.

🧰 Tools & Technologies Used

* Power BI – To build rich visual dashboards and DAX-driven insights
* Power Automate – To automate:
  * Recurring dataset refresh
  * Email monitoring and attachment downloading
* Outlook Automation – Email fetching and file handling
* Python (Pandas, NumPy) – Data cleaning, aggregation, and logic building before dashboarding
* DAX (Data Analysis Expressions) – Used extensively to calculate:
  * Credit risk scores
  * LTV (Loan-to-Value) formulas
  * Custom KPIs and marketing logic
* Dynamic Scheduling Logic – Using Recurrence, Delay, and Refresh blocks in Power Automate

🔄 Workflow Automation
1. Automated Email Watcher
   * Outlook automation detects new incoming survey files (\~25 daily)
   * Files are downloaded automatically (Power Automate flow)

2. Data Aggregation and Cleaning
   * All files are merged, cleaned, and prepped using Python scripts
   * Final dataset is stored in a location connected to Power BI

3. Power BI Refresh Automation
   * Triggered via Power Automate (with recurrence + delay logic)
   * Dataset is refreshed based on schedule or after new data load

4. Dashboard is auto-updated** and accessible to stakeholders without any manual refresh

📈 Key Insights From Dashboard

Income & Spending Trends:
  * Avg. Annual Income: ₹171.25K
  * Avg. Monthly Balance: ₹394.70
  * Avg. Credit Utilization Ratio: 32.17%
  * Avg. Delay in Payment: 21.02 days

Age-Based Analysis:
  * Correlation between age and credit limit changes
  * Distribution of credit types across age groups (Teen, Young Adult, Old Adult, etc.)

Customer Insights Using DAX:
  * DAX-based LTV formula to score customer financial health
  * Offers dynamically generated based on LTV:
    * > 80K → 30% off + home loan at 4%
    * 60K–80K → 15% off + ₹10,000 gift
    * 50K–60K → Any loan at 5% interest

Potential Customers Detection:
  * Based on average credit inquiries > 7.5
  * Segmented by age groups with high LTV

Credit Product Ownership:
  * Avg. number of loans and credit cards per age group
  * Used to identify product interest trends
    
Loan Product Popularity:
  * Most popular: Credit-Builder, Personal, Payday Loans
  * Useful for targeting offers and new services

💡 Business Value
* Saves Time: No manual downloading, combining, or refreshing
* Reduces Cost: Removed the need for additional hires (\~\$12,000/month saved)
* Improves Accuracy: Error-free automation with monitored refresh logs
* Real-Time Insight: Clients (e.g., US Government) get reports on the same day
* Better Targeting: LTV and age-segmentation allow personalized offers
* Scalable: Can be adapted for other regions, teams, or credit products
