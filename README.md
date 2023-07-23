# Analysis of the Indian Startup Ecosystem
## Introduction
This project is an analysis of the Indian Startup Ecosystem. The purpose is to dig deeper into the how startups are funded in India. Based on our findings, management can make informed decisions on the best approach of entry.  
## Hypothesis
### Null Hypothesis
H_o: The location of a business does not affect the amount of funding received from investors.
### Alternate Hypothesis
H_a: The location of a business affects the amount of funding received by investors.
### Research Questions
# Research Questions

1) To what extent do cities influence funding?

2) Which industries are preferred by investors for funding?

3) At which stage do start-ups get more funding from investors?

4) What is the typical funding amount that startups receive in India?

5) Which type of investors invest the most money?
## Data 
This study uses secondary data from 2018 to 2021. These were extracted from three sources:
2020 and 2021 dataset were extracted remotely from a microsoft server database.
2019 dataset was obtained from OneDrive and the third dataset (2018) were obtained from a given Github repository. 
All the dataset were in a csv file format which had the following columns;
1) Company/Brand: Name of the company/start-up.
2) Founded: Year start-up was founded.
3) Sector: Sector of company.
4) What_it_does: Description about Company.
5) Founders: Founders of the Company
6) Investor: Investors
7) Amount($): Raised fund
8) Stage: Round of funding reached
### Tools and Framework used
Python and python functions (Pandas, Numpy etc), Kanban Board, and the CRISP-DM Framework.
## Steps
The project followed the CRISP-DM framework.
1) Business understanding
2) Data understanding
3) Data preparation
4) Modeling
5) Evaluation
6) Deployment
### Business, Data Understanding, and Data Preparation
Using Python IDE, Jupyter Notebook, the following packages were installed and subsequently imported.
• Pandas
• Numpy
• Matplotlib
• Seaborn
• Squarify
The Dataset was loaded into the Jupyter Notebook for analysis using a pandas.read_csv since all the dataset were csv files. As a member of a four-member team, the team agreed that each member works (Business understanding, data understanding, and data preparation) on one year dataset. Working on the 2020 dataset, I loaded the csv file and began studying this dataset to understand the requirements for this project. 
To gain further insight on the dataset, the following codes were used
.head() - to have a quick overview of first five(5) rows
.info() - to see the columns, the null values, and the data types present in the dataset
.column() - to see the names columns
.shape() - to see the dimension of the dataframe
After gaining an overview of the dirt and incosistencies in the data, a number of activities were undertaken to clean up the dataset. This is important to be able to gain meaningful information after analysis. 
The following activities were undertaken to clean up the 2020 dataset
1) rename columns for consistency in all datasets
2) fill in missing data columnwise. The median was used in cases skewed integer or float data type columns. Mode was used in object data types.
3) a column was dropped since it contained only two data
4) other columns like stage and founders were imputed with 'Unknown' since imputing with mode or dropping them would affect our analysis. 
After all team member have finished cleaning their respective dataset, they are merged into one dataframe. This is further cleaned because the 2018 dataset lacked 3 columns which automatically became null after concatenation. After this last cleaning, our combined dataset on the Indian Startup Ecosystem is ready to be analyzed to answer our research questions and Hypothesis. 
### Visualization on research questions
#### Question 1: To what extent do cities influence funding?
![Question1](https://github.com/sethsot/Analysis-of-the-Indian-Startup-Ecosystem/assets/137343449/1f2ebc6b-33f5-407a-8c31-286dbe4b0aca)

#### Question 2:  Which industries are preferred by investors for funding?

![Question2](https://github.com/sethsot/Analysis-of-the-Indian-Startup-Ecosystem/assets/137343449/e2f90013-aa43-4d1f-9525-4e959ef891eb)

#### Question 3: At which stage do start-ups get more funding from investors?

![Question3](https://github.com/sethsot/Analysis-of-the-Indian-Startup-Ecosystem/assets/137343449/e7b40e20-c94c-4a19-85ec-a8eb4785c2e3)
#### Question 4:  What is the typical funding amount that startups receive in India?
![Question4](https://github.com/sethsot/Analysis-of-the-Indian-Startup-Ecosystem/assets/137343449/31d34232-4071-42df-9f39-1863b48deaea)

#### Question 5): Which type of investors invest the most money
![Question5](https://github.com/sethsot/Analysis-of-the-Indian-Startup-Ecosystem/assets/137343449/a28b98f4-f334-4c55-a336-87dd09add32d)

## Conclusion
Based on our Hypothesis testing and analysis, we Reject the null hypothesis since p_value is less than our significance level (0.05)
Therefore, we conclude that 
## The sector of a start-up affects the amount of funding received’ was rejected as there is no relationship between the two.
