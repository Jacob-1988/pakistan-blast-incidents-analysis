## Pakistan Blast Incidents Analysis - Maplotlib Project

### Statement of Problem
Pakistan has faced repeated blast incidents over the years, causing significant loss of life, injuries, and destruction of property. However, raw incident records are often inconsistent, incomplete, and difficult to analyze in their original form. Without proper data cleaning and analysis, it is challenging to:

Identify patterns and trends in blast occurrences across provinces and cities.

Understand the relationship between casualties and contextual factors such as temperature, day type, or location sensitivity.

Assess the targets and sectarian dimensions of such attacks.

Provide data-driven insights for policy makers, researchers, and security agencies.

This project addresses the problem by cleaning, structuring, and analyzing the dataset to uncover meaningful insights that can guide preventive and response strategies.


### Table of Contents:
- Project overview

- Dataset Description

- Data cleaning process

- Exploratory Data Analysi (EDA)

- Key insights

- Tools and Technologies
- Next steps
- Conclusion

### Project Overview:
This project explores and analyzes blast incidents in Pakistan using a dataset of 492 records with 26 features. The dataset contains both categorical and numerical information, including details such as location, casualties, targeted sects, explosive weights, and environmental factors like temperature.

The goal of this analysis is to clean, explore, and extract meaningful insights about blast patterns across regions and time.





 ### Dataset Description:

The dataset contains 26 columns. Some of the key features include:

#### General Information:

- Date, City, Province, Time

- Latitude, Longitude

- Blast Details:

- Target Type, Targeted Sect if any

- Killed Min/Max, Injured Min/Max

- Explosive Weight (max), No. of Suicide Blasts

#### Contextual Information:

- Blast Day Type, Holiday Type

- Location Sensitivity, Open/Closed Space

- Hospital Names, Temperature (C/F)

 #### Data Shape: 
 - 492 rows × 26 columns

#### Data Cleaning Process:
Several steps were taken to ensure the dataset was ready for analysis:

- Handling Missing Values

Holiday Type, Explosive Weight, Killed Min had significant missing values.


- Data Type Conversion

Columns such as Longitude, Explosive Weight (max), and Injured Max were stored as object and converted to numerical types where possible.

- Duplicates & Inconsistencies

Checked for formatting issues in categorical columns such as Blast Day Type and Targeted Sect if any.

Standardized values (e.g., converting “low” → “Low”).


###  Exploratory Data Analysis(EDA)
Some analysis directions explored include:

#### Blast Frequency Analysis


- Distribution of blasts by city, province, and year.

- Identification of hotspot regions.

#### Casualty Analysis

- Minimum vs Maximum killed and injured values.

- Relation between temperature and casualty numbers.

#### Target Analysis

- Distribution of different Target Types (e.g., civilians, government, military).

- Insights on Targeted Sect patterns (where data was available).

#### Spatial & Sensitivity Analysis

- Breakdown of blasts by Location Sensitivity and Open/Closed Space categories.


###  Key insights:
From the cleaning and exploratory analysis of the dataset, the following insights were observed:

1. Geographical Hotspots

- The majority of blast incidents were concentrated in a few provinces, with certain cities emerging as recurring hotspots.

2. Casualties

- There is a wide variation between Killed Min/Max and Injured Min/Max, indicating possible inconsistencies in initial reporting.

- Blasts in closed spaces tended to cause higher casualties compared to those in open spaces.

3. Temporal Patterns

- Blast frequency varied across different years and months, with spikes linked to specific events or influencing factors.

- Some incidents were associated with holidays or religious days, highlighting potential patterns in timing.

4. Target Analysis

- A variety of target types were affected, including civilians, government institutions, and security forces.

- Where available, sectarian targeting data indicated disproportionate attacks on specific groups.

5. Environmental Factors

- Temperature was recorded for most incidents, allowing for exploration of its relationship with casualty counts.

- Preliminary analysis suggests no strong correlation, but it opens avenues for deeper statistical testing.

6. Data Quality Observations

- Several fields such as Holiday Type, Explosive Weight, and Targeted Sect if any had large amounts of missing data, which could limit the depth of analysis.

- Some numerical columns (e.g., Longitude, Explosive Weight) were originally stored as objects, requiring data type correction.

### Tools and Technology:
The following tools and technologies were used for data cleaning, analysis, and visualization:

- Python – Main programming language for analysis

- pandas – Data manipulation and cleaning

- numpy – Numerical computations

- matplotlib – Data visualization (charts & plots)

- Jupyter Notebook – Interactive coding and documentation environment

###   Next steps:
While this project has provided valuable insights through data cleaning and exploratory analysis, further work can enhance the depth and applicability of findings:

1. Advanced Statistical Analysis:

- Apply correlation and regression techniques to quantify relationships (e.g., temperature vs. casualties, location sensitivity vs. fatalities).

2. Predictive Modeling:

- Develop machine learning models to predict casualty severity or likelihood of high-impact blasts based on contextual factors.

3. Geospatial Analysis

- Use mapping tools (e.g., folium, geopandas) to visualize blast hotspots across Pakistan.

4. Dashboard Development

- Build an interactive dashboard in Power BI, Tableau, or Plotly Dash to allow stakeholders to explore the data dynamically.

5. Data Enrichment

- Integrate external datasets (e.g., socio-economic indicators, conflict reports, weather data) for richer analysis.

6. Improved Data Quality

- Address missing values in key fields such as Explosive Weight, Holiday Type, and Targeted Sect to strengthen insights.

###  Conclusion:
This project provides a comprehensive overview of blast incidents in Pakistan by cleaning, analyzing, and visualizing the dataset. It highlights key insights about frequency, casualties, targets, and contextual factors surrounding such events.

The findings can be a useful resource for security agencies, policy makers, and researchers in understanding patterns and mitigating future risks.

### Screenshot of top 10 cities by frequency of blast
<img width="459" height="306" alt="Image" src="https://github.com/user-attachments/assets/06680738-daad-4e11-b8d4-1fe236b57dc0" />

### Screenshot of Total killed vs Injured by Targeted Sect
<img width="462" height="271" alt="Image" src="https://github.com/user-attachments/assets/4c5b3afd-7aa2-45b4-baa3-dcff57297f07" />








