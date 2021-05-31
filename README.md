# PyBer_Analysis
5 Matplotlib, Scipy, Pandas and Nympy.

## PyBer Analysis Overview
Omar and I have been asked by V. Isualize to use Python and Pandas, to create summary data based on the PyBer input .csv ride sharing tables that
were provided. The end output should be created using Pandas and Matplotlib to create a multiple-line graph that shows the total weekly fares
foreach city type: Urban, Suburban and Rural. This report should provide required summary output.

## PyBer Analysis Results:
There were 5 key metrics being calculated in doing the PyBer ridershare analysis.  Below are the details uncovered for each metric as shown in attached shot of the dataframe created with reesult of analysis:
![PyBer_Analysis](./Pyber_summary_df.png)
### Total Rides per City Type - This metric, shows that as you go from Urban to Suburban to Rural, the number of rides decreases.  This would be expected, partly due to the population of those areas; Less people = less required rides.

### Total Drivers per City Type  - Similar to rides per city type, this metric as you go from Urban to Suburban to Rural, the number of drivers decreases.  This would be expected, again partly due to the population of those areas.

### Total Fares per City Type  - Total fares would be impacted by the above two factors, Total Rides per City Type and Total Drivers.

### Average Fare per ride per City Type - this metric indicates that as the area of driving increases, so does the fare.  Therefore, you would expect the average fare to be higher as the distances of the rides becomes further.

### Average Fare per Driver per City Type - same as above metric, Average Fare per Ride, this metric would increase as the distances increase as you go from Urban all the way to Rural.

## PyBer Analysis Summary
If we look at the metrics in the above output and the below data graph,
![PyBer_Analysis](.//TotalFaresbyCityType.png)

*School District Analysis Summary
If we look at the differnce between the Original Spending Summary dataframe and the Challenge Spending Summary dataframe (attached below), we can see there were 5 changes to the school distict analysis in the category that Thomas High School was grouped into due to their school's spending range of $630 to $644.  The other ranges would not have been affected by the changes to Thomas High School, as as expected, there are not changes in the other ranges.

### For the range of $630 to $644 that Thomas school was in we see the following changes BEFORE we format the dataframe:
- Average Math Score went from the original output of 78.518855 to the challenge output of 78.502002. This would be due to the decrease in math scores at Thomas High School once the corrupt data was removed and calculation adjusted.
- Average Reading Score went up for this range from original of 81.624473 to challenge percentage of 81.636261. Again, this would be expected given the results of reading increased slightly when 9th graders were removed.
- % Passing Math went down from 73.484209 to 73.462589, this is impacted by the internal change at Thomas High School for this metric.
- % Passing Reading 84.391793 84.319261 this is impacted by the internal change at Thomas High School for this metric as even though the Average Reading Score went up, % passing would not necessarily have the same increase.
- % Overall Passing - this metric changed from 62.857656 on the original to  62.778233 on the challenge with updated numbers includes.  We would expect this to reflect the changes in % Passing Math and % Passing Reading, and we do see a decrease similar in that to the sum of those figures.
				
![School_District_Analysis](./original_spending_summary_df.png)
![School_District_Analysis](./challenge_spending_summary_df.png)

### For the range of $630 to $644 that Thomas school was in we see the following changes AFTER we format the date:
All of the above differences no longer have any detectable impact after rounding, as shown in the two illustrations: 
![School_District_Analysis](./original_spending_summary_fmt.png)
![School_District_Analysis](./challenge_spending_summary_fmt.png)

### Similarly, for the School Size metrics, we see a difference prior to formatting, but after rounding to 1 decimal place, the data is the same.
![School_District_Analysis](./original_size_summary.png)
![School_District_Analysis](./challenge_size_summary.png)

### Finally, for the district summary analysis, we also see there were no changes as the rounding of the calculations in the formatting process removes any detectable differences as shown in the provided illustrations.
![School_District_Analysis](./original_type_summary.png)
![School_District_Analysis](./challenge_type_summary.png)




## Resources
- Data Source: schools_complete.csv 
	       students_complete.csv
- Software: 4 Panda, Jupyter and Python


# Challenge Overview
Was difficult to understand the .loc function at first, but once I had that figured out most of the rest was easy to re-purpose my code from assignment.
