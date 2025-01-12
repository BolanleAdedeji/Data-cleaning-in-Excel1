# Health Care Analysis

## Table of Content 
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Errors Inside](#errors-inside)
- [Cleaning Steps](#cleaning-steps)
- [Tools Used](#tools-used)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Result](#result)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Project Overview 

Welcome to my Excel Data, where I tackle messy datasets head-on! This project showcases my expertise in transforming raw, inconsistent, and error-prone data into a clean, structured, and ready-for-analysis format.

Whether you're a recruiter looking for a detail-oriented data analyst or a data enthusiast eager to explore the power of Excel, this repository is for you!

### Data Source
Green Data Solution

### Errors Inside
Raw Data: Real-world messy datasets filled with challenges like:

- Missing values

- Inconsistent formatting

- Duplicate entries

- Erroneous data points

### Cleaning Steps 
Step-by-step documentation of cleaning techniques, including:
- Remove duplicate data to maintain a clear dataset, reduce the chances of inconsistency in analysis, remove the chances of having incorrect conclusions.
- Trim the name column to remove unnecessary spaces before, in between and after names
- Edit the name to have proper casing, this ensures the data are uniform, reduces the chance of errors in analysis, enhances data matching, and improves searchability and readability of data.
- Unknown was found in the age column, this was identified and replaced by the mean age which is 33, mean age was achieved by calculating the average, and was replaced using 'find and replace'.
- On the gender column had inconsistencies with how male and female were written, by using "find and replace", all male were replaced with "M" and all females were replaced with "F", empty cells were identified, some of the cells were replaced with either "F" Female where Mrs. was seen and "M" Male where Mr was seen, this was identified using the filter, the remaining empty cells were replaced with "Uknown" using IF(ISBLANK).
- the city colum was edited to maintain consistency in the city name, using the filter, find, and repace.
- on the Blood group column, empty cells were replaced with "Unavailable" using IF(ISBLANK).
- Education Column was edited using If(ISBLANK) to replace all empty cells with "Unknown"
- The salary column had anomalies which needed, a lot of cleaning, the "$" and "-" signs were removes using "find and replace", the "missing" cells were replaced with "0", using "IF", the colum was tested using =ISNUMBER to test if all are numerical, which returned a lot of cells as FALSE, then using "filter,find and replace" the non-numeric content were removed.
- Blank cells in health condition column was replaced with "Unavailable". using "filter, find and replace".
- Credit Score was cleaned using "filter, find and replace".
-  Date column was was cleaned by spliting the date into different column, day of the week, date, month and year, the date and month mixed together was cleaned using filter, and manually switched, then the columns were combined using =date funtion.
-  Data was imported into Power Query to check to edit change, Add column from example, Split column into day, month and year and convert to date format.
-  visualization was done using Excel Pivot table and Charts



### Tools Used
#### - Microsoft Excel:
- Advanced functions,
- conditional formatting, Pivot table 
- data validation.


#### Why This Challenge Matters
Cleaning data is the cornerstone of data analytics—it’s where messy data turns into gold! 
This challenge demonstrates my ability to: Clean different types of column with different dataset format in a scolumn especially date column, it stretches mean to learn and research different methods of cleaning data. At the end of the challenge I was able to showcase my ability to 

- Identify and resolve data quality issues.
- Apply Excel’s full potential for data cleaning and transformation.
- Deliver clean, actionable datasets for decision-making.
- Use pivot table to summarize data
- Use Excel for Dashboard

Let’s dive into the art and science of data cleaning together!

### Exploratory Data Analysis

- Identify cities and  demographics with higher healthcare needs based on health conditions and admission dates.
  

### Result 
- I was able to identify that among 1656 patients admitted accross the cities , Atlanta city has 973 of them making the city highest with poor health condition.
- Blood type B+ and O+ blood type are needed more.
- A+,B+,O+ blood type is prevalent among the patients with poor health condition.
- Other gender has the poorest health condition when compared with male and female.
- Patients with Excellent health condition has high credit score.
- Unemployed patients ranked high in poor health


### Recommendations
_ Healthcare provision should be more in Atlanta city, becuase they have both poorest health condition and are employed with good credit score.
- More health care services should be provided to the other gender to improve their health status.
- A+,B+,O+ blood type should be sourced and supplied more to the blood bank accross the cities with Atlanta city getting more supply
- Unemployment needs to be addressed to reduce the number of unemployed with poor health condition
### Limitations 
- The data did not provide information on the type of health conditions treated to be able to profer specific solution to gender and employment statu.
- Other gender need to be further breakdown to understand the gender type facing poor health condition
- Unable to sort the gender of some of the patients that fall under others due to unavailable prefix.



