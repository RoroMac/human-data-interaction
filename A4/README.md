# A4: Final Project
The final project for HCDE410 investigating the impact that collegiate sports have on their universities. This repo is protected under the MIT license.

I merged the NCAA college football dataset with the college scorecard dataset to determine the impact that the college football coach has on college admission. I randomly sampled 60 universities at different years and annotated these datasets with the head coach football salary at the given time. In determining if there was any relationship I ran two pearson coefficient functions between admission rates and win rates and admission rates and coach salary. Both suggest that to no significant degree that coach salary and football winnings has on a university prestige and suggests the Flutie effect to be false.


# A7 Final Project.ipynb
This file is the primary research report. It includes methods for data cleaning, producing the data visualization, and running an analysis comparing admissions, salary, and college football win rates. It produces all datasets used in the clean data and datavisualizations folder.

# Project Proposal
A text file describing motivations of this project. There are no outputs or dependencies.

# Raw Data
Includes the datasets used in the analysis coming from the college scorecard and the NCAA college football dataset.

# College Scorecard
A federal database for reporting publicly available data from public institutions. Private universities do not have to report and therefore information provided by them may be missing. The scorecard dataset does not have a license but assumed as public domain. Variables of interest include


|Variable|	Description|
|-|-|
|Institution Name |	Used to join college scorecard data to football dataset
|Admission Rate |	Admission rate of the given year, used to calculate change in admission rates between two years|
|Control	|Determine a public institution|
|UGDS|	Size of an undergraduate student population|
|HIGHDEG	|The highest degree provided at the instititution|

# NCAA College Football Dataset
A dataset from the NCAA college football but provided under an open data license. This is used to track win ratios of certain institutions to later determine correlation with school admission rate. Variables of interest include

| Variable | Description |
| - |-|
| Team Name | Name of the college team |
| Number of Games played	 | Number of games played for the given year |
| Number of Games Won	 | Number of games wno for the given year |