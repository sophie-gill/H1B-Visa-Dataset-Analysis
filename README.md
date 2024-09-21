# H1B 2017 Data Analysis in RStudio

This project explores the H1B 2017 dataset using RStudio, providing insights into foreign worker employment in the U.S. under the H-1B visa. Through numerical, visual, and regression-based analyses, we aim to interpret relationships between key variables within the dataset.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Description](#data-description)
3. [Analysis](#analysis)
    - [Numerical Summary](#numerical-summary)
    - [Visual Summary](#visual-summary)
    - [Linear Regression](#linear-regression)
    - [Logistic Regression](#logistic-regression)
4. [Results](#results)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Conclusion](#conclusion)
8. [Technologies Used](#technologies-used)
9. [Contact](#contact)

## Introduction

The H-1B visa allows U.S. companies to employ foreign workers in specialty occupations. The 2017 dataset provides details about the employers, the visa petitions, and other related factors. This project examines the dataset to uncover trends and relationships, leveraging both statistical summaries and machine learning models such as linear and logistic regression.

## Data Description

The dataset includes variables such as:
- **Employer Name**: The company sponsoring the visa.
- **Job Title**: The position for which the worker is employed.
- **Wage**: The salary offered to the worker.
- **Case Status**: Approval or denial of the visa petition.
- **Work Location**: The state or city where the job is located.
  
These variables help us understand trends in employment, petition approval, and the characteristics of employers sponsoring foreign workers.

## Analysis

### 1. Data Preparation
- Missing data was handled through imputation where necessary.
- Variables were transformed as needed for modeling, including normalizing continuous variables for regression.

### 2. Numerical Summary
- Key statistics (mean, median, mode) were computed for variables such as wages and visa approval rates.
- Count and proportion data were used to evaluate the prevalence of H1B visa approval.

### 3. Visual Summary
- Visualizations include:
  - Histograms of wages to show salary distribution.
  - Bar charts displaying the frequency of visa approvals per job title.
  - Geographic maps illustrating the concentration of H1B visa workers across states.

### 4. Linear Regression
- A linear regression model was used to examine the relationship between wages and job titles, employers, and locations.
- Coefficients were interpreted to determine which factors influence wages the most.

### 5. Logistic Regression
- Logistic regression was used to model the probability of visa approval based on factors such as wage, job title, and location.
- Odds ratios were calculated to assess the impact of each variable on visa petition success.

### 6. Regression Diagnostics
- Diagnostic plots were used to check model assumptions such as homoscedasticity, linearity, and independence.
- The regression model’s performance was evaluated with R-squared values, residuals, and cross-validation.

## Results

- **Numerical Analysis**: Higher wages were correlated with visa approval, and certain job titles (e.g., software developers) had a much higher approval rate.
- **Visual Analysis**: There was a clear geographical concentration of H1B workers in states like California and Texas.
- **Regression Models**: The linear regression model showed that wages are significantly influenced by both the employer and the job location. Logistic regression indicated that wage and job title were strong predictors of visa approval.

## Installation

To run this analysis locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/h1b-analysis-rstudio.git
   cd h1b-analysis-rstudio
