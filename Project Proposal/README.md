# **Salary Trends in Data Science: A Comprehensive Analysis of Compensation Factors**
---
## Background & Question
---
### Research Question and Motivation

**Research Question:**  
How do key factors such as experience level, job title, company size, remote work ratio, and geographic location affect salaries in the data science field?

**Motivation:**
- As the data science field continues to expand, understanding the variables influencing salary decisions is crucial.
- Both employers and job seekers need insights into salary trends to make informed decisions.
- This project aims to uncover patterns in compensation, addressing the growing demand for salary benchmarks that account for factors beyond just experience level and job title.

**Need / Niche:**
- Existing salary analyses often overlook key variables such as:
  - Remote work policies  
  - Company size  
  - Geographic location  
- This analysis will fill the niche by providing a deeper understanding of how these factors interact to influence salaries, which is important in today’s hybrid and global work environment.

**Why It’s Worth Exploring:**
- Given the rise in remote work and shifts in the data science job market, understanding the nuances of salary expectations is crucial.
- This analysis can:
  - Help professionals better negotiate compensation packages  
  - Help employers design competitive offers that attract top talent  
  - Guide strategic decisions in recruitment and workforce planning  

**Novelty:**
- While salary analysis in tech is not a new field, this project is original in its approach to combine:
  - The effects of remote work  
  - Company size  
  - Geographic location  
- These factors are increasingly important but often overlooked in traditional studies.

---
## Hypothesis and Prediction

**Hypothesis:**  
Salaries in the data science field are significantly influenced by experience level, job title, company size, remote work ratio, and geographic location.

**Prediction:**
- Experience level and job title are expected to be the most significant predictors of salary, with senior roles earning significantly more than junior ones.
- Remote work ratio will be positively correlated with salary, as remote roles tend to offer more flexibility and higher compensation.
- Employees in large companies will earn higher salaries than those in smaller companies, as larger organizations generally offer more competitive pay packages.
- Geographic location will have a strong effect on salaries, with employees in tech hubs earning higher salaries than those in smaller cities or rural areas.

---

## Data & Analysis

### Dataset Overview

- **Dataset:** `data_science_salaries.csv`  
- **Description and Suitability:**  
  This dataset includes detailed information on data science salaries, job titles, experience levels, employment types, locations, and company sizes across various countries.  
  With almost 15,000 entries, it provides a robust foundation for analyzing role transitions and salary growth across different levels of experience and job types.  
  The data structure allows for segmentation by:
  - `experience_level`
  - `job_title`
  - `salary_in_usd`  
  making it well-suited for tracking career pathways and associated financial outcomes.

### Key Variables and Analysis Plan

#### Key Variables

| Variable Type       | Variables                                                                 |
|---------------------|---------------------------------------------------------------------------|
| Independent         | `job_title`, `experience_level`, `company_size`, `company_location`       |
| Dependent           | `salary_in_usd`                                                           |

#### Analysis Plan

1. **Data Preprocessing and Cleaning**
   - Handle missing values and duplicates.
   - Convert categorical variables (e.g., experience level, job title, company size) into numerical format using techniques like one-hot encoding.
   - Ensure that salary values are standardized in USD for consistency.

2. **Exploratory Data Analysis (EDA)**
   - Use summary statistics (mean, median, standard deviation) to understand the distribution of salaries.
   - Visualize the data using boxplots and histograms to examine salary distributions by:
     - Experience level  
     - Job title  
     - Company size  
     - Remote work ratio  
   - Analyze correlations between salary and other variables (e.g., remote_ratio vs. salary).

3. **Statistical Analysis**
   - Perform ANOVA or t-tests to compare salary differences across different categories (e.g., experience level, job title).
   - Conduct regression analysis to evaluate the relationship between salary and the independent variables.

4. **Predictive Modeling**
   - Build a multiple linear regression model to predict salary based on the independent variables.
   - Evaluate performance using R-Squared and RMSE.

5. **Validation and Insights**
   - Validate the model by comparing predicted salaries against actual salary values.
   - Interpret the coefficients of the model to understand the impact of each variable on salary.
   - Provide insights into how different factors contribute to salary disparities in the data science field.

---

## Success Indicators

- The question will be considered answered if I can quantify the effects of experience level, job title, remote work, company size, and geographic location on salary.
- The hypothesis will be supported if statistical tests show significant differences in salaries based on these factors.
- The regression model will validate the impact of each variable on salary, and model performance metrics (R-squared, RMSE) will confirm the accuracy of predictions.
- Insights into salary trends across different regions, job roles, and companies will provide actionable recommendations for both job seekers and employers.

---
## Technical Details
### Data Wrangling:
- Clean the dataset by handling missing data and duplicates.
- Standardize salary values to USD for consistency.
- Encode categorical variables (e.g., job title, company size) using one-hot encoding.

### Exploratory Data Analysis (EDA):
- Visualize salary distribution across experience levels, job titles, and company sizes.
- Analyze correlations between variables using heatmaps and scatter plots.
- Check for outliers and anomalies in salary data.

### Statistical Analysis:
- Perform ANOVA or t-tests to assess salary differences across categorical variables.
- Use correlation analysis to identify significant relationships between salary and other features.

### Predictive Modeling:
- Build a multiple linear regression model to predict salary based on the identified factors.
- Evaluate model performance using R-squared and RMSE.
- Experiment with other machine learning models (e.g., random forest, gradient boosting) to compare performance.

### Interpretation of Results:
- Extract the most significant predictors from the regression model.
- Validate model predictions by comparing them to actual salary values.
- Provide actionable insights based on the findings.

### Visualization:
- Create interactive visualizations or a dashboard to present key findings.
