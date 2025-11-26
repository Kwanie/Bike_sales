# Bike Sales Analysis


### Project overview
This project transforms raw customer data `bike_buyers` into an **interactive analytical dashboard** designed to identify the most valuable and high-converting customer segments. The primary goal was to calculate the precise **Purchase Rate (Conversion Rate)** across key demographics to drive focused marketing and sales strategies.

### Data Sources
The primary dataset used for this analysis is the "bike_buyers.xlsx" file which includes financial indicators `(Income, Home Owner)`, lifestyle factors `(Commute Distance, Cars)`, and demographic identifiers `(Age, Gender, Region)` and `Purchased Bike` for calculating customer conversion rates.

### Tools
- Excel

### Data Cleaning
To ensure the data was ready for insightful analysis and visualization, the following cleaning and transformation steps were performed:
- **Data Inspection**: Initial review of all columns to check data types, identify missing values, and locate inconsistencies.
- **Duplicate Removal**: Identified and removed duplicate customer entries `(ID)` to ensure accurate calculation of customer counts and conversion rates.
- **Text Field Standardization**: Normalized categorical columns for better readability and filtering:
   - **Marital Status**: Converted single-letter codes `(M, S)` to full text `(Married, Single)`.
   - **Gender**: Converted single-letter codes `(F, M)` to full text `(Female, Male)`.
- **Age Bracketing**: Created a new derived column to group continuous `Age` values into discrete, analyst-friendly brackets using **IFS** (e.g., 25-39, 40-59).
- **Income Grouping**: Created a second new derived column using **IFS** to bin continuous `Income` figures into manageable categories (e.g., Low(<40k), Medium(40k-79k)).

### Exploratory Data Analysis
EDA involved exploring the data to answer key questions such as:
- Which **Age Group** has the highest propensity to purchase a bike?
- How does **Income level** correlate with conversion rate?
- Which **Region and Commute Distance** combination represents the most lucrative niche market?

### Data Analysis
This analysis heavily utilized advanced features in Excel 2016 and Excel Web to create a professional report.
- **Guided Project Fundamentals**: The foundation of this project included skills learned from guided material:
   - **Data Binning**: Applied IFS to transform continuous numerical data (Income, Age) into discrete, actionable categorical groups.
   - **Interactive Controls**: Mastered the use of Slicers for filtering data across factors like Gender, Marital Status, and Number of Cars.
 
- **Independent Analytical Additions (Self-Implemented)**: The following elements were designed to elevate the project beyond a basic exercise:
  - **Metric Calculation**: Transitioned from basic raw counts to the critical **Purchase Rate (% of Row Total)** metric across all visualizations.
  - **Dynamic KPIs**: Designed a resilient system using the `GETPIVOTDATA` function to create a dynamic Sample Size Card that updates with every filter selection, providing context and validating insights.
  - **Advanced Visualization**: Developed a **Deeper Insights Chart** (cross-tabulation of Region and Commute Distance) to reveal high-value niche segments, such as the **Pacific/0-1** Mile Commute group.
  - **Actionable Insights Section**: Added a TextBox with **"Key Findings & Recommendations"** to the dashboard to clearly summarize the business value and actionable conclusions derived from the data.

### Results
Through the analysis i was able to find out that:

- The highest propensity to purchase a bike is observed in the 25-39 age group, with a conversion rate of 56%. This segment represents the primary marketing target.
- While North America has the largest volume of customers, the Pacific region offers the best ROI, with a conversion rate of 58.85% across all demographics.
- The most concentrated buyer segment in the entire dataset is found in the Pacific region among customers with the shortest commute (0-1 Miles). This segment converts at an extremely high rate of 73%.

### Recommendations


    
    
