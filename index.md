---
title: "Juan Zumaran MS DAV Portfolio"
layout: default
---


# Project 1: Visualizing Water Availability in Uruguayan Soil: 
## This project's core accomplishment was the large-scale geospatial data wrangling required to synthesize Uruguay's fragmented environmental landscape into a unified analytical model for the first time. Over three months, I acquired, merged, and processed five massive public datasets spanning water availability, elevation, forest cover, waterways, and historical forest fires. The most significant technical hurdle was merging 495 individual files totaling over 2 GB of raw data to create a single, seamless national elevation layer, which served as the foundational canvas. This was integrated with the other nationwide datasets using a suite of advanced GIS statistical and spatial analysis tools to model the complex interactions between variables like topography, water accumulation, and land cover.

<iframe src="https://storymaps.arcgis.com/stories/3b727433cb174b7dbe92de91502b01fb" width="100%" height="500px" frameborder="0" allowfullscreen allow="geolocation"></iframe>


# Project 2: Mapping and Analyzing Education Atainment and Race in Montevideo, Uruguay. Developed using ArcGIS Pro
## This project investigates the spatial relationship between race, education attainment, and unemployment in Montevideo, Uruguay, testing whether geographic context improves predictive power over traditional linear models. As the sole analyst, I designed a comparative modeling workflow using ArcGIS, training both an Ordinary Least Squares (OLS) regression and a Multiscale Geographically Weighted Regression (MGWR) to predict unemployment rates across census tracts while incorporating spatial autocorrelation and racial demographic data. The final deliverable demonstrates my ability to work across the full lifecycle of a spatial data science project, from data acquisition and exploratory spatial analysis to advanced geostatistical modeling and interpretation of coefficients that became significant only when geography was accounted for. The MGWR model explained 90% of the variance in unemployment rates, a substantial improvement over OLS, revealing that the effects of education and race on unemployment vary significantly across Montevideo—with the highly educated, predominantly White neighborhoods in the south showing markedly different patterns than the less White, lower-education areas at the city's edges.

<iframe src="https://storymaps.arcgis.com/stories/9b7d156e4ba644b5a69c45c486450c85" width="100%" height="500px" frameborder="0" allowfullscreen allow="geolocation"></iframe>


# Project 3: Mapping and Analyzing Cannabis Possesion Arrests and Race in NYC using NYPD and Census Data. Developed using ArcGIS Pro.
## This Story Map project investigates the spatial relationship between race and cannabis possession arrests in New York City from 2020 to 2023, testing the hypothesis that arrests are spatially correlated with the ethnic composition of neighborhoods across Brooklyn, Queens, and Manhattan. As the sole analyst, I designed a comprehensive geoprocessing workflow using ArcGIS, including clipping, spatial joins, projection, tessellation, and Getis-Ord Gi hotspot analysis, to quantify patterns and transform raw arrest data into an interactive web map that visualizes statistically significant clusters alongside census tract ethnicity data. The final deliverable demonstrates my ability to work across the full lifecycle of a spatial data project, from data acquisition and geoprocessing to the creation of a narrative-driven Story Map that makes complex spatial patterns accessible to diverse audiences. The analysis revealed that hotspots with 99% confidence, including Harlem, Bedford-Stuyvesant, and Jamaica, align predominantly with Black-majority neighborhoods, while cold spots correspond to predominantly White or Asian areas, illustrating how spatial analysis can reveal patterns that merit deeper examination within broader discussions of equity and policing.

<iframe src="https://storymaps.arcgis.com/stories/643d2319029a4339b296123565736cc3" width="100%" height="500px" frameborder="0" allowfullscreen allow="geolocation"></iframe>


# Article 1: NYC Shooting Incidents Analysis
## Github Repository: https://github.com/juanito040102/NYC_Shooting_Incidents

Github Pages (Website) (Contains the Visuals): https://juanito040102.github.io/

NYC_Shooting_Incidents/

Project Topic

This project investigates the spatial and temporal relationships between shooting incidents in

New York City, The core objective is not to claim any conclusion on the cause or nature of these

incidents, but to visualize and analyze patterns that may reveal longstanding systemic

inequalities across NYC boroughs. The final deliverable will be a series of interactive plotly

visuals accompanied by a narrative that tell a data-driven story about the urban landscape of

violence and poverty. This project is to be expressed digitally, not in print, and in an interactive

way, not static. Ideally, this project could live in a repository in Github and later be developed

into a static website in which the visualizations maintain their ability to be interactive.

Dataset: NYPD Shooting Incidents

This dataset is obtained through NYC Open Data, and there are two complimentary pieces of

information; the Historic dataset that compiles the shooting incidents from 2006 until the end of

2024, and the active dataset that gathers the shooting incidents of this current year, 2025, up until

the day of accessing the data.

https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8/about_data

https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Year-To-Date-/5ucz-vwe8/about_data

The Historic dataset and the YTD Dataset both have the same columns, but different amounts of

rows. The historic dataset has 29,744 incidents over the course of several years and the YTD

dataset has 769 incidents over the course of almost a year. This means that on average, the

historic dataset expects around 1.6 K records every year. When the datasets are combined, there

are 30,513 incidents over the course of 18 years and 9 months.

They both share the same 21 columns; Incident_Key, Date_Occurrence, Time_Occurrence,

Borough, Location_Occurrence, Precinct, Jurisdiction_Code, Location_Classification,

Location_Description, Murder_Flag, Perp_Age_Group, Perp_Sex, Perp_Race,

Victim_Age_Group, Victim_Sex, Victim_Race, X_Coordinate, Y_Coordinate, Latitude,

Longitude and Georeference_column.

These columns can be grouped into 3 categories; about the incident, about the people involved,

and the geography or location of the incident.

Introduction to Visualizations

This analysis is regarding public shootings in New York City from 2006 and 2025. As a foreigner

who now lives here, the culture and opinions surrounding the second amendment or the right that

Americans have to bare arms shocked me. There is freedom of action but not of consequence.Society in here sometimes seems to assume that because they require the right to bare arms then

some other individual will pass away over a firearm. The fact that this dataset has more than 30K

records is astonishing, and of course there is a lot to be said and done about this subject, and this

analysis could contribute more significantly to the current discourse, however my interest lies in

the seasonality of these incidents. Why is there a constant number of these events occurring? And

when do they occur more often? Because of this train of thought the analysis goes through

visuals regarding hours, days, months, years, and even all at the same time. Some patterns are

visible to anyone, even if there is no python knowledge behind.

How to interact and use these visuals: A tutorial on how to be a user of plotly.

1. Hovering over the data is useful. If it is a line chart, you can follow the trend with the cursor

and get insights on the values and how they were changing over time. If it were a bar chart or

a scatter plot, hovering over the figures will make a pop-up come up and show the user the

data point they were curious about.

2. Clicking on/off data points can be messy. As a user, it is natural to want to click and press

the cursor, but once the point is selected, all of the other data becomes transparent and not the

focus of the visual. Turning off a group inside a bigger variable can be insightful, and turning

it back on is just as easy, so playing with this function is pretty safe.

3. Zooming In/Out is different than the intuitive scroll. To zoom in on a visual, the user needs

to make two clicks, one as a starter point, and then drag the cursor around to generate a

window that once the user lets go, it will expand into screen and only show what the cursor

selected. To zoom back out there are two choices, the zoom buttons on the top right that can

help to go in and out, or the House icon, which is also conveniently on the top right corner,

and will take the user straight back to the original position of the visualization.

4. Nothing is going to break over the user interacting. The user may click and click but the code

for the visual remains intact, and if they just press the house button on the top right everything

will go back to normal.

Methods, Tools and Processes

1) Microsoft Excel: Data Acquisition & Data Cleaning

Download the two datasets and remove the unnecessary row at the top and the additional sheets

that make python be able to read the dataset. Also there is an initial glimpse at the data that is

made in Excel because of how easy Pivot Tables can be to make.

2) Python Notebook

Python notebooks are used to analyze data and create visuals using the libraries pandas, numpy,

matplotlib and plotly (plotly.express).

For this analysis, the main tool used was a python notebook to clean the data types, combine the

two datasets, but mostly to generate insightful visuals. The main objective is to analyze the datathrough a temporal interest / lens. This means to study if the data has evident seasonality, or

frequencies that vary according to some sort of date/time information piece. On the other hand,

one or two visuals regarding the victim or perpetrator information could be of use / relevant to

complement the rest of the analysis. Additionally, this notebook has the task of creating an

interactive map visual in which the user can observe the incidents of one year, and still be able to

switch to visualize another year. Moreover, the user has to be able to hover over points and get a

pop-up of some of the data, and be able to zoom in and out of the map to go into detail or simply

see the big picture.

3) Github & Github Pages

Once the data is clean, the visuals are created, those plotly graphics can be transformed into

HTML code and be uploaded to a Github repository, accompanied by the notebook, a read me

file and other relevant documents to generate a static website that can host these visualizations

and be more accessible to a different audience that is not familiar with python notebooks.

Expected Design Products

Tools planned to use: Python Notebook (using pandas, numpy and plotly) into a github

repo with a read.me file.

Data Cleaning:

Column Types:

Int/Float (Numeric): id, precinct and jurisdiction code.

Object: date, time, boro, location occurrence, location classification, location

description, age / sex / race groups (for both vic & perp), latitude and longitude.

Boolean: Murder_flag

It is evident that date and time of occurrence should not be object type of data, and require to be

changed to a date time column on their own to be able to operate with the data. Using the

function ‘to_datetime’ from the pandas library it is possible to create a new column that uses the

‘date’ and ‘time’ strings to generate a new column ‘datetime’.

Categorical Columns:

The categorical columns are columns that have object type of data but it is relevant to analyze

them too. These columns are related to the incident; Borough, Location Occurrence, Precinct,

Location Classification and Location Description. There are other categorical columns in thedataset like: Perp Age Group, Perp Sex, Perp Race, Victim Age Group, Victim Sex, and Victim

Race.

Using the function ‘value_counts’ it is possible to obtained an ordered list of the different values

the column is possible to have and what their frequency in the dataset is. It is relevant to know

that the Combined Data frame has 30,513 incidents to spot which columns have any missing

values. Here are the number of incidents with their respective values, ordered by amount of

incidents.

• Borough: BK. (12K), BX. (9K), Q. (4.5K), M. (4K) and S.I. (0.8K). Missing Values = 0

• Precinct: not relevant to this iteration of this analysis. Possible recommendation or next step.

• Loc_Occur:Outside (4,158), Inside (759), Missing Values (25,596). Not Useful.

• Loc_Class:Street (3K), House (0.8K), Others (1K), Missing Values (25.6K). Not Useful.

• Loc_Desc: Multi Dwelling (5.3K), Others (6.4K), Missing Values (18.7K).Not Useful.

• Perp_Age: 18-24 (6.8K), 25-44 (6.6K), under 18 (1.9K), Missing Values (14.4K). Not Useful.

• Perp_Sex: Male (17.3K), Female (0.5K), Missing Values (12.7K). Not Useful.

• Perp_Race: Black (12.7K), Hispanic (4.3K), Missing Values (13.0K). Not Useful.

• Vic_Age: 25-44 (14.0K), 18-24 (10.9K), under 18 (3.2K), other (), Missing Values (70).

• Vic_Sex: Male (27.5K), Female (3.0K), Intersex (1), Missing Values (12)

• Vic_Race: Black (21.5K), White Hispanic (4.6K), Black Hispanic (3.0K), White (0.8K),

Asian/Pacific Islander (0.5K), Native (0.01K), Missing Values (73)

3) Missing Values: there are non variables pertinent to this analysis that have a very high number

of missing values. The variable that do have a lot of missing values are not relevant to this

analysis in this iteration.

UX Research

Observations, Tasks, Interviews. Two People

Who, What, How?

• Who: Primary: One LIS Student with little python knowledge. Secondary: Another person that

does not know the tools at all. They need to be able to follow the story.

• What:

5. Comprehension: are users able to understand the visuals and the map?

6. Usability: can users hover for details, and navigate the visualization without instructions?

7. Insight & Value: What is the user’s main takeaway?

8. Missing Information: What other analysis did the user suggest is complimentary to this one?

• How: Two interviews last 30 minutes each. One simple task for each visualization.

1. Observe: Hesitations? Pain Points?

2. Feedback Survey: 5 point scale for understanding. Any difficulties?LIS Student (Interviewee 1)

Narrative: they understand narrative and story. They think the topic is controversial.

Map: they understand the map but had questions about the data.

Usability Visuals: at first they did not understand the zoom function. With a tutorial from the

interviewer they understood and recreated the function easily.

Usability Map: hovered and clicked accurately with no hesitation and little instruction, only

telling them that there was a hover and zoom feature. Were able to visualize the different data

points and information shown.

Missing Information: analysis on police surveillance and the relationship of these two variables

My sixteen year old sister who’s never been to New York (Interviewee 2)

Narrative: they understand the story. They find the information to be eye-opening

Map: Liked the map. Does not change per year, the year functionality does not add a lot to the

visual.

Usability Visuals: Had a little trouble with the zoom.

Usability Map: Hovered and clicked on points and switched the years very easily.

Missing Information: Wanted more information about the prosecution and the perpetrators

outcome of the case.

Findings both of the Visualizations and the UX Research

1. Figure: Daily Occurrences Over Time

This figure is a line chart that shows there is initially some seasonality to the data because if the

user can observe the pattern that repeats, with the low number of incidents happening during

winter, and the high number of incidents occurring during the summer of each year.

Also this figure shows two dates that could explain some of the variability. The first one is a

marker for July 4th 2020, which was the day with most incidents in the whole dataset, 47 in one

day. This phenomenon probably occurred because of the combination of the summer and the

pandemic, people were inside during lockdown, and during the summer especially July 4th the

people went out a lot.

2. Figure: Occurrences by Hour of the Day

This figure is a vertical bar chart that illustrates how the different hours of the day have different

amount of incidents. It is striking the different values that a change of one hour make. The lower

values are in the hours people go to work, between 5AM and 14PM. The highest point in the

chart is 11PM. Between 14PM and 11PM the number of incident rises on average 200 points.

3. Figure: Occurrences by MonthLine chart that shows the total number of incidents per month. The lowest point is February

(1.6K) The highest is July (3.6K)

4. Figure: Heatmap.

The heat map shows the average number of incidents per month per year. He highest value on the

whole table is July 2020, with an average of 10.5 incidents per DAY. The lowest month was a tie

between March 2017, February 2020 and February 2025, all with an average of 2 incidents per

day.

If you look at the heat map horizontally, it is apparent that the summer months have the highest

averages on average, except for 2017, 2018 and 2019. It is also apparent that January and

February are expected to be low values on average every year.

If you look at the heat map vertically, the 2017-2019 period stands out as a moment in this heat

map when whole years had averages below 5 incidents for every month. It is also noticeable that

these past few years have been very low averaged. Since 2023 there is not a month with more

than 5 incidents per day on average.

The two clouds that appear at first sight are June-September from 2006-2012. The other cloud is

May-September of 2020-2022. Pandemic.

5. Figure: Top 20 Dates with most incidents

All during the summer. Varied In years.

6. Figure: Stacked Vertical Bar Chart: Total Amount of Incidents by Borough colored by race of

the victim.

Brooklyn at the top, bronx second, queens third, Manhattan 4th and staten island last. Most

incidents the victim has been black. Both white hispanics and black hispanics are in second and

third place across all boroughs.

7. Figure: Scatter Plot: Victim Age, Sex, and Race

The biggest bubble is black men in their 25-44 (9039). The second biggest group is black men in

their 18-24 (7193). After that its black men under 18 (2013). After that the race changes but the

sex does not. White hispanic men in their 25-44 (1925), after that its the same group but in their

18-24 (1505). Then we switch races again to black hispanic. In their 25-44 (1229) and 18-24

(1005). Under 18 its around 300 for both hispanic groups.For women, its black women in their 25-44 (766) and in their 18-24 (628), after that is under 18

(330) and 45-64 (222). If we switch to white hispanic women, the highest value is in the group

from 25-44 (241) and then 18-24 (132).

8. Figure: Map ALL

9. Figure: Map per Year

Findings Regarding User Experience:

1. Lack of Transversal analysis. The interviewees would have liked that data be combined and

cross-analyzed with other lateral datasets, so that the analysis seemed richer and more

complex.

2. Sometimes the user needs a tutorial because the audience for this analysis is small; it is for

someone who knows a little python but does not know any visuals or any principle of design.

In retrospect, the analysis could have been complex and intense, having simple visuals or also

difficult to execute and understand ones.

# Article 2: How does Smoking Affect the Risk of Developing Chronic Heart Disease?
##Introduction

Heart disease remains one of the leading causes of death worldwide, and understanding the risk factors behind it is critical for both prevention and early intervention. In this paper, I use data from the well-known Framingham Heart Study to explore what conforms a patient’s risk of developing Coronary Heart Disease (CHD) over a ten-year period. The variable at the center of this analysis is ‘TenYearCHD’, which indicates whether a patient was considered at high risk of experiencing a heart-related event within the next decade. This binary (1 for high risk, 0 for low risk) serves as the outcome in a logistic regression model, which I use to understand and predict heart disease risk.

The dataset used is publicly available on Kaggle and contains a wide range of clinical and demographic information on each patient. These include medical indicators such as blood pressure, cholesterol, heart rate, and glucose levels, as well as lifestyle related variables like smoking habits, medication use, and education level. This rich dataset allows for a deeper investigation into how various factors interact and contribute to the overall risk value of a patient.

The primary aim of this project is twofold: first, to investigate which variables significantly influence a patient's risk classification (specifically smoking habits), and second, to build a model capable of accurately predicting risk for new patients. This article does not just aim to replicate what the researchers have done but also seeks to make the findings more interpretable and relatable to a broader audience.

My particular motivation for conducting this analysis stems from a curiosity about the role of smoking in heart disease. While it is well known that smoking negatively affects the lungs and respiratory system, it is equally important to highlight its role in cardiovascular health. The dataset includes not only whether a patient smokes, but also an estimate on how many cigarettes they smoke per day. This presents an opportunity to examine the nuanced impact of smoking intensity on heart disease risk. By focusing on this factor, I aim to raise awareness about the broader consequences of smoking and show how even data driven models like logistic regression can help visualize and quantify health risks that might otherwise be underestimated.

Background Research

The international Journal of Epidemiology describes the Framingham Heart Study (the FHS) as the “First Large-Scale Cardiovascular Epidemiology Study in the Country” (Tsao, 2015). This premier longitudinal study from the 1950’s stood out as the first of its kind, and many authors acknowledge its importance to the cardiovascular field. This study is remembered as the first to also establish relationships between Cardiovascular Diseases (CVD) and “obesity, systolic blood pressure, high cholesterol and cigarette smoking” (Tsao, 2015). The reason there are many published research papers is because chronic heart disease is one of the leading causes of death and disability worldwide (D’Agostino, et. al., 2013). 

The survey was focused on the town of Framingham, Massachusetts, the study sampled 60% of adults aged 30-69 years, gathering a final sample of 5209 people. The study contained clinical parameters, but also medical family history, X-Rays, EKGs and tests. This all was to capture the multifactorial nature of the disease with a goal to “detect abnormalities thought to play a role in the development of CVD” (Tsao, 2015). 

FHS casted a light on the causes of cardiovascular disease, and the longitudinal structure of the survey provided the adequate format to capture and study the multifactorial “clinical parameters” that may cause CVD, but also the structure of the data is helpful for the increase of the risk over time, since some authors point out that older age is associated with a higher risk of developing Coronary Heart Disease (CHD). The original hypothesis of the FHS, back in 1948, was that CVD was multifactorial (D’Agostino, et. al., 2013). 

Some of the factors that are associated with triggering heart disease are age, sex, cholesterol, blood pressure and smoking (Latifah, Slamet, 2020). Age and Blood pressure have been extensively researched in the last 70 years using mainly the FHS dataset. Age is argued to have a significant effect on contributing as a risk factor to the risk of having heart disease; and many authors find that younger individuals have lower cardiovascular risk and higher overall survival (Terry et al., 2005). 

Along the lines of the multifactor analysis of the FHS, some authors support the interaction between variables to also have a significant effect, for example, cholesterol levels were greater in smokers as compared with non-smokers, meaning that variables amplify synergistically (Tsao, 2015). Other authors found that even though the systolic and diastolic blood pressure are great indicators of possible heart disease, they have similar information. In 1971, a study found that there was a trend of declining relative importance of diastolic BP and a corresponding increase in the relevance of the systolic BP with advancing age, suggesting that these variables could be summarized into one as a predictor (Wilson, Castelli, Kannel, 1987).

Most of these studies train and test logistic regression models, since it has a good classification capability, but some opted for random forests or other regression models (Latifah, Slamet, 2020).

Research Questions

RQ1: How does smoking affect the risk of developing heart disease?

To assess how smoking influences the probability or the odds of developing heart disease in the next 10 years, I will use a Logistic Regression Model. Regression is used to analyze the particular effects, called coefficients, of the different independent variables into the dependent one, so to answer the RQ1, it is necessary to run a regression using smoking data and testing these hypotheses; 

Null Hypothesis: there is no significant effect of smoking into TenYearCHD.

Alternate Hypothesis: there is an effect on average that can be captured of the number of cigarettes smoked a day into the TenYearCHD, to a 5% p value.

RQ2: Can we build a linear model that accurately classifies new data points? 

Testing and iterating for a model that is acceptable, better than guessing at random. For this RQ2, the accuracy should be over 80%, and the precision and recall of the model should all be acceptable. 

Null Hypothesis: there is not a logistic regression model that can accurately predict and classify, with an 80% accuracy, the risk of having chronic heart disease in ten years using the framingham dataset.

Alternate Hypotheses: it is possible to train a logistic regression model that can classify the target variable with an 80% accuracy.

Dataset and Variables

Each row in the dataset represents an individual patient from the town of Framingham, Massachusetts, as part of the well-known Framingham Heart Study. The dataset contains a variety of demographic, behavioral, and clinical attributes used to assess cardiovascular risk.

‘TenYearCHD’: ‘TenYearCHD’ is the target binary variable, representing whether a patient is at risk of developing coronary heart disease (CHD) within the next ten years, based on clinical assessments and historical data; a value of 1 means the patient is classified as risky. It is important to clarify that this variable reflects predicted risk. In this dataset, about 15% of the total sample (562 patients) are labeled as being at high risk for CHD. This class imbalance should be kept in mind when evaluating model performance, especially in terms of precision and recall, as the model might tend to favor predicting the majority class (no risk) without careful tuning.

‘Male’: is a binary indicator that denotes the sex of each individual in the dataset, with a value of 1 representing male. Out of the total 3,750 individuals remaining in the cleaned final dataset 2419 are female, meaning that women make up a slightly larger portion of the sample (64%). 

‘PrevalentHyp’: is a binary indicator that shows whether a patient has a history of hypertension. A value of 1 indicates that the patient has been diagnosed with hypertension. In this dataset, 1316 individuals have a history of hypertension (35%).

‘Glucose': represents each patient's blood glucose level and is measured as a continuous numerical value. Values range from a low of 45 to a high of 400, indicating a wide spread in the data. The distribution is notably right-skewed, meaning that while most patients have relatively normal glucose levels, there is a small number of individuals that exhibit extremely high values. A closer look at the summary statistics reveals that the median glucose level is 78, and the mean is slightly higher at 82, which again reflects the influence of outliers on the distribution. The interquartile range (IQR), spans from 71 to 87.

An issue with this variable is the relatively high number of missing values. Nearly 10% of the entries for glucose are missing, so I opted for listwise deletion, meaning that any individual with a missing value for any variable, not just glucose, was removed from the dataset. While this approach ensures that the data used in modeling is complete, it comes at a cost: the dataset shrank by approximately 13%, leaving 3750 individuals for analysis out of the original sample.

‘Age’: ranges from 32 to 70 years old, with both the mean and median at 49 years old, suggesting a symmetrical distribution overall. This dataset is not the longitudinal FHS, each row is a person. There is a heavier concentration of younger individuals, particularly those between the ages of 32 and 45. As people grow older, their expected likelihood of developing cardiovascular conditions increases.

‘CigsPerDay’: represents the number of cigarettes smoked per day by each patient and ranges from 0 to 70 cigarettes. 2144 individuals report zero cigarettes per day, meaning that they do not smoke. Among the smokers, there is a noticeable concentration of patients who smoke 20 cigarettes a day, with a smaller group consuming 30 cigarettes daily. There were 29 missing values (NA), and the distribution of this variable is skewed, with a heavy mass at 0, and it highlights the challenge of modeling continuous variables when many individuals report no smoking at all.

‘TotChol’: ‘Total Cholesterol’ represents the cholesterol level in the blood, recorded as a continuous variable ranging from 100 to 700 mg/dL. This variable had 50 missing values. The distribution shows that about 60% of the individuals have cholesterol levels exceeding 240 mg/dL, which is typically considered a health risk threshold for cardiovascular disease. The mean cholesterol level is 236 mg/dL, while the median is 234 mg/dL, indicating a relatively symmetric distribution with a slight right skew.

‘SysBP’: represents the systolic blood pressure, which measures the pressure in the arteries when the heart beats. This is an essential indicator of cardiovascular health. The values in the dataset range from 70 to 300 mmHg, with 50% of the individuals having systolic blood pressure levels at or below 140 mmHg. The average systolic blood pressure is 132 mmHg, while the median is 128 mmHg, and the mode is 120 mmHg, suggesting that 120 is a commonly observed value in the dataset. Blood pressure readings higher than 140 mmHg are generally considered a sign of hypertension, which significantly increases the risk of heart disease, stroke, and other cardiovascular problems. 

‘DiaBP’: is the diastolic blood pressure, which measures the pressure in the arteries when the heart rests between beats. The values in the dataset range from 40 to 150 mmHg, with 50% of the individuals having diastolic blood pressure levels at or below 80 mmHg. The mean diastolic blood pressure is 83 mmHg, while the median is 82 mmHg, indicating a fairly symmetric distribution. High diastolic blood pressure (generally considered above 90 mmHg) is associated with an increased risk of heart disease and stroke, especially when combined with high systolic blood pressure.

Healthy individuals typically have a sysBP under 120 mmHg and a diaBP under 80 mmHg.

Hypertension tends to be diagnosed when sysBP is between 130-180 mmHg and diaBP is between 80-110 mmHg, and a Hypertension Crisis occurs when sysBP exceeds 180 mmHg and diaBPexceeds 120 mmHg.

‘Education’: a categorical feature ranging from 1 to 4, indicating the patient’s highest level of education. Education level might not be directly relevant to health outcomes in this specific context. I chose to discard this variable early in the analysis.

‘CurrentSmoker’: binary indicator that identifies whether a patient currently smokes. Including this binary variable in the model seems redundant since the cigarettes per day data is more insightful to quantify the relationship between smoking status and the likelihood of being classified as high-risk for heart disease.

‘BPMeds’: binary indicator that shows whether a patient is currently taking medication for blood pressure. A value of 1 indicates that the patient takes medication, while a value of 0 indicates that the patient is not.

‘Prevalent Stroke’: binary indicator that denotes whether a patient has a history of stroke. Only 25 individuals in the whole dataset have a stroke recorded, which represents a very small proportion of the sample. Given the low prevalence of this condition, including the variable in the model would not provide much predictive power. 

‘Diabetes’: binary indicator that shows whether a patient has been diagnosed with diabetes. In this dataset, only 109 individuals have diabetes, while the remaining 4,129 do not. Although diabetes is a major risk factor for coronary heart disease, the relatively low number of individuals with diabetes in this dataset may limit its impact in the logistic regression model.

‘BMI’: continuous index of a patient's body mass, calculated using height and weight. There are 19 missing values in this column.

‘HeartRate’: continuous measure of a patient’s resting heart rate, with values in the dataset ranging from 40 to 140 beats per minute (bpm).

Correlations

The correlation analysis revealed several notable relationships among the continuous variables. On the negative side, there were modest inverse correlations between age and the number of cigarettes smoked per day (-0.19), as well as between systolic blood pressure (SysBP) and cigarette consumption (-0.09), suggesting that younger individuals with lower blood pressure tend to smoke more. On the other side, age showed moderate positive correlations with total cholesterol (0.26), systolic blood pressure (0.39), and prevalent hypertension history (0.31), while systolic blood pressure was also positively correlated with total cholesterol (0.22) and prevalent hypertension history (0.70). When examining the relationship between the continuous variables and the target variable, TenYearCHD, the highest correlations were found with age (0.23), systolic blood pressure (0.22), glucose (0.12), and total cholesterol (0.09), indicating these factors are more closely associated with coronary heart disease risk. All of these positive correlations suggest that the older the individual is, they are associated with a higher cholesterol, higher blood pressures, higher glucose levels and a considerably smaller amount of average cigarettes smoked. This also results in this group of individuals to be associated with a higher predicted risk on average. 

Among the binary variables, some meaningful patterns also emerged. There were negative correlations between being a current smoker and having a history of hypertension (-0.10), between taking blood pressure medication and being male (-0.05), and between BP medication use and current smoker (-0.05). Positive correlations were observed between blood pressure medication and hypertension history (0.26), between male and current smoking status (0.20), and between having diabetes and hypertension history. In terms of the target variable, the strongest binary correlations were found with prevalent hypertension (0.18) and male gender (0.10), both of which showed some association with increased coronary heart disease risk.

Risky Patients Subset

After this initial assessment of the variables, I created a subset of the data that only contains individuals that were assigned risk level 1, meaning that these individuals are the ones who were estimated to be at risk in ten years for CHD by the framingham study. This subset of the data is the Risky People Analysis, and some of the correlations show best when studying the risky people, such as: Systolic Blood Pressure vs Diastolic Blood Pressure (correlation of 0.79), Age vs Cigarettes Smoked Per Day (-0.19), and Age vs Pulse Pressure (0.39), which is the result of the subtraction between Systolic and Diastolic BP. SysBP and DiaBP are highly positively correlated, and there is a clear trend of both variables increasing. For the risky people, sysBP ranges from 75 to 300 and diaBP ranges from 50 to 150. The group of risky people who had a history of hypertension have a much higher average of both blood pressures than the individuals who did not have hypertension. This is because with a diagnosis of Hypertension, higher values of BP are expected. 

While analyzing the relationship between Age and CigsPerDay, there is a clear decline in the amount of cigarettes smoked with the increasing age. It is expected that with aging, more and more patients are willing to smoke less or quit. There is a negative correlation between age and cigarettes smoked per day. Additionally, of the group of risky people, there is a difference in how many people smoke compared to the original dataset, there are far less ‘0’ values. Which suggests that smoking may be one of the indicators of what determines the risk level of a patient. For the patients with a history of hypertension, the number of cigarettes smoked per day is considerably lower than for those who do not have a history of hypertension. 

The last variable relationship is age and pulse pressure (PP), which is a calculated variable that results from the subtraction of the diaBP from the sysBP. In this form, we can summarize the effect of both Blood Pressures, and compare that calculated variable to Age. The Pulse Pressure goes from 35 to 70. There is a clear positive correlation between age and PP, which is expected because older patients tend to have a higher Blood Pressure which could lead to other health problems. Again, patients with a history of hypertension have a much higher average of pulse pressure, since hypertension is linked to a higher blood pressure value. 

Methodology

The main hypothesis is: How does smoking cigarettes affect the probability of the risk of developing heart disease? With the null hypothesis being that there is no effect of smoking on the level of risk assigned to the individual. To test this hypothesis I will use a logistic regression model, which is appropriate for a binary outcome variable and continuous or categorical predictors such as number of cigarettes smoked per day. The model coefficients cannot be directly interpreted in terms of the increased or decreased likelihood of heart disease, but the odds ratio is an indicator of the impact of one variable over the outcome. Can we predict the risk of CHD? That is our second hypothesis. In order to test for this, I decided to try 4 different logistic regressions in order to see which is the best model in terms of accuracy and R².

To test for these two hypotheses we must establish a threshold. For the first one, I suppose that the ‘currentSmoker’ binary variable does not have a significant impact on the risk of CHD, but rather ‘cigsPerDay’, may have a statistically significant effect. If this is the case, the odds of assigning a level of risk to a patient are higher for those who smoke, and those who smoke a lot. The second hypothesis tests for predictability. The model that predicts most correctly should have an accuracy of at least 85%, and a high  R² too. If this turns out to be the case, then our model could very well be used to assign a level of risk to a new data point. 

Models

To train these models, it is important to randomly split the dataset into two sets; train and test, with an 80-20 split, which means 80% of the data is used to train the model and the test set is used to evaluate how the model reacts to new data points. 

Model 1: Logistic Regression 

The first model includes all the variables in our data. Only some variables prove to have a significant effect on the outcome variable. These are; age, male, cigs per day, prevalentHyp, totChol, sysBP and glucose.

It is important to test the multicollinearity assumption, this means that there should be a VIF (variance inflation factor) analysis of the variables being used in the model. All variables should have a coefficient equal to or lower than 3, and the VIF (Variance Inflation Factor) for this model shows that both ‘sysBP’ and ‘diaBP’ exceed this threshold. This suggests that the model may be suffering from multicollinearity, meaning that these variables are strongly correlated with one or more other predictors in the model, or each other. Multicollinearity can inflate the standard errors of the coefficients, making them less reliable and potentially distorting the interpretation of the model. To improve the model, it may be necessary to remove or combine correlated predictors.

The variables that the model determines have a statistically significant effect are male, age, cigsPerDay, prevalentHyp, totChol, sysBP, and glucose. However, these coefficients have to be modified to be interpreted accurately, in terms of odds ratios and if the variable increases in one unit, the expected effect is either going to be positive, negative or none. The odds ratios are compared to 1, if they are close to 1 then the effect is minimal or zero, if the odds are positive then there is an associated increase in the odds of the event occurring, and if the odds are negative then on average, the odds of the event happening are diminished. 

The logistic regression results suggest that the odds of being classified as high risk for coronary heart disease (CHD) are 65% higher for males compared to females. This means that, holding other variables constant, being male significantly increases the likelihood of CHD risk. Age has an odds ratio of 6.7%, meaning that for each additional year of age, the odds of being at risk increase by 6.7%. This is particularly relevant since the youngest individuals in the dataset are 32 years old, and risk appears to increase steadily with age.

The variable CigsPerDay shows that for each additional cigarette smoked per day, the odds of CHD risk increase by 2.0%. This reflects the compounding effect of daily smoking on heart health over time. Having a history of hypertension (PrevalentHyp) raises the odds of being at risk by 30%, emphasizing that past or existing blood pressure problems are a strong predictor of future heart conditions. Total cholesterol (totChol) has a smaller but still measurable effect, with an odds ratio of 0.22% per unit. This means that for every 1 mg/dL increase in cholesterol, the odds of CHD risk increase by 0.22%, highlighting the cumulative effect of having high cholesterol levels.

For systolic blood pressure (sysBP), the odds increase by 1.5% per mm Hg. This indicates that higher systolic pressure is meaningfully associated with greater CHD risk, aligning with medical guidelines that classify elevated blood pressure as a key risk factor. Lastly, glucose levels have an odds ratio of 0.94% per unit, meaning that for every mg/dL increase in blood glucose, the odds of being considered high-risk go up slightly, underscoring how metabolic health also contributes to cardiovascular outcomes.

Model 2: Stepwise Logistic Regression

The second model uses the first model as an input, and chooses to remove variables based on a certain criteria that can be specified. In this case, the stepwise model selects variables, or predictors, based on the AIC (Akaike Information Criterion), and the iteration with the lowest AIC value is returned. The direction of the stepwise is crucial, forward starts with an empty model and adds predictors, the backwards approach starts with all of them and then starts removing variables, but both directions are usually used at once, finding the best-fitting model. This best model is the one that retains the least amount of variables that predict a significant amount of the variance. 

After running the stepwise model, the resulting regression output showed that the Variance Inflation Factor (VIF) values were all below the threshold of 3, including for variables like ‘sysBP’ which previously indicated potential multicollinearity concerns. Specifically, having no VIF value above 2.0 suggests that the model no longer suffers from problematic levels of multicollinearity, meaning that the predictors included in the final model are not excessively correlated with one another. The variables that the model chose to keep are the same ones as the first,  but only keeping the ones that had a significant effect on the predicted variable; male, age, cigsPerDay, prevalentHyp, totChol, sysBP, and glucose.

The logistic regression results suggest that the odds ratios of the stepwise model are similar to the first model. Being classified as high risk for coronary heart disease (CHD) is still 65% higher for males compared to females. Age suffered an increase in the odds ratio to 6.8%. CigsPerDay shows that for each additional cigarette smoked per day, the odds of CHD risk increase by 2.2%. Having a history of hypertension (PrevalentHyp) has a smaller effect but still raises the odds of being at risk by 28.6%. Systolic blood pressure (sysBP) kept the same effect, the odds increasing by 1.4% per mmHg. Total cholesterol (totChol) maintained a smaller effect, with an odds ratio of 0.20% per increase of ml/dL. Lastly, glucose levels diminished the first odds ratio to 0.90% per unit.

The results from the logistic regression show that the model I built is significantly better at predicting heart disease risk than a model with no variables at all. In statistical terms, the reduction in ‘deviance’ (302.5) tells us how much better our model is at explaining the outcome, and the improvement is quite large. I also looked at how many variables were used to get this improvement, there were 7 key predictors selected. To check whether this improvement could have happened just by chance, I used a chi-squared test that returned an extremely small p-value (basically zero), meaning it's very unlikely that our results are random. Overall, this tells us that our model is useful and meaningful for identifying patients at higher risk of heart disease.

Model 3: Logistic Regression with Interaction Terms

To strengthen the predictive power of my model while keeping it grounded in clinical logic, I selected four additional variables based on well-established patterns in cardiovascular research. First, I introduced a binary variable for individuals with a diastolic blood pressure over 110 (High diaBP), as this level is clinically recognized as dangerously high and strongly associated with hypertensive crisis, making it a meaningful threshold for risk assessment. I also categorized age into three distinct groups; young adults (32–45 years old), middle-aged adults (45–60 years old), and older adults (60–70 years old). To reflect how heart disease risk accelerates in non-linear ways across life stages, this was to prove that being old has a different impact than being young, rather than an interpretation of years increasing and risk increasing with each one. Next, I created a binary variable for heavy smokers, defined as those who smoke more than 10 cigarettes per day. This cut-off is informed by studies showing significantly elevated cardiovascular risk among heavier smokers and the distribution of the variable cigsPerDay showed this group of individuals, distinguishing them from occasional or light smokers. Finally, I added an interaction term between ‘prevalent hypertension’ and ‘male’ to capture the sex-based differences in how high blood pressure contributes to heart disease. These additions allow the model to reflect more nuanced patterns of risk, consistent with the literature, without overfitting or relying on overly complex variable structures.

The variables that the model identified as statistically significant include: male, total cholesterol, systolic blood pressure, glucose, high diastolic blood pressure, age group indicators for ‘old’ and ‘young’, heavy smoker status, and the interaction between male and hypertension. Notably, variables such as the regular age variable, the "middle-aged" category, cigarettes per day, prevalent hypertension and diastolic blood pressure were excluded. This is likely because including all closely related or overlapping variables would cause the model to overfit by perfectly capturing the variation in the data. The VIF analysis indicated that systolic blood pressure (sysBP) has a value exceeding 3, suggesting the model is affected by multicollinearity. 

The odds of being at risk for coronary heart disease are 51% higher for males compared to females. Individuals with high diastolic blood pressure (greater than 110) have a 54.8% higher likelihood of being at risk. The odds of being at risk increase by 64% for those categorized as "old" (ages 60-70), while the odds decrease by 64.3% for "young" individuals (ages 32-45) when compared to the reference group. Heavy smokers (smoking more than 10 cigarettes per day) are 67.2% more likely to be at risk for coronary heart disease. Additionally, the odds for individuals with both male gender and a history of hypertension are 28.6% higher compared to others. For every one mmHG increase in systolic blood pressure, the odds of being at risk increase by 1.6%. As glucose levels increase, the odds of being at risk increase by 0.97%, while for total cholesterol, the odds of being at risk increase by 0.26% for every unit increase in cholesterol. 

Model 4: Stepwise Logistic Regression with Interaction Terms

The fourth model uses the third model as an input, and removes or selects variables, or predictors, based on the AIC (Akaike Information Criterion), and iterates until the lowest AIC value is obtained with the best iteration. This model is the one that retains the least amount of variables that predict a significant amount of the variance. The Variance Inflation Factor (VIF) values were all below 3 for all variables, including ‘sysBP’ which previously indicated potential multicollinearity. Specifically, having no VIF value above 1.7 suggests that the model does not have surprising levels of multicollinearity. The statistically significant variables that the model kept are the same ones as the third model, but only the ones that had a significant effect on the predicted variable; male, cigsPerDay, prevalentHyp, totChol, sysBP, glucose, highDiaBP, old, young, heavy_smoker and male_hypertension.

The odds ratios of this stepwise model are similar to the third model. Being classified as high risk for coronary heart disease (CHD) is 53% higher for males compared to females. Old individuals have a higher risk at 64%, but if the individual is young, is it expected to still have a decrease of 64%. HeavySmokers shows that for people who smoked more than 10 cigarettes a day, the odds of CHD risk increase even more in the stepwise model, from 67% to 71%. If the patient is a male and also has a history of hypertension (Male_Hypertension) the odds of being a risky patient are still 28%. Systolic blood pressure (sysBP) kept the same effect, the odds increasing by 1.6% per mmHg increased. Total cholesterol (totChol) maintained the smaller effect, with an odds ratio of 0.25% per increase of ml/dL. Glucose levels kept the same odds ratio as the third model, with an increase of 0.92% per unit. 

Results



RQ1: How does smoking affect the risk of developing heart disease?

Across all four models, the variable ‘currentSmoker’ lost statistical significance when ‘cigsPerDay’ was included, suggesting that the number of cigarettes smoked daily captures more meaningful variation than simply whether someone smokes. Interestingly, the ‘cigsPerDay’ variable itself had a skewed distribution, with nearly half of the observations being zero, effectively preserving the information from the original binary smoker variable while adding granularity. In both Models 1 and 2, ‘cigsPerDay’ showed a statistically significant effect (p-value < 0.001) on the likelihood of developing heart disease, with odds ratios of 2.0% and 2.2%, respectively. This implies that each additional cigarette smoked per day is associated with approximately a 2.2% increase in the odds of being classified as high-risk, holding other factors constant. Models 3 and 4 replaced ‘cigsPerDay’ with a binary variable ‘Heavy_Smoker’, defined as smoking 10 or more cigarettes per day. This new variable was also statistically significant in both models, with odds ratios of 67.2% and 70.8%, indicating a substantial increase in risk for heavy smokers compared to those who smoke less or not at all.

RQ2: Can we build a linear model that accurately classifies new data points?

To evaluate whether a logistic regression model can classify future chronic heart disease (CHD) cases with at least 80% accuracy, four different models were constructed and compared using a range of performance metrics. Model 1 included all 13 available variables, while Model 2 applied stepwise regression to Model 1, reducing the number of predictors to 7. Similarly, Model 3 extended the feature set by engineering new binary and interaction variables, resulting in 14 predictors, and Model 4 applied stepwise regression to Model 3, ending with 9 variables.

All four models demonstrated high accuracy, ranging from 84.8% to 85.5%, successfully surpassing the 80% threshold outlined in the alternate hypothesis. This suggests that a logistic regression model can, at least in terms of accuracy, outperform random guessing and provide meaningful classification of individuals at risk of developing CHD within ten years. However, accuracy alone is insufficient when evaluating predictive performance on an imbalanced dataset like this, where non-events (no CHD) dominate. As such, precision and recall offer additional insight.

Precision is the proportion of predicted positives that are actually positive, going from 0.425 to 0.487 across models. Model 4 achieved the highest precision, indicating that nearly half of its CHD-positive predictions were correct. While promising, this still means that over half of predicted cases may be false positives. Recall, or sensitivity, was more concerning. All four models returned low recall values (~0.157 to 0.176), meaning that the models missed around 82% to 84% of actual CHD cases. This suggests the models are far more likely to correctly predict who won’t get CHD than who will.

The McFadden’s R² values, which range from 11.14% to 11.76%, suggest that while the models do better than a null model, they explain only a modest portion of the variance in the outcome. The small variation in McFadden’s R² across models indicates that the feature engineering in Model 3 and its stepwise reduction in Model 4 did not dramatically improve explanatory power over the original models.

The Akaike Information Criterion (AIC) provides a measure of model quality that penalizes complexity. Model 2 had the lowest AIC (2301), suggesting that it offers the most efficient trade-off between fit and simplicity. The difference in deviance, how much the model improves from the null model, was highest for Model 1 (304) and lowest for Model 4 (288), though the differences are relatively minor. The Area Under the Curve (AUC) values also hovered around 0.72–0.74, with Model 2 slightly outperforming the rest (0.7428), confirming that all models perform moderately well in distinguishing between positive and negative CHD cases.

In conclusion, the findings support the alternate hypothesis that a logistic regression model can predict CHD risk with over 80% accuracy. However, the low recall across all models raises concerns about their ability to reliably identify at-risk individuals. While Model 4 offers the highest precision and accuracy, Model 2 performs best in terms of overall model quality (lowest AIC and highest AUC). Future iterations could explore alternative modeling techniques, such as random forests or penalized logistic regression, to improve recall without sacrificing accuracy or interpretability.

Conclusion

All Models estimated the effects of smoking, but only 3 and 4 estimated that being a heavy smoker increases the patients odds by 70% of being classified ‘at risk’ of developing heart disease in ten years. The effect of the higher smoking data points is statistically significant (p value = 0). 

Model 4 emerges as the best-performing model overall. It achieves the highest accuracy, precision, and recall among all four models tested. While it includes more variables than the most minimal models, its enhanced predictive power makes it the most effective at correctly identifying individuals at risk. The model strikes a solid balance between complexity and performance, demonstrating strong classification ability in a real-world health context.

This model showed that understanding the data, and diving into the medical research can improve a simple logistic regression, and achieve better metrics.  In this case, some continuous variables could be switched by a binary factor that indicated presence of a high value or not; diastolic blood pressure and cigarettes smoked per day, into binary factors high diastolic BP and heavy smoker. An added variable of ‘age’ also made the effects more interpretable. The three new age groups indicated that being young lowered the risk and being old increased the risk of having heart disease. Not only did these new variables improve the original model in predictability, but it made the results more interpretable, and higher odds easier to understand. The models all showed an R²  over 10%, which is considered standard for the medical field and this type of classification study. 

Both Null hypothesis were rejected, and the alternate hypothesis were supported by the results; it is possible to build a good logistic regression model, and there is a significant effect of being a heavy smoker on the risk of having heart issues in ten years.  

Visualizations



Histogram: Age Variable Distribution, separated by risk group ‘TenYearCHD’



Histogram: CigsPerDay Variable Distribution, the variable shows how many individuals smoke how many cigarettes per day.



Histogram: totChol Variable Distribution, the variable contains the values of total Cholesterol in each patient.



Histogram: sysBP Variable Distribution, the variable sysBP contains the data for the systolic blood pressure of the patients. Additionally, the histogram is separated by the risky group of individuals and the not risky patients.



Histogram: diaBP Variable Distribution, the graphs shows the diastolic blood pressure of the patients, separated into the two groups of patients; risky and not risky. 



Histogram: BMI Variable Distribution, the graph shows the distribution of the Body Mass Index variable. 



Histogram: HeartRate Variable Distribution, the histogram shows the values of the heart rate of all the patients. 



Matrix: Correlations of Continuous Variables, the matrix shows the correlation between all of the continuous variables in the dataset.



Matrix: Correlations of Binary Variables, the matrix shows the correlation between all of the continuous variables in the dataset.



Matrix: Correlations of All Variables



ScatterPlot: SysBP versus DiaBP, legend = PrevalentHyp, and the data is the subset of risky individuals, meaning TenYearCHD ==1. The graph shows how the values interact with each other, the trends, and the differences between the two groups; people with hypertension or not. 



ScatterPlot: Age versus CigsPerDay, legend = PrevalentHyp, and the data is the subset of risky individuals, meaning TenYearCHD ==1. The graph shows how the values interact with each other, the trends, and the differences between the two groups; people with hypertension or not. 



ScatterPlot: Age versus PP (Pulse Pressure), legend = PrevalentHyp, and the data is the subset of risky individuals, meaning TenYearCHD ==1. The graph shows how the values interact with each other, the trends, and the differences between the two groups; people with hypertension or not. 



Regression Summary: Model 1 logistic regression output.



VIF Analysis Summary: Model 1 logistic regression Variance Inflation Factor Table



Odds Ratio: Model 1 logistic regression odds ratio table.



Regression Summary: Model 2 Stepwise model regression output: 



VIF Analysis Summary: Model 2 stepwise regression Variance Inflation Factor:



Odds Ratio: Model 2 stepwise regression odds ratio table.



Regression Summary: Model 3 logistic regression with interaction terms and new variables regression output table.



VIF Analysis Summary: Model 3 logistic regression Variance Inflation Factor:



Odds Ratio: Model 3 logistic regression odds ratios table.



Regression Summary: Model 4 stepwise model regression output table.



VIF Analysis Summary: Model 4 logistic regression Variance Inflation Factor:



Odds Ratio: Model 4 logistic regression odds ratio table.

References

WHO. “Cardiovascular Diseases (CVDs),” June 11, 2011. https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds).

Olvera Lopez, Edgardo, Brian D. Ballard, and Arif Jan. “Cardiovascular Disease.” In StatPearls. Treasure Island (FL): StatPearls Publishing, 2025. http://www.ncbi.nlm.nih.gov/books/NBK535419/.

Tsao, Connie W, and Ramachandran S Vasan. “The Framingham Heart Study: Past, Present and Future.” International Journal of Epidemiology 44, no. 6 (December 1, 2015): 1763–66. https://doi.org/10.1093/ije/dyv336.

D’Agostino, Ralph B., Michael J. Pencina, Joseph M. Massaro, and Sean Coady. “Cardiovascular Disease Risk Assessment: Insights from Framingham.” Global Heart, Framingham Legacy Issue, 8, no. 1 (March 1, 2013): 11–23. https://doi.org/10.1016/j.gheart.2013.01.001.

Franklin, Larson, Khan, Wong, Leip, Kennel, and Levy. “Does the Relation of Blood Pressure to Coronary Heart Disease Risk Change With Aging?” In Circulation, Vol. 103 (Issue 9), 2001. https://doi.org/10.1161/01.CIR.103.9.1245.

Detrano, Robert, Andras Janosi, Walter Steinbrunn, Matthias Pfisterer, Johann-Jakob Schmid, Sarbjit Sandhu, Kern H. Guppy, Stella Lee, and Victor Froelicher. “International Application of a New Probability Algorithm for the Diagnosis of Coronary Artery Disease.” The American Journal of Cardiology 64, no. 5 (August 1989): 304–10. https://doi.org/10.1016/0002-9149(89)90524-9. 

Brand, Richard, Ray Rosenman, Robert Sholtz, and Meyer Friedman. “Multivariate Prediction of Coronary Heart Disease in the Western Collaborative Group Study Compared to the Findings of the Framingham Study.” 53, no. 2 (February 1, 1976): 348–55. https://doi.org/10.1161/01.CIR.53.2.348.

Castelli, WilliamP, ThomasR Dawber, Manning Feinleib, RobertJ Garrison, PatriciaM Mcnamara, and WilliamB Kannel. “THE FILTER CIGARETTE AND CORONARY HEART DISEASE: THE FRAMINGHAM STUDY.” The Lancet, Originally published as Volume 2, Issue 8238, 318, no. 8238 (July 18, 1981): 109–13. https://doi.org/10.1016/S0140-6736(81)90297-X.

Terry, Dellara F., Michael J. Pencina, Ramachandran S. Vasan, Joanne M. Murabito, Philip A. Wolf, Margaret Kelly Hayes, Daniel Levy, Ralph B. D’Agostino, and Emelia J. Benjamin. “Cardiovascular Risk Factors Predictive for Survival and Morbidity-Free Survival in the Oldest-Old Framingham Heart Study Participants.” Journal of the American Geriatrics Society 53, no. 11 (2005): 1944–50. https://doi.org/10.1111/j.1532-5415.2005.00465.x.

Latifah, Firda Anindita, Isnandar Slamet, and Sugiyanto. “Comparison of Heart Disease Classification with Logistic Regression Algorithm and Random Forest Algorithm.” AIP Conference Proceedings 2296, no. 1 (November 16, 2020): 020021. https://doi.org/10.1063/5.0030579.

Wilson, Peter W. F., William P. Castelli, and William B. Kannel. “Coronary Risk Prediction in Adults (The Framingham Heart Study).” The American Journal of Cardiology, A Symposium: Doxazosin: Coronary Artery Disease Risk Factor Management, 59, no. 14 (May 29, 1987): G91–94. https://doi.org/10.1016/0002-9149(87)90165-2.

Castelli, W. P. “Epidemiology of Coronary Heart Disease: The Framingham Study.” The American Journal of Medicine, Coronary Heart Disease: Hypertension and Other Risk Factors, 76, no. 2, Part A (February 27, 1984): 4–12. https://doi.org/10.1016/0002-9343(84)90952-5.

Salton, Carol J., Michael L. Chuang, Christopher J. O’Donnell, Michelle J. Kupka, Martin G. Larson, Kraig V. Kissinger, Robert R. Edelman, Daniel Levy, and Warren J. Manning. “Gender Differences and Normal Left Ventricular Anatomy in an Adult Population Free of Hypertension. A Cardiovascular Magnetic Resonance Study of the Framingham Heart Study Offspring Cohort.” Journal of the American College of Cardiology 39, no. 6 (March 20, 2002): 1055–60. https://doi.org/10.1016/s0735-1097(02)01712-6.

Shu, Ting, Bob Zhang, and Yuan Yan Tang. “Effective Heart Disease Detection Based on Quantitative Computerized Traditional Chinese Medicine Using Representation Based Classifiers.” Evidence-Based Complementary and Alternative Medicine 2017, no. 1 (2017): 7483639. https://doi.org/10.1155/2017/7483639.

# Article 3: Navigating Social Media as a Transgender User: Comparing Different Community Standards, Content Moderation, Legal Name Policy and the Dangers of Far Right Wing Anti-Trans Rhetoric.
## Comparing Different Community Standards, Content Moderation, Legal Name Policy and Politics.

Abstract:

Social media platforms play a pivotal role in shaping the experiences and identities of transgender individuals online. My interest in social media policies began after reading the article “Tumblr was a Trans Technology”, which highlighted Tumblr’s unique ability to foster fraternity, openness, and visibility for transgender users, particularly through its allowance of gender-affirming surgery images. However, Tumblr’s trajectory changed significantly after its temporary shutdown and subsequent return with new, restrictive policies. These shifts underscore the importance of critically examining how social media platforms construct and enforce their community guidelines. This seminar paper compares the policies of some major social platforms—Meta, Twitter, TikTok, and Tumblr—to evaluate how they address the needs of transgender community members, especially in adult and gender reassignment surgery content. Drawing from my own lived experience as a transgender person who discovered and explored my identity through social media, I propose a set of recommendations for social media designers aimed at creating safer, more inclusive digital spaces for transgender individuals, but mostly how we can change the actual platforms that exist today.  

In addition, this paper critically analyzes the rhetoric propagated by some right-wing scholars and politicians who argue “How Big Tech Turns Kids Trans”. Such claims not only stigmatize transgender individuals but also pose significant risks to the safety and well-being of LGBTQ+ groups online. By combining my personal insight, policy analysis, and a critique of harmful rhetoric, this work aims to illuminate the challenges faced by transgender users while providing actionable solutions and recommendations to social media platforms for fostering inclusive online environments.

Introduction

This paper aims to explore social media and its role in being a safe space for transgender users. Combining my own experience online, social media policies, why far right-wing anti-trans rhetoric is dangerous and provide a set of recommendations based on these aspects; social media policy regarding gender reassignment surgery content, far right-wing rhetoric on ‘big tech turns kids trans’ (Eckert, 2019), analyzing Tumblr as a case study (Haimson, Oliver L., Dame-Griff, Capello, Richter., 2021), and contributing with my knowledge as a trans user on social media. These recommendations aim to express what aspects of current companies could change to improve the trans experience online. 

Social media must serve as a haven for minorities who lack exposure to their stories in offline life. There is immense power in information, and had I not been exposed to trans narratives online during my adolescence. This seminar paper seeks to examine the policies social media platforms implement—whether they empower and protect or fall short in fostering a supportive space for transgender users. It will also provide direction for future and current social media developers and companies on how to create more inclusive online environments.  

My life online as a trans person has been mostly positive, and the hate speech I have endured online does not compare to physical altercations in real life. I argue that for me, social media was more of a safe space to show my true character, because of the power of community that is created and inherently part of social media. Our world has never been more connected and it keeps getting more technologically enhanced constantly. Social media companies should realize the power that information has to trans users, medical or not, just information about transness and trans people, and not try to only profit from their platforms and content. 

I was assigned male gender at birth, but I now identify as a transgender woman. For me, there is no history of transgender individuals on either side of my family. I was born and raised in the suburbs of Montevideo, Uruguay—a small Latin American country whose capital has a population of around 1.5 million people. Growing up, my social environment lacked visible trans people in my family, in my private school, in my small neighborhood in the suburbs, and overall social context. I am not oblivious to the fact that trans people have existed and still exist in Uruguay, but my first encounter with a trans person was online. 

From a young age, I always felt different from the boys around me. I felt an ongoing pull toward belonging to the girls' groups, a feeling that eventually helped me better understand who I am today.

This sense of difference always felt intrinsic to me, as though I wasn’t meant to fit neatly into the binary. My personality, interests, and identity were in constant conflict with the male gender shaped and constructed by my social context. Yet, I couldn’t fully belong with the girls either due to my anatomy and chromosomes. As a result, I found myself engaging in what I now remember as “binary, forced cisgender events”—playing boys’ sports like soccer and rugby, wearing the male school uniform, and dressing in male-coded clothing outside of school. These experiences, though deeply misaligned with me, have shaped the person I am today. From as early as I can remember, there has been a fundamental rejection of the male gender within me, paired with an enduring fascination with the female gender. I didn’t want to play those sports, wear those clothes, or live the life expected of a little boy. There is a very evident breaking point for me, the first time I got called ‘pretty’ instead of ‘handsome’. I realized I wanted to be perceived as a girl because that was and is my identity, what feels accurate according to my knowledge. 

It was through online platforms like YouTube that I first encountered what it meant to be transgender. Watching creators like Gigi Gorgeous helped me find language and helped me figure out who I was, and connect to a broader population.  During my teenage years, I began to learn more about being transgender, primarily through social media and online groups. I was captivated, though I could not fully explain why. At 17, while discussing my struggles with the male gender and my place within the gay male gender stereotype—I had come out as gay at 15—a friend asked me, “Are you sure you’re not just trans?” My immediate response was, “Of course not.” At the time, I had been conditioned by my social context to see transgender people as mentally ill, or even associated with sex work. There wasn’t a single defining moment when I was told that being transgender was wrong, but certain experiences left a lasting impression. I remember one time, around the age of 10 when I wore my mother’s dresses and organized a “runway show” with my male friends as the audience. My stepfather pulled me aside and asked if boys my age were also doing this and whether it was “normal.” I lied and said, “Yes.” That moment crystallized for me the realization that my interests and identity set me apart from other boys—a difference I had already felt deeply and which likely contributed to the years of bullying I endured for being gay, feminine, or “girly.”

The power of social media during my teenage years was immense—it became a safe space, a protective blanket shielding me from the often unwelcoming outside world. Online, I found representation and inspiration, particularly through trans women like Laverne Cox in “Orange Is the New Black”. Her 2014 interview with TIME encapsulates why social media has such a profound impact on transgender teenagers. She stated, “We’re able to have a voice in a way that we haven’t been able to before. We’re being able to write our stories and we’re being able to talk back to the media” (Steinmetz, Katy., 2014). This ability to see and hear the stories of people like me was transformative. It allowed me to envision a future where I could embrace my identity, free from the constraints of societal expectations and norms. Social media wasn’t just a platform; it was a lifeline, a space where I could explore who I was without fear of judgment.

This is why I firmly believe that social media is essential for sharing stories like Laverne Cox’s and others to empower the trans youth and ‘set the agenda differently’. Growing up in Uruguay, I had no trans role models or peers. Even now, as an adult, I’ve only met a few from back home. The internet and the online world filled that void, offering me information, advice, and a sense of emotional refuge that helped me navigate the challenges of my teenage years. Transgender individuals are statistically more likely to face mental health struggles and have a lower life expectancy than their cisgender counterparts. For me, these realities hit painfully close to home. At 18 and 19, I attempted to end my own life twice. I truly believed there was no physical place for me to to transition, and social media showed me what life I could live in the future, it gave me hope by showing me other people’s stories that were going or went through the same thing as me.

This is not meant to be a sad story but rather a reflection on growth and self-discovery. As I grew older, I realized that leaving my home country was essential for me to fully explore and embrace my gender. My teenage years in Uruguay often highlighted the challenges of expressing myself authentically.  A few years ago, I attended a party wearing makeup and a crop top, a small but significant step in affirming my identity. That night, I was hate-crimed by a group of five straight cisgender men my age. Their violence was a stark reminder of the risks associated with being visibly different in a society that struggles to accept diversity. Even earlier, in high school, when I began growing my hair longer—a small act of rebellion and self-expression—a male classmate cut off a piece of it with scissors. My hair held immense significance to me; it was the one part of my body that felt feminine and aligned with who I truly was. These experiences, while painful, fueled my determination to seek a life where I could live authentically and safely. In high school, a friend whom I had known for more than ten years threatened to out me and tell everyone I was gay because he found my Twitter (now X) filled with RuPaul’s Drag Race posts. There, I could explore my identity more openly than in regular society. 

As I encountered the stories of other trans women online—each unique, neither overtly happier nor sadder than mine—I began to dream of moving abroad. I longed for a more open and respectful society where I could live authentically, free from the confines of a conservative, Hispanic, Catholic culture. That dream brought me to New York City, and these past few months have been a journey of self-discovery, since I find people here to be more open than back home to trans people. This sense of belonging, having trans friends, was something I had only previously glimpsed through online interactions—chatting with trans people, watching videos, and engaging with trans communities. Finding out more about what it was to be trans, opened my eyes to possibilities I hadn’t known existed in my youth. It revealed a community and a space for people like me, one often obscured and stigmatized by society as merely a ‘mental health problem’. This erasure of trans existence reinforces why visibility and representation matter so deeply. Online platforms introduced me to a world I didn’t know I could inhabit—a world where being trans is not a problem to be fixed but a life to be celebrated. 

Regarding Social Media 

Oliver Haimson

The foundation of this paper is deeply informed by the works of Oliver Haimson, a researcher who examines social media through the lens of "Intersectional Trans-Feminist Futures in HCI" (Human Computer Interaction). Haimson’s perspectives shed light on how social media platforms function as essential tools for social transition, providing unique spaces where transgender individuals can explore, express, and affirm their identities. His paper "Social Media as Social Transition Machinery" plays a pivotal role in this paper, illustrating the transformative power of digital platforms in enabling identity exploration and fostering community connections. Additionally, Haimson’s advocacy for "trans-competent interaction design" emphasizes the importance of creating digital environments that are not only inclusive but also attuned to the specific needs and challenges faced by transgender users. These frameworks collectively underscore the argument of this paper, emphasizing how social media platforms can and should be designed to empower marginalized communities, particularly transgender individuals, in their journey toward self-actualization and social acceptance.

In “Social Media as Social Transition Machinery”, Oliver L. Haimson expands Van Gennep’s liminality framework stages: Separation, Transition, to Incorporation. Haimson uses Gender Transition as a case study to analyze how people experience life transitions, and how trans people start by separating from their old selves, transitioning, and later reincorporating into society with a new identity (Haimson, Oliver L., 2018). 

Haimson argues that “identity is multiple, fragmented, and complex,” challenging the notion that individuals can be confined to a singular, static identity or a single social media platform that assumes a lifelong, unchanging network. Instead, he posits that different social media sites collectively operate as components of a larger “social transition machinery,” working together to facilitate significant life transitions. Drawing on Van Gennep’s liminality framework, Haimson explores how these transitions unfold for transgender users in digital spaces, while critically examining the conventional understanding of the “transition” stage. He questions the characterization of this stage as “identity-less,” emphasizing that even during times of flux, users actively construct and express their identities in meaningful ways. This perspective not only broadens our understanding of identity formation in online spaces but also highlights the integral role of diverse social media platforms in supporting complex and dynamic identity journeys. (Haimson, Oliver L., 2018). The author argues that social media is a rite of passage for transitioning, but adds to the literature by challenging “sex reassignment surgery as the primary rite of passage”, and argues that “online identity reconstruction is the modern pivotal rite of passage”. Examples like newlywed couples, and mothers, sharing their life transitions online for a brief and intense period and after incorporation, the usage decreases. Social media as social transition machinery is defined by the author as a tool that users use to present multiple identities, for a trans person who they are on Facebook (at the time) is different than who they are on Tumblr. Social media can provide an escape to social networks, and presenting multiple identities at once is not dishonest, but rather part of the life transition process. (Haimson, Oliver L., 2018)

“Social Media as Social Transition Machinery” examines how technology designers should adopt a deeper understanding of their users and their unique transition processes, akin to the relationship between health professionals and their patients. Haimson presents four main arguments to support his findings: first, social media enables users to embrace and express multiple identities simultaneously; second, users maintain connections with their networks even during significant life transitions; third, social media platforms themselves function as critical tools for facilitating social transitions; and finally, they provide a means for individuals in transition to reconstruct their online identities as part of a symbolic rite of passage (Haimson, Oliver L., 2018).  

Haimson’s work is central to this paper because it offers a transformative perspective on how social media shapes identity, particularly for transgender users. Haimson demonstrates that digital platforms are tools of empowerment, enabling individuals to navigate complex life transitions with agency and self-expression. I aim to reinforce the argument that social media when designed with trans competence and inclusivity, serves as critical infrastructure for marginalized communities not as a manipulative force, but as a mechanism for liberation, healing, and self-actualization.

Tumblr as a case study

“Tumblr was a trans technology” talks about the diverse policies implemented throughout Tumblr’s lifetime through the looking glass of Trans bloggers Haimson and others explore the changes in community standards of Tumblr and how in the early years, adult nudity was allowed, which was deemed “educational or medical in gender transition contexts”, but later on, Tumblr was purchased and introduced a policy that banned adult nudity. “Tumblr allowed trans users the changeability, network separation, and identity realness, along with the queer aspects of multiplicity, fluidity, and ambiguity, needed for gender transition. Haimson argues a trans technology enables trans experiences in these ways but must go beyond that. It also must uphold policies and an economic model that embraces adult or erotic content—an integral part of the transition and intersectional community building for many trans bloggers—without characterizing it as pornographic and removing it” (Haimson, Oliver L., Dame-Griff, Capello, Richter., 2021).

There are a series of themes that the authors explore and how these create a safe space or a trans technology. “Temporality, Openess, Change, Separation, Realness, Erotics and Intersectionality”. The authors discuss “temporality” which refers to the historical and social context in which trans users have existed on Tumblr and other social media platforms. The authors emphasize that while platforms like Tumblr have hosted vibrant trans communities, the corporate profit motive often undermines their ability to provide sustained support. For example, content moderation policies driven by advertising goals can result in the shadowbanning or outright removal of content related to the trans experience. Haimson highlights that advertisers often demand access to “ideal demographics,” leading to the exclusion of content that does not align with their narrowly defined target audiences. While I argue that social media companies may also capitalize on divisive content to radicalize certain groups—such as far-right users—as part of a profit-driven strategy, Haimson focuses on the structural limitations imposed by ad revenue models (Haimson et al., 2021).   (Haimson, Oliver L., Dame-Griff, Capello, Richter., 2021).

“Openness” is another key theme, encompassing the platform’s ability to create a safe and comfortable environment where users can share personal stories, express emotions, and seek understanding. One interviewee described their transition blog as “my safe space,” a sentiment that resonates deeply with me. Growing up, I longed for such a space, but I only joined Tumblr after its 2017 policy changes, which had already begun to erode the openness that earlier users had experienced. This openness allowed trans individuals to explore their identities, share their journeys, and find solidarity in ways that were often unavailable offline (Haimson, Oliver L., Dame-Griff, Capello, Richter., 2021). 

“Change” is a theme tied to the transformative experiences of trans users, both in their physical appearances and personal lives, as documented on their transition blogs. These blogs served as dynamic records of their journeys, showcasing the fluidity and evolution of their identities over time.  “Separation” refers to the distinction between the online communities trans users built on Tumblr and their offline social networks. This separation was particularly important for individuals who faced stigma or rejection in their everyday lives, allowing them to connect with supportive communities without fear of judgment or discrimination. “Realness” captures the ability of trans users to present new or evolving identities online, which often became integral parts of their lived realities. The anonymity afforded by Tumblr further enhanced this realness by providing users with the flexibility to experiment with their identities without immediate real-world consequences (Haimson et al., 2021).  

The final themes, “intersectionality and erotics”, are particularly significant in understanding the broader implications of Tumblr’s policy changes. The authors argue that the platform’s decision to ban adult content, including material related to gender reassignment surgery, was not only a blow to individual users but also to the broader trans community’s ability to produce and share knowledge. This decision disproportionately affected marginalized groups within the trans community, particularly trans people of color, who often face compounded barriers to visibility and support. The authors contend that erotic content, far from being gratuitous, was a powerful tool for community-building and self-expression. By sharing intimate aspects of their transitions, trans users reclaimed agency over their bodies and narratives, fostering a sense of empowerment and solidarity. The removal of such content, however, not only marginalized these users further but also perpetuated harmful stereotypes about trans people and their communities (Haimson et al., 2021). 

Tumblr’s evolution from a haven for trans users to a platform with restrictive policies illustrates the broader challenges faced by social media companies in balancing community needs with profit-driven objectives. For trans users, platforms like Tumblr represent more than just digital spaces—they are lifelines, providing the tools and environments necessary for identity exploration, self-expression, and community.

By choosing this case study, I aim to highlight the critical role of social media in supporting marginalized communities. Tumblr’s early policies and the subsequent backlash against its restrictive changes demonstrate the need for platforms to adopt inclusive designs that empower their users. As a trans person, I believe that understanding and amplifying these stories is essential to advocating for better policies and ensuring that digital spaces remain safe and affirming for all.

Statistical Analysis on Mental Health published on the JAMA network

As a data-driven person, pursuing a Master of Science in Data Analytics and Visualizations, I wanted to explore academic research in the statistics field, to find if there was a correlation between social media use and transgender individuals. This study also goes into other fields, analyzing the behavior of cis people online and overall focuses on studying mental health in their respondents (Coyne, Sarah M., et al., 2023).

An analysis of Social Media Usage (referred to as SMU) published on the JAMA Open Network studies the variance of different variables across 1200 young US residents through a self-reported method. The motivation behind their study is that “Mental health among children and adolescents is a critical public health issue, and transgender and gender nonbinary youths are at an even greater risk” and “currently, 25% to 32% of TGNB youth attempt suicide”. This study argues social media plays a role in providing transgender and nonbinary youth a safe space to explore their identities online (Coyne, Sarah M., et al., 2023).

This analysis tests the relationship between SMU, identifying as TGNB (transgender and non-binary), and depression levels. They found that “depression and conduct problems were lower for TGNB youths when they reported regularly cleaning or curating their social media feed, but both depression and conduct disorders were higher for cisgender youths when they engaged in this same activity” (Coyne, Sarah M., et al., 2023). 

This study resonates deeply with my personal experience of using social media as a trans individual. By curating my social media feed to align with my evolving identity and interests, I found a safe space where I could explore different parts of myself without judgment or external pressures. This process was not merely a passive consumption of content but an active and empowering exercise in self-expression and self-affirmation. Social media is a powerful tool for fostering resilience, connection, and self-discovery when used intentionally. These findings. strengthen the case for designing inclusive social media policies that cater to the unique needs of TGNB users while addressing the mental health challenges faced by young people across all identities.

Comparing Some Different Social Media Policies



Community standards are key to how community members behave and use social media. A study points out that “more research is also needed on how community standards evolve” and this analysis I have conducted will probably already be outdated and some of these extracts may have changed. (Bateman, Jon, Natalie Thompson, and Victoria Smith., 2021). I argue that a good indicator of how social media companies make their platforms online spaces and in the case of trans users may be finding information about gender-reaffirming surgery, which Oliver Haimson points out in “Tumblr was a trans technology”. But also adult nudity overall, and studying specifically what has been written about Meta’s ‘Real Name Policy’ are important parts of how social media community standards influence operations. These companies all have for-profit models, and inherently, their users well being is not the priority, since the algorithm itself feeds off the addiction some people have to use social media excessively because of their mental health. 

We can analyze this table both ways, by company or by row, which means analyzing what they say concerning adult nudity or gender confirmation surgery. If we look at companies; Tumblr, Meta, and Titkok remove content with genitals, but Tumblr allows for mature content to be labeled. However, X allows adult nudity. 

Tumblr has a very short policy, and they have changed their policy that Haimson references and explicitly states that they remove content with genitalia, without giving examples, this reflects that they default genitalia content as pornography or just nudity when it could be medical information.

Meta is known for having a ‘Real Name Policy’ which I will discuss later in this paper. They remove adult nudity and genitalia, except in “a medical or health context (...) such as gender confirmation surgery”. They refer to nudity as a form of protest, to raise awareness, and for education or medical reasons. It is a notable policy, and I found it to be restrictive but at least comprehensive. 

TikTok is another example of not allowing adult content on their policy. They also forget to express that gender confirmation surgery can be information for medical reasons.  They do not allow any adult nudity on their site, and even avoid showing restricted content in the algorithm of the “For You Page”. This means anyone could report a trans person’s account, and while the appeal is ongoing, their content would not get any views. 

X defines adult nudity content as “material depicting adult nudity or sexual behavior that is pornographic or intended to cause sexual arousal. This also applies to AI-generated, photographic, or animated content such as cartoons, hentai, or anime. Examples include depictions of: full or partial nudity, including close-ups of genitals, buttocks, or breasts; explicit or implied sexual behavior or simulated acts such as sexual intercourse and other sexual acts.”

Finally, X differs in policy, they do not remove content with genitalia and users may share adult nudity. The company also places importance on consent and individual production and distribution, while associating sexual expression with artistic expression. A negative aspect could be the omission that gender confirmation surgery is not distributed as pornography to cause arousal, and they are two very different types of content. Making sure that is included in the policy could benefit trans users on the platform from hate speech and trolling. 

If we read horizontally, some recommendations and highlights are pointed out. In regards to adult content, there are two sides, one prohibits it and one allows it. The other two mainly prohibit it but allow medical or labeled posts to stay up. If adult nudity is not allowed, gender-confirmation surgery images as information probably are not going to be allowed. However, X allows it and Meta names gender reassignment surgery as medical content, and they allow content of that type. 

Labeling content seems to have worked for Tumblr’s case because users cannot see labeled content if they do not want to, but also as seen in Haimson’s research with Tumblr bloggers, they benefit from labels and tags to reach people who are queer, accepting and open. Meta states they allow medical content if labeled correctly, but the appeals are a complicated process, sometimes requiring to provide a Legal ID which might not be the same name on the user’s page, because of their ‘Real Name Policy”. I examined their data on appeals, and in 2023, 2 million posts were not restored after an appeal on Facebook and 100K on Instagram. The chances of getting a post back up again are 60% on Facebook and 90% on Instagram through an appeal, that has discourse online on how fair it is to trans users.

Another aspect I think is relevant to highlight is the mention of gender reassignment surgery in the company's policy. I believe either allowing this content (X) or not (Meta sometimes) is better than not mentioning this term as medical information (TikTok). Transparency is always going to benefit the users of the platform because they have to be able to know what is allowed or not explicitly to not get their accounts suspended. 

Meta and their Legal or Real Name policy

Mark Zuckerberg said “[h]aving two identities for yourself is an example of lack of integrity.”, in “What’s in a name? Facebook’s Real Name Policy and User Privacy” Shun-Ling Chen, argues that this policy is dangerous because of the amount of data the user is giving with their legal name (gender, religion, generation, ethnicity, or country of origin). Moreover, she argues that Facebook [now Meta] is not a Social Media, but rather an “Identity Service” with a business model that the main goal is collecting as much data from users’ behavior. Chen quotes Zuckerberg saying that he admitted to Congress that data collection is the center of their business model (Chen, Shung-Ling., 2018).

Aside from the issues regarding data privacy this policy creates, Chen points out the “context collapse” users may not be able to separate social contexts, finding it awkward to communicate on the platform, while also not being able to “explore different personas” and possibly causing “ a chilling effect and hindering free speech”, while simultaneously “exposing marginalized communities to harassment or danger”. Another interesting aspect of the consequences of this policy is what happens to Native Americans because their names do not fit Western frames, drag queens getting their accounts suspended because their stage name is not a real name, or even abuse victims trying to protect themselves getting accounts deleted because of this Real Name Policy (Chen, Shung-Ling., 2018). It is also the only social media evaluated in this paper to have its users provide their legal name.

Chen explains that they caveat this policy by saying that real names foreclose bad behavior and associate anonymity with trolling. She states that anonymity is not the same as pseudonyms and that a real community can be built under a fake name. Her result or conclusion is that “Zuckerberg repeatedly emphasizes that users have control of their data, including how much of their data Facebook collects for targeted advertising” but “users do not have such control if Facebook continues to insist on its real name policy because our names contain a lot of information about us” (Chen, Shung-Ling., 2018). 

Haimson co-wrote with Hoffman about this policy in “Constructing and enforcing "authentic" identity online: Facebook, real names, and non-normative identities”. Chen, Haimson, and Hoffman reference The Zuckerberg Files to argue against this policy, which contains “a digital archive of all publicly available utterances of Zuckerberg regarding Facebook from 2004 to 2014, compiled and maintained by Michael Zimmer (2013)” Haimson argues in “Social Media as Social Transition Machinery” that identity is multiple, while Zuckerberg believes this represents a lack of integrity.  (Haimson, Oliver L., and Anna L. Hoffman, 2016) (Haimson, Oliver L., 2018). 

Aside from the arguments these two research projects have against the policy, there is a statistical analysis by Oliver Haimson, regarding content moderation for three groups of individuals, conservatives, trans folk, and black people. “Disproportionate Removals and Differing Content Moderation Experiences for Conservative, Transgender, and Black Social Media Users: Marginalization and Moderation Gray Areas” is a research project that found that “Facebook often removes trans accounts as violating its “real name” policy, which simultaneously enforces and prevents online authenticity for trans users” (Haimson, Oliver L., Daniel Delmonaco, Peipei Nie, and Andrea Wegner., 2021). 

Positionality Statement and Anti-Trans Dangerous Right Wing Rhetoric

To disclose my position on this subject, I am a trans person, and I think social media has to empower trans users and provide them with a space to explore identities, find information, build community, and find a safe place. 

There has been a constant anti-trans movement throughout our history, but now more than ever it lives online, and there is the regular hate speech and trolling. Still, there is a growing academic content that argues that big tech is turning kids trans and that social media is being run by an evil group in California with an agenda (Eckert, Jared, and Mary McCloskey., 2022). From their point of view, I am the perfect case, since I first learned what trans was online, and these researchers would argue that YouTube was the main influence in my “turning” trans, but they miss a huge point, why did trans feel adequate for me? Why did all these people’s experiences that date back years and years feel common, and felt like me?

“Digital spaces are ever more designed to promote sexual and transgender content.” (Eckert, Jared, and Mary McCloskey., 2022). This is just not true. The authors use misinformation with no sources behind it, just commentary, to radicalize the reader, and make them feel that social media companies are promoting pornographic material to kids. As we have seen with social media policies, most of them ban adult nudity, except if labeled, or has a valid medical reason. 

Eckert and McCloskey claim that X is banning users who argue that trans activism is grooming. They state there is a “woke design of social spaces”, and this a clear case of a misinformation campaign that only perpetuates harmful stereotypes erases trans history, and exposes trans people to harm and danger online and offline. Because even if trans creators were trying to take advantage of minors, the sharing of information and content regarding gender reassignment surgery and trans knowledge, is being compared to a case of sexual abuse, for being perceived as an attempt to establish an emotional connection with a vulnerable person. However this may apply, the user sharing the information does not get a direct benefit, rather than just building community. These far right-wing researchers are portraying trans creators as cult leaders who get benefits from “converting” minors trans (Eckert, Jared, and Mary McCloskey., 2022). 

As I write, the United States is embroiled in a heated debate over gender-affirming care. It’s crucial to address the harmful rhetoric that perpetuates misinformation, such as the baseless claim that Eckert and McCloskey make. President Donald Trump has added fuel to this discourse, stating the false claim, “Can you imagine you’re a parent and your son leaves the house and you say, ‘Jimmy, I love you so much, go have a good day in school,’ and your son comes back with a brutal operation? Can you even imagine this? What the hell is wrong with our country?” (Brandon, Alex., 2024). 

This rhetoric reflects the ongoing battle between two opposing perspectives: one believes in a conspiracy that executives are forcing children into transitioning against their will, while the other seeks to empower transgender youth by providing them the support and space to grow into healthy, self-actualized adults. I stand firmly with the latter. 

My own story is a testament to the importance of such spaces, both online and offline, in enabling transgender individuals to thrive. There is not a gender ideology online to “turn kids trans”, we finally have somewhere to resonate and explore with different identities. Social media does not make kids trans, there have been trans people throughout history, across cultures and our experiences are not a product of online activity and gender ideology, but rather authentic self-discovery, social media companies provide this anonymous, safe space for trans users that may feel misaligned with social gender norms.  

Recommendations for current social media sites

To my knowledge and my lived experiences, it is important to protect trans youth, since they are the weakest group to fall into mental health issues. There is power in sharing trans stories and giving them a platform, and visibility. It impacts the whole trans community, and in this paper, I argue how social media is the perfect place to explore different identities online. Haimson also supports this; “digital spaces can be important places for identity exploration without some of the barriers present in the physical world” (Haimson, Oliver L., 2018). 

Oliver L. Haimson’s research contributes other recommendations. Mainly centered on “trans competent interaction design”, he reaffirms the power building a community has, and that social media platforms should opt for a non-profit model or a “cooperative approach” (Haimson, Oliver L., Dame-Griff, Capello, Richter., 2021). “Tumblr was a trans technology” explores a set of values that describe how to create a trans technology, with the first goal being empowering trans users. He characterizes Tumblr as a trans technology because of “Temporality, Openness, Change, Separation, Realness, Erotics and Intersectionality” (Haimson, Oliver L., Dame-Griff, Capello, Richter., 2021). The overall argument of his research is that trans people need a place to explore a “flexibility in identity” sometimes, because their social context is not fit for them.

Moreover, in his research with others regarding content removals for trans users, they give four recommendations; tagging or labeling content, applying different content moderation approaches instead of just one, using specialized tools for marginalized groups, and involving communities affected in creating moderation policy (Haimson, Oliver L., Delmonaco, Nie, Wegner., 2021).

Haimson also is interested in Meta’s Real name policy, which is a prime example of how social media policies can harm marginalized communities like trans people. He found that Facebook (at that time) was suspending trans users’ accounts because they breached the ‘Real Name Policy’, and also argued that identity is multiple, which the CEO of Meta Mark Zuckerberg has disagreed, with and believes is “dishonest” (Haimson, Oliver L., Anna Lauren Hoffman., 2016). Shung-Ling Chen, another researcher interested in the ‘Real Name Policy’, issues a very strong statement that “Anonymity is quite different from pseudonymity”, which also aligns with what Haimson believes could improve social media companies, that anonymity is key to exploring different identities and creating that separation between online life and social context (Chen, Shung-Ling., 2018).

In regards to the analysis of social media policies, I found that it is better to allow gender reassignment surgery content on the platforms and classify this content as medical information, not pornography. However, there is a possibility of introducing an industry-wide standard of labeling content, to personalize algorithms of our own social media feeds, but also protect others who are not interested in seeing these posts. There is also another point, that Haimson calls companies to act on, and that is visibility and transparency, which I found that not all of them mention the words ‘gender reassignment or confirmation surgery’ in their policies. This could benefit trans users from online hate speech but also make room for them on the platforms. 

In regards to Meta, they have an extensive policy that did not allow gender confirmation surgery content but did name it, there is some mystery regarding the appeals some of the content creators on that platform face. They assure that this content may remain on their site if it is correctly labeled, but there is discourse online of people not being able to navigate through appeals regarding the legal name policy. This policy specifically is an example of what not to do as a social media company. There is an issue in believing that identity is constant and not multiple, but also there is a data privacy issue with giving that kind of personal or legal information. 

To conclude, it is relevant to acknowledge the growing far right-wing rhetoric on trans youth. Transgender people have existed throughout history and are not conditioned to behave a certain way by social media companies, we exist from lived experiences and authentic personal discoveries. This rhetoric is dangerous because of the use of misinformation campaigns to convince the public of a ‘gender ideology’, to further marginalize trans people and expose them to harmful and dangerous situations online and in real life. 

Bibliography 

Bateman, Jon, Natalie Thompson, and Victoria Smith. “How Social Media Platforms’ Community Standards Address Influence Operations.” Carnegie Endowment for International Peace, April 1, 2021. https://carnegieendowment.org/research/2021/04/how-social-media-platforms-community-standards-address-influence-operations?lang=en.

Billingsley, Amy. “Technology and Narratives of Continuity in Transgender Experiences.” Feminist Philosophy Quarterly1, no. 1 (July 22, 2015). https://doi.org/10.5206/fpq/2015.1.6.

Brandon, Alex. “Trump Repeats False Claims That Children Are Undergoing Transgender Surgery during the School Day.” NBC News, September 9, 2024. https://www.nbcnews.com/nbc-out/out-politics-and-policy/trump-false-claims-schools-transgender-surgeries-rcna170217.

Cavalcante, Andre. “Tumbling Into Queer Utopias and Vortexes: Experiences of LGBTQ Social Media Users on Tumblr.” Journal of Homosexuality 66, no. 12 (October 15, 2019): 1715–35. https://doi.org/10.1080/00918369.2018.1511131.

Chen, Shun-Ling. “What’s in a Name - Facebook’s Real Name Policy and User Privacy.” SSRN Electronic Journal, 2018. https://doi.org/10.2139/ssrn.3332188.

Coyne, Sarah M., Emily Weinstein, J. Andan Sheppard, Spencer James, Megan Gale, Megan Van Alfen, Nora Ririe, et al. “Analysis of Social Media Use, Mental Health, and Gender Identity Among US Youths.” JAMA Network Open 6, no. 7 (July 24, 2023): e2324389. https://doi.org/10.1001/jamanetworkopen.2023.24389.

Eckert, Jared, and Mary McCloskey. “How Big Tech Turns Kids Trans.” The Heritage Foundation, September 15, 2022. https://www.heritage.org/gender/commentary/how-big-tech-turns-kids-trans.

Gray, Mary L. Out in the Country: Youth, Media, and Queer Visibility in Rural America. NYU Press, 2009.

Haimson, Oliver L., and Anna Lauren Hoffmann. “Constructing and Enforcing ‘Authentic’ Identity Online: Facebook, Real Names, and Non-Normative Identities.” First Monday, June 10, 2016. https://doi.org/10.5210/fm.v21i6.6791.

Haimson, Oliver. “Social Media as Social Transition Machinery.” Proceedings of the ACM on Human-Computer Interaction 2, no. CSCW (November 2018): 1–21. https://doi.org/10.1145/3274332.

Haimson, Oliver L., Daniel Delmonaco, Peipei Nie, and Andrea Wegner. “Disproportionate Removals and Differing Content Moderation Experiences for Conservative, Transgender, and Black Social Media Users: Marginalization and Moderation Gray Areas.” Proceedings of the ACM on Human-Computer Interaction 5, no. CSCW2 (October 13, 2021): 1–35. https://doi.org/10.1145/3479610.

Haimson, Oliver L., Avery Dame-Griff, Elias Capello, and Zahari Richter. “Tumblr Was a Trans Technology: The Meaning, Importance, History, and Future of Trans Technologies.” Feminist Media Studies 21, no. 3 (April 3, 2021): 345–61. https://doi.org/10.1080/14680777.2019.1678505.

Steinmetz, Katy. “TIME Cover Story: Interview With Trans Icon Laverne Cox.” TIME, May 29, 2014. https://time.com/132769/transgender-orange-is-the-new-black-laverne-cox-interview/.

Williams, Thomas James Vaughan, Calli Tzani, Helen Gavin, and Maria Ioannou. “Policy vs Reality: Comparing the Policies of Social Media Sites and Users’ Experiences, in the Context of Exposure to Extremist Content.” Behavioral Sciences of Terrorism and Political Aggression 0, no. 0 (April 2023): 1–18. https://doi.org/10.1080/19434472.2023.2195466.


