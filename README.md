# Repository Overview
This Repository is a place to store our data files in order to work collaboratively on this project over FSB data.

# Project Overview
The Farmer School of Business conducts annual surveys to learn about student's job placement post-graduation. The data is mixed with most coming from self-reported student surveys and the other observations coming from the Miami University database. Our goal with the data is to understand the macro placement and salary trends for FSB students over the last three years in order to assist Kirk Bogard, the Associate Vice President for Development and External Relations in FSB. Specifically, we will:

* Create a a graph that shows the average salary per year, per major of Farmer graduates.
* Overlay a graph of the previous year's average salary per year, per major of Farmer graduates
* Compare these graphs with averages from other schools to show FSB’s success (if FSB performs better than the national average)

This will help by:

* Understanding of data that has been collected over the last 3 years in a structured way
* Having the average salary of each FSB major for past years
* Understanding of which majors tend to have higher salaries within the same company

## File Overview
1) Project-2.RMD: R-Markdown file that contains our data processing in order to generate clean data for analyses. It is the first file that needs to be run in this workflow.

2) Project-2.HTML: HTML file that displays our data processing in an easy to understand layout detailing which variables were kept/removed as well as how we cleaned the variables we kept. 

3) Student Success Dashboard.RMD: R-Markdown file that contains the code for generating our dashboard.

4) Student Success Dashboard.HTML: HTML file that displays our dashboard, the final deliverable, showing salary distribution by major in FSB over the previous 3 years, salary distribution of FSB as a whole, FSB major salaries compared to Kelley Business School and the Fisher School of Business majors, and the salary distribution for different majors within the same company. This is the main deliverable file and most important for gaining insights. The graphs are all intereactive with different options to zoom in, scroll within the graph, and even download the graphs as png. The data table in the Salaries by Top Company tab is for the top ten companies and can be filtered for different years, majors, salaries, and companies in the top ten companies in terms of hiring recent Miami graduates. The filtered dataset can be downloaded as a csv or excel file.

5) Copy of poster Value proposition canvas simple white.png: Our business value proposition in an image format that is included in the Project-2.RMD and HTML file.

## Main Data Source

You have three years of data representing FSB graduates, including graduates in 2019, 2020, and 2021. The dataset provided had 42 variables.  The source is either derived by me during data cleaning/merging, from the Oracle Business Intelligence Enterprise Edition (OBIEE) maintained by Miami adminsitration, or from the self reported senior survey.

1.  nmajor: numeric,derived, the number of majors 
2.  major1: text, OBIEE, first major
3.  major 2: text, OBIEE, second major
4.  BBRJ: binary, OBIEE, an attribute of a student, but we do not know what this stands for
5.  Business Direct Admit: binary, OBIEE, a direct admit to FSB as a first year
6.  Combined Cacc and Masters: binary, OBIEE, combined degree student
7.  Dean's List: binary, OBIEE, achieve dean's list status at least once
8.  First Generation College Stdnt: binary, OBIEE, first generation student status
9.  FSB Scholars: binary, OBIEE, FSB scholars program
10.  Honors Program: binary, OBIEE, member of University honors program
11.  President's list: binary, OBIEE, achieved president's list at least once
12.  Study Abroud Courtesy Account: binary, OBIEE, do not know meaning
13.  Transfer Work: binary, OBIEE, do not know exact meaning
14.  Cum Laude: binary, OBIEE, graduated Cum Laude
15.  Magna Cum Laude: binary, OBIEE, graduated Magna Cum Laude
16.  Summa Cum Laude: binary, OBIEE, graduated Summa Cum Laude
17.  University Honors: binary, OBIEE, graduated with University Honors
18.  University Honors w/Distinction: binary, OBIEE, graduated with University Honors with Distinction
19.  minor1: text, OBIEE, first listed minor
20.  minor2: text, OBIEE, second listed minor
21.  IPEDS.Race.Ethnicity: text, OBIEE, race/ethnicity
22.  Gender: text, OBIEE, sex
23.  GPA.Range: text, OBIEE, GPA within a .5 range
24.  Term.Code: numberic, OBIEE, First four digits are the physcal year (beginning in July, e.g. July 2020 is FY 2021).  Last two digits is the term (10=fall, 15=winter, 20=spring, 30=summer).
25.  Year.x: text, derived, first four digits of Term.Code stored as a character variable
26.  latin_honors: text, survey, latin honors designation
27.  survey_city: text, survey, student reported city in which their job is located
28.  survey_company: text, survey, student reported company in which they accepted a job
29.  survey_deptfunc: text, survey, student reported job function
30.  survey_gradprogram: text, survey, student reported graduate program they will be attending
31.  survey_gradschool: text, survey, stuent reported graduate school they will be attending
32.  survey_internfour: text, survey, student reported fourth internship they held during college
33.  survey_internthree: text, survey, student reported third internship they held during college
34.  survey_interntwo: text, survey, student reported second internship they held during college
35.  survey_internone: text, survey, student reported first internship they held during college
36.  Survey_internships: text, survey, Student reported number of internships they held during college
37.  survey_offers: text, survey, student reported number of offers for full time employment received
38.  survey_plans: text, survey, student reported plans after graduation
39.  survey_pref_field: text, survey, student reported whether working in preferred field
40.  survey_pref_loc: text, survey, student reported whether working in preferred location
41.  survey_salary: numeric, survey, student reported salary
42.  survey_state: text, survey, student reported state in which job is located

## Support Data Sources

Indiana University Salaries: https://kelley.iu.edu/recruiters-companies/undergrad/statistics/salary-statistics/index.html

Ohio State Salaries: https://files.fisher.osu.edu/careers-recruiting/public/2021-10/AnnualReport2021.pdf?VersionId=UnbXIIgZenGaz8EVfozFCS1lJrl9bf5A

CPI Inflation Calculator: 
https://www.officialdata.org/us/inflation/2022?endYear=2021&amount=60000
