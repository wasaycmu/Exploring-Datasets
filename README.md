# Exploring-Datasets

# Dallas Animal Shelter Data Analysis

## Project Overview

The **Dallas Animal Shelter Data** reflects the operational processes carried out by shelter personnel assisting citizens with surrendered and stray animals. The shelter utilizes Chameleon software to document its operations, which are updated daily to improve citizens' understanding of shelter activities. The dataset spans from October 1, 2017, to the present, with the focus being on Q2, Q3, and Q4 of 2019, and Q1 of 2020.

### Business Understanding

This analysis aims to improve animal welfare and optimize shelter operations by answering the following questions:
- **Adoption Outcomes**: How do attributes like breed, species, timing, and location affect adoption outcomes?
- **Length of Stay**: What factors influence how long an animal stays at the shelter?
- **Trends in Incoming Animals**: Are there seasonal trends in animal intakes?

The insights gained could help in resource allocation, identifying at-risk animals, and improving shelter efficiency.

## Data Sources

The dataset was extracted from the **Dallas Animal Shelter** and includes information on animal types, breeds, intake conditions, and outcomes. The dataset is continuously updated to reflect the shelter's operations.

### Dataset Columns
- **Animal Type**: Type of animal (e.g., Dog, Cat)
- **Animal Breed**: Breed of the animal (e.g., Labrador, Siamese)
- **Council District**: The district number where the shelter is located
- **Intake Type**: How the animal was brought into the shelter (e.g., owner surrender, stray)
- **Intake Subtype**: Detailed type of intake (e.g., at large, confined)
- **Reason**: Reason the animal was brought in (e.g., diseased, financial burden)
- **Intake Date**: Date the animal was brought into the shelter
- **Outcome Type**: What happened to the animal (e.g., adopted, euthanized)
- **Outcome Date**: Date the animal's outcome was determined
- **Other relevant columns**: Include breed codes, reason codes, outcome codes, and various status fields.

## Objectives

The main objective of this analysis is to understand factors that influence animal outcomes in the shelter and to identify areas of improvement. The ultimate goal is to create a predictive model that could assist shelter personnel in making data-driven decisions to improve animal welfare.

## Data Cleaning and Preprocessing

The dataset underwent significant cleaning to remove irrelevant columns and handle missing values. The following columns were removed due to irrelevance to the analysis:
- **Tag Type**, **Activity Number**, **Source Id**, **Census Tract**, etc.

After cleaning, the dataset contains 13 relevant columns for analysis, including attributes such as **Animal Type**, **Animal Breed**, and **Outcome Type**.

## Exploratory Data Analysis (EDA)

### Descriptive Statistics
We started by generating descriptive statistics for the dataset to understand the distribution of key variables such as animal type, breed, intake type, and outcomes.

### Aggregated Analysis
The data was grouped by animal type, breed, and intake subtype to understand the distribution of animals across these categories.

### Visualization
Various visualizations were created to gain insights into animal outcomes and shelter operations:
- **Histogram of Outcome Times**: A histogram was plotted to visualize how long animals stayed at the shelter before receiving their final outcome. The distribution showed a quad-modal pattern, with peaks at day 0-2, day 5, day 10, and day 30, suggesting different types of shelter operations (e.g., euthanasia, adoption, medical care).



### Hypothesis Testing
We hypothesize that animals remaining in the shelter for longer periods (5, 10, 30 days) are typically those requiring medical treatment or waiting for adoption. Further analysis will be conducted to validate this hypothesis.


### Future Steps
 - Trend Analysis: We will compare the data from 2019-2020 with data from other years to understand the impact of the COVID-19 pandemic on animal shelter operations.

 - Predictive Modeling: We aim to build predictive models to forecast outcomes based on animal attributes, helping to optimize shelter operations and improve animal welfare.


### Conclusion
This analysis serves as a starting point for improving the operational efficiency of animal shelters. By understanding the factors influencing animal outcomes and the trends in incoming animals, the shelter can allocate resources more effectively, prioritize at-risk animals, and increase adoption rates.


### Technologies Used
 - Python (Pandas, NumPy, Matplotlib)

 - Jupyter Notebook for interactive data exploration and visualization
