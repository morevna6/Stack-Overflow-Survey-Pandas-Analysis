# Stack Overflow Developer Survey Analysis

## Project Overview

This project analyzes the 2025 Stack Overflow Developer Survey dataset using Python and Pandas.

The goal of the analysis is to explore developer demographics, work experience, remote work patterns, Python usage, learning methods, compensation trends, education levels, age groups, and industry distributions.

The project was completed as part of a Pandas data analysis assignment.

## Dataset

The dataset used in this project is the Stack Overflow Developer Survey dataset.

File used:

- `results.csv`

The dataset contains survey responses from developers and includes information such as age, education level, employment status, work experience, programming languages, learning methods, remote work status, yearly compensation, country, and industry.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook

## Analysis Questions

The notebook answers the following questions:

1. How many people participated in the survey?
2. How many participants answered all questions?
3. What are the central tendency measures for work experience?
4. How many people work remotely?
5. What percentage of participants program with Python?
6. How many people learned programming through online courses?
7. Among participants who program with Python, what are the mean and median yearly compensation values by country?
8. What are the education levels of the top 5 participants with the highest compensation?

## Bonus Analysis

The project also includes two bonus analyses:

1. What percentage of participants program with Python in each age group?
2. What are the most common industries among remote workers in the top 25% yearly compensation group?

## Key Findings

- The survey contains 49,191 responses.
- No participant answered every single column without missing values, mainly because the dataset contains many optional questions.
- The average work experience is approximately 13.37 years.
- The median work experience is 10 years.
- 10,931 respondents are fully remote workers.
- 18,466 respondents have worked with Python.
- Python usage among participants is approximately 37.54%.
- 10,973 respondents learned programming through online courses or certification.
- Software Development is the most common industry among remote workers in the top 25% compensation group.

## Notes

For remote work analysis, only respondents whose `RemoteWork` value is exactly `Remote` were counted as fully remote workers. Hybrid work categories were shown separately but not included in the final remote worker count.

For complete responses, `dropna()` was used across all columns. Since the dataset has many optional columns, the number of fully complete responses is 0.

For compensation analysis, missing yearly compensation values were ignored during aggregation.

## Project Structure

```text
stackoverflow-developer-survey-analysis/
│
├── results.csv
├── stackoverflow_developer_survey_analysis.ipynb
└── README.md
