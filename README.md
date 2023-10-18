# Business-Inquiry-to-Research-Solution

This data science exercise is focused on assisting a hypothetical agency partner in discovering and describing patterns related to the uptake of a benefit for small businesses eligible for federal aid. The overarching goal is to explore the potential for a future randomized trial. Two primary datasets serve as the foundation for this analysis. One comprises the email addresses of business owners with self-reported details about their operations, while the other offers unique insights based on the ZIP codes of these businesses. Although all business owners were informed of their eligibility, not all chose to apply. The analysis seeks to understand the types of businesses that applied and those that refrained, thereby offering actionable insights for the agency partners.

## Data Source
The data sets we received from our partners are named `business_data.csv` and `zip_data.csv`. The first contains a number of variables at the business-level:
  - `applied`: a binary indicator for whether a small business owner applied for aid;
  - `FTE`: number of full-time equivalent employees;
  - `MOB`: indicator for whether the business is minority-owned;
  - `WOB`: indicator for whether the business is woman-owned;
  - `FY19`: reported revenue in the 2019 fiscal year;
  - `FY20`: reported revenue in the 2020 fiscal year;
  - `email`: the email address of the business owner;
  - `zip_id`: the ZIP code of the business.

The latter contains info at the ZIP code level:
 - `zipCode`: the ZIP codes in the county of interest;
 - `size`: the population within the zip code;
 - `status`: the urban/rural status of the zip code.

## Libraries Used
The analysis utilizes the following R libraries and packages:
- `dplyr`: Used for data manipulation with verbs like filter, mutate, and join.
- `ggplot2`: A versatile library for creating rich visualizations using a consistent grammar.
- `tidyr`: Provides functions for reshaping and tidying data structures.
- `corrplot`: Visualizes correlation matrices with various aesthetics.
- `stargazer`: Generates well-formatted regression tables for LaTeX and ASCII outputs.
- `rpart`: Constructs classification and regression trees for predictive modeling.
- `rpart.plot`: Offers enhanced visualizations for trees created using rpart.
- `caret`: A comprehensive toolkit for training and evaluating machine learning models.
- `pwr`:  Conducts power analysis and determines required sample sizes for statistical tests.

## Analysis
The main objective of the analysis is to discover and describe patterns in the uptake of a benefit. Analysis steps include:
- Data Wrangling
- Hypothesis testing
- Logistic regression
- Decision Trees
- Increasing Application Rates
- Sample Power Analysis

## Key Achievements
1. **Statistical Rigor**: Successfully employed hypothesis testing techniques like chi-squared and Fisher's exact test to discern application rate differences among business groups.
2. **Modeling Proficiency**: Utilized logistic regression to model the probability of application based on several predictor variables, offering a comprehensive understanding of the influencing factors.
3. **Attention to Detail**: Addressed potential pitfalls in logistic regression modeling, such as multicollinearity, ensuring robustness in the findings.

## Conclusion
The combination of hypothesis testing and logistic regression has provided a multifaceted understanding of the application behaviors among businesses. The analysis has shed light on specific groups with distinct application tendencies, as well as the combined influence of various business attributes on the likelihood to apply.

## Future Work
1. **Model Enhancement**: Incorporate more advanced machine learning techniques to enhance predictive accuracy.
2. **Feature Exploration**: Explore additional potential predictor variables and assess their significance in influencing application behaviors.
3. **Qualitative Insights**: Augment the quantitative findings with qualitative research to understand the underlying reasons behind the observed patterns.

## Author
Jesus Cantu Jr.

## Last Updated 
April 14, 2023
