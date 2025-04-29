Aviation Risk Analysis

                        Project Overview
This project analyzes aviation incident data to help identify the safest aircraft models for commercial or private use. It aims to support the company's expansion into the aviation sector by minimizing operational risk.

                    Data Preparation and Analysis with Pandas
This section explains how I loaded, cleaned, explored, and presented aviation incident data using the Python pandas library (tool for working with tabular data.)
Loading the two CSV files into pandas DataFrames.
I worked with two CSV files:

processed_aviation_data.csv: A detailed dataset of aviation incidents, including aircraft model, date, location, injury severity, and damage level.

aircraft_accident_counts.csv: A summarized dataset showing the number of accidents by aircraft model.

I used pandas to load these into DataFrames (tables) for analysis:

The error message indicates that the file 'AviationData.csv' cannot be decoded using UTF-8. I will try to read the file with a different encoding, such as 'latin-1', which is often used for Western European text.
The Objectives
- Identify aircraft models with the lowest incident and fatality rates.
- Explore trends in damage types and injury severity.
- Support data-driven decisions for aircraft purchasing.
  
                     Data Cleaning
Before analysis, we cleaned the data to ensure accuracy. This included:

Removing duplicates: Prevent counting the same incident twice.

Standardizing column names: e.g., converting all names to lowercase and removing spaces for consistency.

Converting dates: Changed event dates to datetime format and extracted the year.

Fixing inconsistent categories: Ensured fields like Injury Severity and Aircraft Damage were standardized (e.g., "Destroyed" vs "destroyed").


                  Exploratory Data Analysis (EDA)

Exploring the loaded datasets to understand their structure, data types, and basic statistics.

EDA helps us understand the structure and patterns in the data. With pandas, we performed:

Descriptive statistics (mean, count, etc.)

Distribution checks (e.g., number of incidents per year)

Categorical summaries (e.g., how many aircraft were "Destroyed" vs "Substantial Damage")

Examining their shapes, data types, descriptive statistics, missing values, and unique values for relevant columns, as per the instructions.

                 Grouping Data for Insights
We grouped the data to generate useful summaries, such as:

Total incidents by aircraft model

Fatal injuries by year

Damage level by aircraft category

                Visualizations

- Visualizations: bar charts, treemaps, pie charts, maps







- Tableau dashboard for business presentation (https://public.tableau.com/app/profile/kelvin.shilisia/viz/AircraftRiskAnalysis_17458565253400/Dashboard1?publish=yes)

## 🔍 Key Findings
- Cruise and maneuvering phases have the highest accident rates.
- Substantial damage is the most common outcome.
- Certain models like Cessna 172 and Diamond DA40 have lower fatal injury records.

## ✅ Recommendations
- Prioritize newer aircraft models with better safety history.
- Train crew for in-flight risk phases, not just takeoff/landing.
- Invest in maintenance and emergency response planning.

## 🧭 How to Use This Repo
1. Clone the repo
2. Explore the `notebooks/` or Tableau dashboard
3. Review visual insights and presentation materials

## 👤 Author
Kelvin Shilisia  
📧 kelvinshilisia@gmail.com  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/your-profile)

## ❓ Questions or Contributions?
Open an issue or submit a pull request!



