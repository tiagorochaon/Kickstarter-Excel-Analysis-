# Kickstarting with Excel
## Overview of Project
Crowdfunding platforms like Kickstarter and Indiegogo have been growing in success and popularity since they began in the late aughts. Everyone from indie creators to famous celebrities have utilized crowdfunding to launch new products and generate buzz, but not every project has found success.

### Purpose
Getting funded on a crowdfunding website requires meeting or exceeding the project's initial goal, so many organizations spend months looking through past projects in an attempt to discover some trick for finding success. For this week's homework, you will organize and analyze a database of 1,000 generated sample projects in order to uncover any hidden trends.

## Analysis and Challenges
Using the Excel [workbook](CrowdfundingBook.xlsx) provided, modify and analyze the data of 1,000 example projects in an attempt to uncover market trends. 

* Dataset created by Trilogy Education Services, LLC.


* Use conditional formatting to fill each cell in the `outcome` column with a different color, depending on whether the associated campaign was successful, failed, canceled, or is currently live.

  * Create a new column called `Percent Funded` that uses a formula to uncover how much money a campaign made relative to its initial goal.

* Use conditional formatting to fill each cell in the `Percent Funded` column according to a three-color scale. The scale should start at 0 and be a dark shade of red, transitioning to green at 100, and blue at 200.

  * Create a new column called `Average Donation` that uses a formula to uncover how much each project backer paid on average.

  * Create two new columns, one called `Parent Category` and another called `Sub-Category`, that use formulas to split the `Category and Sub-Category` column into the two new, separate columns. 

  ![Category Stats](Images/CategoryStats.PNG)

  * Create a new sheet with a pivot table that will analyze your initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per **category**.

  * Create a stacked column pivot chart that can be filtered by country based on the table you have created.

  ![Subcategory Stats](Images/SubcategoryStats.PNG)

  * Create a new sheet with a pivot table that will analyze your initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per **sub-category**.

  * Create a stacked column pivot chart that can be filtered by country and parent-category based on the table you have created.

* The dates stored within the `deadline` and `launched_at` columns use Unix timestamps. Fortunately for us, [there is a formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) that can be used to convert these timestamps to a normal date.

  * Create a new column named `Date Created Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `launched_at` into Excel's date format.

  * Create a new column named `Date Ended Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `deadline` into Excel's date format.

  ![Outcomes Based on Launch Date](Images/LaunchDateOutcomes.PNG)

  * Create a new sheet with a pivot table with a column of `outcome`, rows of `Date Created Conversion`, values based on the count of `outcome`, and filters based on `parent category` and `Years`.

  * Now create a pivot chart line graph that visualizes this new table.

* Create a report in Microsoft Word and answer the following questions.

1. Given the provided data, what are three conclusions we can draw about crowdfunding campaigns?
2. What are some limitations of this dataset?
3. What are some other possible tables and/or graphs that we could create, and what additional value would they provide?

### Three conclusions we can draw about crowdfundind campaings?
•	19% of the donations exceeded 200% which means that the goal is not real
•	57% OF THE campaigns were successful.
•	1% of the campaigns are still live.

### Limitations of this dataset?
•	We had to create new columns like Goal Rangers to get the percentage of some campaigns. 

### Other possible tables and or graphs that we could create, and what additional value would they provide
•	We can create tables using dates to know if the campaigns were too long or not related with pledged.

