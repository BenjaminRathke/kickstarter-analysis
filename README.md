# Kickstarting with Excel

## Overview of Project
This project utilizes Microsoft Excel tools to evaluate the success or failure of Kickstarter campaigns for Louise's play "Fever". Specifically, the project analyzes data correlation in a large data set between goal amounts and outcomes (i.e. success or failure), and launch dates and outcomes.

## Analysis and Challenges
In order to perform the analysis, a pivot table and line graph were created to visually represent and more easily compare the correlations.  

### Outcomes vs. Months
A pivot table was created in order to easily arrange data and filter to appropriate years and categories for launch months and outcomes. For the purposes of this project, categories were filtered to "theater," "all" years, and display data for all months. By doing so, we might easily and quickly view the potential correlations between success (or the lackthereof) and campaign start months.
#### Outcomes vs. Months Pivot Table
![Outcomes Based on Month Pivot Table](resources/Outcomes_Launch_Pivot.PNG)

### Outcomes vs. Goals
A standard table utilizing the COUNTIFS function was used to filter the appropriate data, and easily create a line graph to illustrate success or failure based on goal amounts and outcomes.  By doing so, we might easily and quickly view the potential correlations between success (or the lackthereof) and goal amounts.
#### Example "COUNTIFS" Formula:  
=COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<=4999",Kickstarter!$R:$R,"plays")
#### Outcomes vs. Goals Table
![Outcomes Based on Goals Table](resources/Outcomes_Goals_Table.PNG)

### Challenges
Few challenges were encountered.  One notable exception was in the copying of cell formulae in the percentage columns to other columns for the Outcomes Based on Goals table.  the "$" operator was inappropriately used to reference the denominator, thus locking the referenced cell inappropriately for all percentage values.  Removing and re-replicating the formula fixed the problem immediately.

Possible other issues that could (but did not) occur include accidentally changing data values in the original data set, accidentally referencing wrong cells or columns in the data, a 0% cancelled result for all monetary ranges in the Outcomes vs. Goals table may have caused confusion and caution, but a quick verification of the results upheld the 0% results.

### Analysis of Outcomes Based on Launch Date
![Outcomes vs. Launch](resources/Theater_Outcomes_vs_Launch.png)
The number of successful and failed campaigns are highest in the month of May.  Successful campaigns decrease steadily throughout the year and failed campaigns stay relatively constant. 

### Analysis of Outcomes Based on Goals
![Outcomes vs. Launch]()

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
