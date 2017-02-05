# machine_learning
Data analytics

# Analyze a Data Set
This Jupyter Notebook was based on a dataset found at:
https://archive.ics.uci.edu/ml/datasets/Housing

The data set concerns housing values in suburbs of Boston, and contains the following attributes.

## Attribute Information:

1. CRIM: per capita crime rate by town 
2. ZN: proportion of residential land zoned for lots over 25,000 sq.ft. 
3. INDUS: proportion of non-retail business acres per town 
4. CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise) 
5. NOX: nitric oxides concentration (parts per 10 million) 
6. RM: average number of rooms per dwelling 
7. AGE: proportion of owner-occupied units built prior to 1940 
8. DIS: weighted distances to five Boston employment centres 
9. RAD: index of accessibility to radial highways 
10. TAX: full-value property-tax rate per $10,000 
11. PTRATIO: pupil-teacher ratio by town 
12. B: 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town 
13. LSTAT: % lower status of the population 
14. MEDV: Median value of owner-occupied homes in $1000's

## Data Analytics

The analysis looks at: 
- The relationship between median housing values and the home age
- The correlation between crime rate and student/ teacher ratio at local schools
- The proportion of black citizens within a suburb and the distance from that suburb to employment centers
- The connection between home values, nitrus oxide contamination, and proximity to industrial centers
- The relationship between crime rate and proportion of non-retail businesses


# Working with Imperfect Data

This Jupyter Notebook was based on a dataset from the Seattle Police Department, outlining Incident Reports in the city of Seattle, as of January 28, 2017.

The dataset can be found here: https://data.seattle.gov/Public-Safety/Seattle-Police-Department-Police-Report-Incident/7ais-f98f

## Attribute Information:

1. CAD CDW ID
2. CAD Event Number
3. General Offense Number
4. Event Clearance Code
5. Event Clearance Description
6. Event Clearance SubGroup
7. Event Clearance Group
8. Event Clearance Date
9. Hundred Block Location
10. District/Sector
11. Zone/Beat
12. Census Tract
13. Longitude
14. Latitude
15. Incident Location
16. Initial Type Description
17. Initial Type Subgroup
18. Initial Type Group
19. At Scene Time

## Process

The data was originally displayed in rows of information separated by commas. The first row contained the column names, also separated by commas. To access this information, I created a Pandas dataframe that specified the comma as the delimiter, and the first row as the header row. I set low_memory to False, because the data set included a mix of data types. 

Because these column names consisted of multi-word strings, often with spaces between the words, I wound up renaming them as simple, shortened strings (ex: "DESC"). This made it easier to use these names to access information.