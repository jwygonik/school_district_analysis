# school_district_analysis

# Overview
In the School District Analysis we compile the test scores and averages across the different schools and compare them alongside one another to try to gain insight on what factors may have a positive or negative impact on overall performance. 

# Results: 

Using bulleted lists and images of DataFrames as support, address the following questions.

	* How is the district summary affected? 
		- Although the difference is small, after replacing the tampered data from the Thomas High School 9th grade, we do see a small decrease across the 'Average Math Score' and 'Average Reading Score' categories as well as the passing percentages in the '% Passing Math', '% Passing Reading', and '% Overall Passing'. 

		### Original District Summary
		(school_district_analysis/original_district_summary.png)
		### Adjusted District Summary 
		(school_district_analysis/adjusted_district_summary.png)
	* How is the school summary affected?
		- We saw a slight decrease across the Average Scores and Passing Percentages, but none of these differences exceeded a tenth of a score or percent. 

	* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s 	performance relative to the other schools? 
		- Although there was a decrease in peformance accross categories, it was not significant enough to change Thomas High School's ranking when compared with other the other schools. They remained ranked number two even with the adjustments for the 9th grade. 

	* How does replacing the ninth-grade scores affect the following:
		* Math and reading scores by grade 
			- We cleaned out the bad Thomas High School 9th grade data by replacing the dishonest Math and Reading scores with a NaN for each student. When we generated summaries of Reading Score by grade and Math Score by Grade, the average score for both in the 9th grade column was replaced by NaN and we were unable to accurately compare their performace to the other schools. 
		* Scores by school spending
			- The only spending group that was effected by this change was the range Thomas High School fell into. The $631-645 spending range differed by a few small decimal points. However, when we reformatted the data and rounded the values, the differences were not reflected in the average score categories or the percentage categories. 
		* Scores by school size
			- Similar to the spending groups, the only school size category that was effected by the change was the Medium category where Thomas High School was. There were very slight differences in the decimals of the average scores and percentage data, but once we reformatted the DataFrame, the results matched the previous summary. 
		* Scores by school type
			- Just as the above summaries, The District School summary had slight differences because Thomas High School fell into that category. And once again, after reformatting the data, there was no visible difference between the two DataFrames. 
#Summary: 
Filtering out the inaccurate scores for one of the High Schools did have some small effects on the data, but overall we were able to maintain the integrity of the accurate data we did have. Changing the 9th graders scores to NaN did prevent us from getting the full picture of Thomas High School's performance across grade levels but it was a small sacrifice to maintain the accuracy of the rest of the analysis. Although we saw small variations in reading score and math score averages, when we got to the final stages of cleaning the data, these were not reflected in the final product. The passing percentages were also maintained in the final data summaries due to the formatting choices of the client. Had we not rounded the numbers up, the differences in the scores and percentages are visible, but miniscule. None of the adjustments were really enough to effect the outcome and ranking of Thomas High School when comparing it to the other schools. 