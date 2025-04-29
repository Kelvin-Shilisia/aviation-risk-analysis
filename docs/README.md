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
<img width="646" alt="image" src="https://github.com/user-attachments/assets/52229274-a56b-4e65-9c8f-851438430df8" />

This graph shows the trend of the accidents over time. 

A treemap that shows Number of Accidents per Broad Phase of Flight 
![image](https://github.com/user-attachments/assets/70fea892-b765-4bde-ae37-23913e182a5e)

Insights: 
Most accidents occur during the Cruise and Maneuvering phases
Cruise phase (the period when the aircraft is flying level between climb and descent) has the highest number of accidents.

Maneuvering phase (low altitude, turning, or adjusting flight path) also shows a high accident rate.

Business Meaning: It’s important to focus on in-flight training and risk management even after takeoff and before descent — accidents don't just happen during takeoff or landing.

Recommendation: Invest in advanced pilot simulator training focusing on Maneuvering
![image](https://github.com/user-attachments/assets/1f5ae50d-e606-46e9-b361-7815014ca7f1)

A combined bargraph that shows Aircraft Damage per Category 

![image](https://github.com/user-attachments/assets/33e97748-e9d8-452f-9218-e4b461bce6d3)

Insights: 
Substantial damage is by far the most common outcome
Most incidents lead to substantial damage rather than minor damage or total destruction.


Substantial damage often requires major repairs but the aircraft may still be recoverable.


Business Meaning: Insurance, repair, and maintenance costs will be significant — but total aircraft loss is less common than expected.


Recommendation: Invest in Comprehensive Maintenance Programs
![image](https://github.com/user-attachments/assets/5fab60d9-2546-44e4-8057-b22d7128f8a4)

A line Graph showing Uninjured Passengers over the last 15 years

![image](https://github.com/user-attachments/assets/1c972d3a-4209-4da0-b1e9-96d20b98bdc1)

Insights: 
Decline in the number of uninjured
A decline in the number of uninjured passengers suggests that more people are sustaining injuries during incidents.

This could be due to factors such as:
Poor cabin safety procedures
Inadequate use of safety belts or cabin equipment failures

Recommendations:
Enhance In-Cabin Safety Procedures
Invest in Crew Safety Training
![image](https://github.com/user-attachments/assets/2ce296f6-b456-494d-bab1-de38c74b0e5d)

Recommendations: 

Purchase aircraft models with low fatality history.

Implement maintenance and pilot training programs.

Monitor ongoing incident trends post-purchase.

Focus mid-flight safety procedures.

Invest in takeoff/landing training.

Maintain but don't overly prioritize these phases.
![image](https://github.com/user-attachments/assets/18bf9ea0-0a0d-437e-875f-6a0fb2cd0416)

Exporting processed data for data visualization on Tableau. 
- Tableau dashboard for business presentation
  An Interactive dashboard
  <img width="636" alt="image" src="https://github.com/user-attachments/assets/86db9517-dc60-43c6-a642-51c9b3e0bd4f" />

- (https://public.tableau.com/app/profile/kelvin.shilisia/viz/AircraftRiskAnalysis_17458565253400/Dashboard1?publish=yes)

How to Use This Repo
1. Clone the repo
2. Explore the `notebooks/` or Tableau dashboard
3. Review visual insights and presentation materials

Author
Kelvin Shilisia  
kelvinshilisia@gmail.com  
[LinkedIn Profile](https://www.linkedin.com/in/your-profile)





