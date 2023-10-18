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
- **Data Wrangling**: Initial exploration and cleaning of datasets, including handling missing values, renaming columns, and merging datasets based on zip codes.
- **Identifying Application Rates**: Focus on understanding the types of businesses that applied and those that didn't.
- **Hypothesis Testing**: Categorical variables were analyzed to identify significant differences in application rates. Techniques like `chi-squared test` and `Fisher’s exact test` were employed.
- **Logistic Regression**: Regression models were built to predict application behavior based on variables like `Full-Time Equivalent (FTE)`, `Minority-Owned Business (MOB)`, and `Women-Owned Business (WOB)`. The influence of `rural/urban` status and business size was also explored.
- **Decision Trees**: Decision tree models were built to gain insights into factors affecting applications. Trees were visualized for interpretation.
- **Increasing Application Rates**: Strategies to increase application rates were explored, including the feasibility of sending mailers.
- **Sample Power Analysis**: Power analysis was conducted to determine the required sample size for potential randomized trials.

## Achievements & Outcomes
- **Statistical Insights**: Hypothesis testing, especially using chi-squared tests and Fisher’s exact tests, discerned application rate differences among business groups. Significant differences in application rates were identified among various business types and ownership categories, especially `Minority-Owned Business (MOB)` and `Women-Owned Business (WOB)`.
- **Predictive Modeling**: Logistic regression models highlighted key predictors such as `Full-Time Equivalent (FTE)`, `MOB` status, and `WOB` status. `Rural/urban` status and business size also emerged as influential factors in determining application behaviors.
- **Decision Trees Insights**: Through decision trees, `FTE`, `MOB`, and `WOB` were identified as primary factors that differentiate between businesses that applied and those that didn't. Additionally, rural/urban status and business size played pivotal roles in application patterns.
- **Strategic Approaches**: One of the strategies explored to increase application rates was the possibility of sending mailers to businesses, particularly targeting those identified as least likely to apply based on the analysis.
- **Foundation for Future Trials**: Power analysis determined the required sample size for potential randomized trials, ranging from a minimum of 20 to a maximum of 1203, depending on the desired effect size, significance level, and power.

## Conclusion
The comprehensive analysis provided a robust understanding of the dynamics influencing small businesses' decisions to apply for federal aid. Through various statistical methods, factors like the number of `FTE` employees, `MOB` status, `WOB` status, and business location emerged as pivotal. The exploration of mailer-based engagement strategies offers a potential approach to boost application rates. Additionally, power analysis lays a concrete foundation for assessing the feasibility of future randomized trials.

## Future Work
-  **Model Enhancement**: Incorporate more advanced machine learning techniques to enhance predictive accuracy.
-  **Feature Exploration**: Explore additional potential predictor variables and assess their significance in influencing application behaviors.
-  **Qualitative Insights**: Augment the quantitative findings with qualitative research to understand the underlying reasons behind the observed patterns.

# Note
To fully understand the conclusions drawn in this analysis, it is recommended to go through the entire R notebook, including the code and its outputs. You can view the HTML version of the notebook [here](http://htmlpreview.github.io/?https://raw.githubusercontent.com/JESUSC1/Business-Inquiry-to-Research-Solution/main/Business_Question_Data_Analytics.html).

## Author
Jesus Cantu Jr.

## Last Updated 
April 14, 2023
