# Bike Sales Analysis


## Table Of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)



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
This section summarizes the actionable insights derived from the interactive dashboard and PivotTable analysis

- The **highest propensity** to purchase a bike is observed in the **25-39 age group**, with a conversion rate of **56%**. This segment represents the primary marketing target.
- While North America has the largest volume of customers, the **Pacific Region** offers the **best ROI**, with a conversion rate of **58.85%** across all demographics.
- The **most concentrated** buyer segment in the entire dataset is found in the **Pacific Region** among customers with the **shortest commute (0-1 Miles)**. This segment converts at an extremely high rate of **73%**.
- In contrast, customers in the **Europe Region** with a **long commute (10+ Miles)** show the **lowest propensity** to purchase, with a conversion rate plummeting to **16.67%**.
  


### Recommendations
The findings identify not just who to target, but where and how to allocate resources for the **maximum return on investment (ROI)**

- **Targeting Focus:** Marketing spend should be heavily weighted towards the **25-39 age bracket** and the **Pacific Region**, specifically through social media platforms popular with that demographic.
- **Geographic Strategy:** Local store presence and visibility campaigns are critical in high-density areas of the Pacific, where bikes are likely used for **local, short-distance errands**.

  

### Limitations

- **Software Version Conflict**: The project required frequent transitions between **Excel Web** and **Excel 2016 (Desktop)**. This was necessary because specific functionalities were unavailable or unstable in one version, necessitating workarounds in the other.
-  **Visualization Workaround (Hiding Data)**: To create the clean, focused visualization required to display only the **Purchase Rate (Yes)** columns in the PivotChart, a creative workaround was necessary. The underlying **'No'** column in the PivotTable had to be manually colored white.
-  **Aesthetic Compromise**: While this workaround successfully filtered the focus to the desired metric, it caused minor gridline misalignment in the resulting PivotTable display.
-  **Result Integrity**: Crucially, despite these visual and procedural compromises, the **data integrity and mathematical accuracy of all charts remained correct and fully understandable**, successfully delivering the intended analytical insights.
  


### References
[Alex The Analyst](https://youtu.be/opJgMj1IUrc?si=lAo1_ek0q6w1I51O)

[Documentation](https://youtu.be/0N9xekdKCwk?si=pYb1LZVcvS0ud96I)

    
    
