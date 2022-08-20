# Kickstarter
Outcomes Based On Goals

##Goals

The goal of this analyis was to analyze and sort data from the Kickstarter worksheet to find what percentages failed, succeeded and cancelled based on numerical amounts in order. Specifically, in the subcategory of plays. 

##Application

To begin this process we begin by using the COUNTIFS funtion to filter by dollar amount, failed/cancelled/succeeded and filtered with the subcategory plays. The code I used to do this is as follows =COUNTIFS(Kickstarter!$D:$D, "<=1000",Kickstarter!F:F, "successful",Kickstarter!R:R,"plays")

The next process for this analysis was done by using the SUM function to total all 3 columns (failed/cancelled/succeeded). To do this I used the following code: =SUM(B2,C2,D2)

Finally we pull the percentages by dividing the column with the specific category divided by the total amount of projects and change the outcome to percentages under the General Tab. An example of this which was used for cell F2 is =B2/E2.

##Challenges

When beginning this project I ran into a few issues learning how to apply code in the correct format. My first issue I encountered was attempting to list the code as >1000 OR <=5000. After running into errors I learned to then seperate the code as Kickstarter!$D:$D,>1000,Kickstarter!$D$D,<=5000. The second issue I encountered was forgetting to also filter in the subcategory "plays". I corrected this by adding the line Kickstarter!R:R, "plays" to the end of the code. 

##Overview

When looking at the graphs for the sheet "Theater Outcomes by Launch Date" we can draw the following conclusions. The most successful period of time occurred between the months of April and May. The least successful period of time between September and October. 
When examining "Outcomes Based on Goals" the most successful category of success appeared in the less than 1000 range. 
