# NYPD-Arrest-Analysis

![image](https://github.com/CarlosGG18/NYPD-Arrest-Analysis/assets/117116368/d7511652-6a8d-4624-bd39-891718e09ea7)

# Overview 

New York City, known for its vibrant urban life, also faces unique challenges in maintaining law and order. This project aims to analyze the NYPD arrest dataset from 2022 to March 2024 to uncover patterns in arrest data and identify crime hotspots across the city. By examining this data, I hope to gain insights into the spatial and temporal distribution of crime, understand demographic trends, and build predictive models to help allocate law enforcement resources more effectively.

# Dataset

The dataset I am utilizing is the [NYPD Arrest Data](https://data.cityofnewyork.us/Public-Safety/NYPD-Arrest-Data-Year-to-Date-/uip8-fykc/about_data)
, which contains information on arrests made by the NYPD, including details such as arrest date, offense description, borough, law category, demographic information of the arrestee, and longitude & latitude of the arrest. I incorportaed both the 2024 year-to-date arrest data as well as the historical arrest dataset but only used arrests made after 2022 due to memory limitation, which can be found within the cleaning.ipynb notebook.

# Objective

Identify Crime Hotspots: Determine geographic areas with high arrest rates and analyze the types of crimes prevalent in these areas.
Examine Demographic Patterns: Investigate how arrest rates vary across different demographic groups and identify any significant disparities.
Analyze Temporal Trends: Explore how crime rates fluctuate over time and identify any seasonal or temporal patterns.
Predict Crime Types: Develop machine learning models to predict the type of crime based on available data.

# Problem Statement

Analyzing arrest data is crucial for understanding crime dynamics and the criminal justice system's response in a large urban setting. By identifying patterns in offense types, demographics, and geographical locations, law enforcement can better allocate resources, develop targeted intervention strategies, and evaluate the effectiveness of past policies. This project aims to answer the following key questions:

What are the most common types of offenses in NYC?
How do arrest rates and types vary across different boroughs?
What are the temporal trends in arrest data?
Are there noticeable differences in arrest rates based on demographic factors like race and gender?

# Exploritory Data Analysis (EDA)

1) **Crime Count**

The analysis shows that the majority of arrests in NYC are for misdemeanors (about 55%) and felonies (about 45%), with a minimal percentage for traffic violations and other minor offenses. The consistent distribution, even in the 2024 year-to-date data, highlights a sustained focus on more serious crimes. The stable proportion of misdemeanors and felonies suggests that law enforcement efforts are primarily concentrated on these categories, potentially reflecting ongoing priorities in policing and public safety strategies. Minor categories such as traffic violations and unclassified offenses, each constituting less than 1% of arrests, indicate that these are relatively rare and may not require as much focus in broader law enforcement policies.

| Crime Count 2022-2023                               | Crime Count 2024 YTD                             |
|-----------------------------------------------------|--------------------------------------------------|
![Crime count 2022:2023](https://github.com/user-attachments/assets/b0d31ea0-3600-493a-a858-eabc08f684d2)|![crime count ytd](https://github.com/user-attachments/assets/f21368be-c973-4fe2-b4cf-b338f923f2a9)




2) **Age Group**

The analysis of arrests by age group reveals that the 25-44 age group has the highest arrest rates in both 2022-2023 and 2024 year-to-date (up to March). This group consistently makes up over 57% of total arrests, indicating that young to middle-aged adults are more likely to be involved in activities leading to arrests. The second-highest arrest rates are observed in the 45-64 age group, followed by the 18-24 age group.

| 2022-2023 Arrests by Age                            | 2024 YTD Arrests by Age                          |
|-----------------------------------------------------|--------------------------------------------------|
![age arrests 2022:2023](https://github.com/user-attachments/assets/d11b9184-28b3-41fa-bb18-356b5f1fc80c) |![age arrests ytd](https://github.com/user-attachments/assets/2fe8ad19-dd78-4c27-9041-a5ab8c9a556f)

These observations suggest that law enforcement activities are significantly concentrated on young to middle-aged adults, which may reflect the demographic most involved in or exposed to circumstances leading to criminal behavior. This consistent pattern over the years suggests a stable trend in the demographic composition of arrests in New York City.




3) **Race**

Distribution of Arrests by Race (2022-2023): The majority of arrests are concentrated among Black and White Hispanic individuals, who together account for over 74% of all arrests. This significant disparity suggests that law enforcement efforts are disproportionately affecting these racial groups. The rest of the racial groups have considerably lower arrest rates.
![image](https://github.com/user-attachments/assets/54fa4cb9-af65-4a8b-9eb4-9cdfa15974f4)


Comparison of Felony and Misdemeanor Arrests by Race (2022-2023): Both felony and misdemeanor arrests are most prevalent among Black and Hispanic individuals. Notably, Black individuals have a higher rate of felony arrests compared to other groups, indicating potential racial biases in the types of crimes leading to arrests.

![image](https://github.com/user-attachments/assets/d3ddcb58-7af8-4342-ac17-55619f9f4e50)


Year-to-Date Comparison for 2024: The racial distribution of arrests in 2024 (up to March) follows a similar pattern to the previous years, with Black and White Hispanic individuals being the most frequently arrested. This continuity suggests that the disparities in arrest rates among different racial groups indicate systemic biases or socioeconomic factors that influence crime rates and law enforcement practices. The concentration of felony and misdemeanor arrests among specific racial groups highlights the need for targeted community support and reform in policing practices to address these inequities.

![image](https://github.com/user-attachments/assets/628fcea0-1983-4571-a765-2b1e9eb07a2b)

