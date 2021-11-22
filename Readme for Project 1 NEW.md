Readme document for Project

Business Understanding:

This project (Write a Data Science Blog Post) is part of Udacity Data Scientists Nanodegree Program.

In this project, I have used the Dataset of -average-salaries-by-education-in-saudi-arabia. This enables us to 
find certain interesting facts about the salary difference , salary increase etc in Saudi Arabia 

The following questions are selected by me to analyse this dataset.

1. How much is the salary increase berween 2017 and 2021 , for different type of education?
2. What is the salary difference for Male and Female employees during 2017-2021 ?
3. what is the percentage of salary for Saudis compared to Non Saudis ?

Data Understanding:

The following is the first 10 rows of the data we will analyse .

Degree Level	Nationality	Gender	Year	Quarter	Salary	Currency
0	Primary	NonSaudi	Female	2017	Q1	1590	SAR
1	Primary	NonSaudi	Male	2017	Q1	2173	SAR
2	Primary	Saudi	Female	2017	Q1	4172	SAR
3	Primary	Saudi	Male	2017	Q1	6172	SAR
4	Primary	NonSaudi	Female	2017	Q2	1597	SAR
5	Primary	NonSaudi	Male	2017	Q2	2213	SAR
6	Primary	Saudi	Female	2017	Q2	3875	SAR
7	Primary	Saudi	Male	2017	Q2	5957	SAR
8	Primary	NonSaudi	Female	2017	Q3	1596	SAR
9	Primary	NonSaudi	Male	2017	Q3	2250	SAR

This is the count, mean , std etc of the Data.

	Year	Salary
count	504.000000	504.000000
mean	2018.777778	8950.031746
std	1.315991	6372.635277
min	2017.000000	1331.000000
25%	2018.000000	4194.000000
50%	2019.000000	7890.500000
75%	2020.000000	12448.750000
max	2021.000000	35622.000000

Data Preparaion :

1. #Data Preparation 

we will prepare the data to be used later for the full analysis. we will find and correct the missing values in the dataset. 

This function shows the total number missing values of all columns

df.isna().sum()

Degree Level    0
Nationality     0
Gender          0
Year            0
Quarter         0
Salary          0
Currency        0
dtype: int64

This function drops all the records which have null values

df = df.dropna()

This function gives total the duplicate data

print(df.duplicated().sum()) 

Libraries used : PANDAS , MATPLOTLIB

Motivation for this Project: I went through some datasets and this one was suiting my requirement of analysis of the Salary of KSA .I found this as more useful and valuable for the review of the experts and for the Job seekers. 

Analysis and Conclusion:


After the analysis with three questions, I could find out that;

-- we can see there is an overall slight decrease of about 0.65 % in the salary annually for different degree levels .
   except Masters , Doctorate where the increase is about 5.5 % appx
-- we can observe that the Salary was always higher by 29% to 36% for Male Employees when compared to Female Employees.

-- we can see that the salary range for the Saudis is always more than that of Non-Saudis.

This Dataset is available for review at : https://www.kaggle.com/majedalhulayel/average-salaries-by-education-in-saudi-arabia.

I have used to Python , using Jupyter Notebook to write the code for the Visuals using third party modules Pandas and Matplotlib. 

Acknowledgement: Kaggle.com 






