# Mental Health Data Analysis Project

This project analyzes mental health survey data using SQL. The goal is to gain insights into mental health trends, factors affecting mental well-being, and how different demographics respond to mental health issues.

## Objectives

- Understand patterns in mental health data.
- Explore correlations between mental health conditions and factors such as age, gender, and employment.
- Analyze the accessibility and awareness of mental health resources.

## Dataset

The dataset used for this project contains survey responses on mental health issues, demographics, and workplace mental health support. It includes the following columns:

- **Age**: Respondent's age.
- **Gender**: Gender identity of the respondent.
- **Workplace Support**: Does the respondent's workplace provide mental health support?
- **Mental Health Condition**: Has the respondent ever been diagnosed with a mental health condition?
- **Seeking Treatment**: Is the respondent currently seeking treatment for mental health issues?
- **Awareness**: Awareness of mental health resources and options.

## SQL Queries

The project uses SQL to query the dataset and derive insights. Key SQL operations include:

- **Filtering Data**: Selecting subsets of data based on specific conditions (e.g., people with a diagnosed mental health condition).
- **Aggregation**: Calculating averages, sums, and counts to find patterns in the data.
- **Joins**: Combining tables to analyze relationships between different factors.
- **Group By**: Grouping data by demographic factors such as age or gender to find trends.
- **Order By**: Sorting results for easier interpretation of trends.

## Example SQL Queries

Here are a few example queries used in the project:

1. **Count of respondents by gender who have sought mental health treatment:**
   ```sql
   SELECT gender, COUNT(*) AS treatment_count
   FROM survey_data
   WHERE seeking_treatment = 'Yes'
   GROUP BY gender;
