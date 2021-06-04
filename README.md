# Kickstarter-analysis
Performing analysis on Kickstarter data to uncover trend

## Overview of Project

### Purpose
 The purpose of the project is to use the acquired Excel knowledge to visualize campaign outcomes based on their launch dates and their funding goals using the Kickstarter dataset. By the end of the project, we will have a visual representation of "outcomes based on goals" and "theater outcomes based on launch date". This project will also include the limitation(s) to the dataset, the challenges and/or difficulties encountered and how I came them. 
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
I created the "year" column to extract the year from the "Date Created Conversion" column using this formula =YEAR(@S:S) and applied the result to the rest of the column. (column S is "Date Created Conversion"). After this, I created a new sheet named "theater outcomes by launch date", inserted a pivot table, filtered the pivot table based on "parent category" and years, placed "outcomes" in the column label and values, "date created conversion" in the row label and finally, created a line with markers chart to visualize the relationship between outcomes and launch month.
![2](https://user-images.githubusercontent.com/76136277/120840916-d78b4080-c538-11eb-8c2d-1c30e52a9d34.PNG)

### Analysis of Outcomes Based on Goals
After creating the required rows and columns for this project, and typing in the range in the goal column, I used the COUNTIFS function to pull out data from the Kickstarter dataset to complete the "number successful", "number failed" and "number canceled" columns. I used the Sum() function to add up each row to get the total projects. I calculated the percentages by dividing the number of project by total project and multiply by 100. For example, calculating the percentage successful for Column B2 would be =(B2/E2)*100 and applied to the rest of the column. I used the same formular to calculate the percentage failed and canceled. Lastly, created a pivot table and chart from the data.
### Challenges and Difficulties Encountered
The only challenge/difficulty I encountered was in the "Outcomes based on Goals" deliverable. Firstly, the row label of the pivot table was not in the right order, even though the sheet I created the pivot table from was in the right order. This made the line chart a bit different from the one provided in Canvas. I used the 'filter" to sort the column, but didn't work. I was able to resolve this problem after searching on google for other methods with this link - (https://support.microsoft.com/en-us/office/design-the-layout-and-format-of-a-pivottable-a9600265-95bf-4900-868e-641133c05a80#:~:text=Change%20the%20order%20of%20row%20or%20column%20items,menu%20to%20move%20the%20item%20to%20another%20location). I had a similar challenge with "outcome based on launch date" pivot table as well.
![1](https://user-images.githubusercontent.com/76136277/120840825-b62a5480-c538-11eb-8852-9786963726b0.PNG)

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - Kickstarters campaigns in the "theatre" category is the most prevalent category and reached its peak in May.
  - January, March, September, November and December had roughly the same number of failed campaigns launched in the "theater" category. 
- What can you conclude about the Outcomes based on Goals?
  - There is 67% success rate and 33% failure rate within goals that ranges from 30000 to 39999.
  - Goals that ranges between 45000 to 49999 had 100% failure.
- What are some limitations of this dataset?
  - The dataset does not have much information on what the donors will get in exchange for their donations. This can impact the donor's decision to donate if they believe they would receive something in return for their donation.
  - Some countries have higher chances of succeeding in a particular category than the others which influences the outcome. For example, countries like US, GB, AU etc. will have a higher success rate than Hongkong in the theater/musical category. 
- What are some other possible tables and/or graphs that we could create?
   - "Outcomes based on Pledges"
   - "US Photography outcomes by launch date"
   - "Outcomes by Country"
   - Graphs that break up each category into its subcategories. 
