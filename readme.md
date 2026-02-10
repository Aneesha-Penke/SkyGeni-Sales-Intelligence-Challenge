**Sales Intelligence Challenge**
Thsi project analyses CRM sales data to understand why win rate changed and identify the key drivers of wins and loses and also build a lightweight decision engine to flag high risk deals.

Dataset-
sales lifecycle(dates and stage)
Deal outcome, amount
Metadata- industry, region product etc

** APPROACH **
1. Data prepartion
 Checked for missing and duplicate values
 Converted date columns into proer datetime format
 Converted a binary win_flag from outcome
 Created time based features(Month and Quarter)

2. EDA
 Win rate is analyzed across all features like time, dales reps, Industry, region, product,lead source, deal stage, deal amount, sales cycle days.
 The insights gathered from EDA are written in the python notebook.

** The win rate decline is not systemic

3. Sales Cycle Insight
 Fast deals - higher win rate
 Very long deals - higher win rate
 Mid cycle deals - lower win rate.

4. Custom metrics
 Lead Quality ratio- measures win rate to lead source, and gives underperforming lead sources
 Stage Stall score - Maps stage level performance. Used to detect deals in unproductive stages.

5. Decision Engine(Option  B--Win Rate Driver Analysis)
  A logistic regression model is used to identify which factors import or hurt the win probability
  - Ranked list of positive and negative win rate drivers

PART-4 -Mini System design and PART-5 -Reflection are written in the python notebook

** HOW TO RUN THE PROJECT **
 pip install pandas numpy matplotlib seaborn scikit-learn
 Place "skygeni_sales_data.csv" in the directory
 Open and run code.ipynb (In production this would be modularized into python scripts)


** KEY DECISIONS **
 Focused on EDA- To amke sure insights are derived from data and not model assumptions.
 Sales cycle bevaiour showed most actionable signal for win rate decline.


