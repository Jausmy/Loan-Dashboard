# Data Portfolio: Loan Risk Factors Dashboard

## Overview
This report presents a comprehensive analysis of loan approval trends and associated risks that may lead to an application getting declined. By examining historical loan application data, we aim to identify key trends in applicant demographics, financial profiles, and risk scores, and provide insights to optimize loan approval processes and mitigate the potential of defaulting.

## Executive Summary
By examining key metrics such as credit scores, annual income, net worth, debt-to-income ratios, and risk scores, we identified key trends and areas for potential improvement in the loan approval process. A key insight from the analysis is that approved applicants consistently exhibited higher credit scores, annual income, and net worth compared to declined applicants [(see Analysis of Applicant Profiles by Approval Status)](#Analysis-of-Applicant-Profiles-by-Approval-Status). Based on the analysis, we recommend focusing on refining risk assessment models by incorporating factors such as employment status, education level, and loan purpose to improve the accuracy of loan approval decisions and minimize potential financial losses. By implementing these recommendations, the financial institution can potentially reduce loan defaults by 10-15% and improve overall profitability [(see Potential Impact of Recommendations)](#Potential-Impact-of-Recommendations).

## Methodology
### Data Sources
The primary data source for this analysis is a loan application dataset comprising of 20,000 rows and 36 columns, including:
- Application Date
- Applicant Demographics (Age, Marital Status, Number of Dependents)
- Financial Information (Annual Income, Credit Score, Employment Status, Loan Amount, Loan Duration, Debt-to-Income Ratio, etc.)
- Loan Specifics (Loan Purpose, Previous Loan Defaults, Payment History)
- Risk Assessment (Risk Score, Loan Approved)
Each row in the dataset representing a unique application

![Original dataset](assets/Loan_-_Data_Source_Excel.png)

### Tools Used
The following tools were used for data analysis and visualization:
- Microsoft Excel – Data familiarization and exploration
- Microsoft SQL Server – Data cleaning and aggregation
- Microsoft PowerBI – Data visualization

### Data Cleaning and Preparation
The following data cleaning and preparation steps were performed using SQL:
- Converted the "ApplicationDate" column to the appropriate date data type.
- Converted the "LoanApproved" column values from 0 and 1 to "Declined" and "Approved" respectively for better readability.

### Data Exploration
Initial data exploration involved familiarizing ourselves with the dataset and identifying key variables. This included examining net worth, credit scores, and risk scores across different application statuses.

### Data Analysis Techniques
The following data analysis techniques were employed:
- Trend Analysis: We analyzed trends in loan applications and approval rates over time, specifically by year. This involved aggregating data by year and visualizing the trends to identify any significant changes in loan application volume or approval criteria.
- Comparative Analysis: We compared the financial profiles and risk scores of approved and declined applicants to identify key factors that influence loan approval decisions. This involved grouping data by approval status and calculating descriptive statistics for key metrics such as average credit scores, annual income, and debt-to-income ratios.
- Diagnostic Analysis: This analysis was used to identify any significant differences or fluctuations in loan approval rates or risk scores over time. By examining various factors such as economic conditions, changes in lending policies, or shifts in applicant criteria, we aim to better understand the underlying reasons for these fluctuations.

## Future Considerations for Data Analysis
In the future, we can leverage additional data analysis techniques to further refine our understanding of financial risk and optimize loan approval processes. These techniques include:
- Predictive Modeling: This technique can be used to build risk prediction models that assess the likelihood of loan default based on applicant characteristics and financial history. By incorporating machine learning algorithms and advanced statistical methods, we can develop more accurate risk assessment tools and improve loan approval decisions.
- Segmentation Analysis: This method involves dividing loan applicants into distinct groups based on shared characteristics such as risk profiles, financial stability, or loan purposes. By understanding the unique needs and risks associated with different applicant segments, we can tailor specific loan products, customize approval criteria, and minimize potential financial losses.

## Analysis of Loan Approval Trends
### Overall Trends
The overall loan approval trends are summarized below:
- Total Applicants: 2,557 applicants
- Approved Applicants: 600 (23.5% approval rate)
- Average Approved Applicants per Year: 86
- Declined Applicants: 1,957 (76.5% decline rate)
- Average Declined Applicants per Year: 280

## Analysis of Applicant Profiles by Approval Status
Approved applicants consistently exhibited higher credit scores, annual income, and net worth compared to declined applicants. This suggests that these factors play a significant role in loan approval decisions.

|Metric|Approved Applicants|Declined Applicants|
|---|---|---|
|Average Credit Score|583.71|568.14|
|Average Annual Income|$103.68k|$45.34k|
|Average Net Worth|$119.36k|$59.10k|
|Average Liabilities|$35.32k|$37.06k|
|Average Debt-to-Income Ratio|0.16|0.49|
|Average Age|42|39|
|Average Risk Score|40.25|54.02|


## Year-over-Year Analysis
A year-over-year analysis of key metrics revealed some fluctuations in applicant profiles and risk scores. For example, in 2018, approved applicants had a higher average net worth ($140.91k) compared to other years, while in 2021, declined applicants had a higher average debt-to-income ratio (0.54). These fluctuations may be attributed to various factors such as economic conditions, changes in lending policies, or shifts in applicant demographics.

## Correlation Analysis
A correlation analysis was conducted to identify potential relationships between various financial factors and risk scores. The analysis revealed the following:
- Strong positive correlation: A strong positive correlation was observed between risk score and debt-to-income ratio, indicating that applicants with higher debt-to-income ratios tend to have higher risk scores.
- Weak negative correlation: A weak negative correlation was observed between risk score and credit score, indicating that applicants with higher credit scores generally have lower risk scores.
These correlations highlight the importance of considering multiple financial factors when assessing loan applications and determining risk scores.

## Recommendations
Based on the analysis of loan approval trends and risk factors, the following recommendations are proposed:
- Refine Risk Assessment Models: Incorporate additional factors such as employment status, education level, and loan purpose into risk assessment models to improve the accuracy of loan approval decisions.
- Monitor Applicant Trends: Continuously monitor trends in applicant demographics, financial profiles, and risk scores to identify potential shifts in risk levels and adapt lending policies accordingly.
- Develop Targeted Loan Products: Develop loan products tailored to specific applicant segments with varying risk profiles and financial needs.
- Enhance Credit Scoring: Explore alternative credit scoring models that incorporate non-traditional data sources to assess creditworthiness more comprehensively.
- Educate Applicants: Provide educational resources and financial counseling to loan applicants to promote responsible borrowing and improve financial literacy.
- High Interest Options: For applicants with high net worths or high income, but also high risk scores, provide them with loans with higher interest rates to increase profits on risky loans as opposed to declining them altogether.

## Potential Impact of Recommendations
By implementing these recommendations, the financial institution can anticipate the following positive outcomes:
- Reduced Loan Defaults: Refining risk assessment models and implementing targeted lending strategies can potentially reduce loan defaults by 10-15%.
- Improved Profitability: Minimizing loan defaults, optimizing lending practices, and creating high interest loan options for high net worth/income applicatns with high risk scores, can lead to increased profitability and financial stability.
- Enhanced Customer Satisfaction: Providing personalized loan products and educational resources can improve customer satisfaction and loyalty.

## Limitations and Future Considerations
While this analysis provides valuable insights and recommendations, it's important to acknowledge certain limitations:
- Data Availability: The analysis is limited by the available data. Access to more granular data, such as detailed credit history, loan default history, and employment records, would allow for a more comprehensive risk assessment.
- External Factors: External factors such as economic downturns, changes in interest rates, and regulatory changes can significantly impact loan performance and should be considered in future analyses.

## Key Takeaways
This analysis provides valuable insights into loan approval trends and risk factors. Here are the key takeaways:
- Creditworthiness is a key factor in loan approvals: Approved applicants consistently exhibited higher credit scores, annual income, and net worth compared to declined applicants.
- Debt-to-income ratio is strongly correlated with risk: A strong positive correlation was observed between risk score and debt-to-income ratio, highlighting its importance in risk assessment.
- Fluctuations in applicant profiles and risk scores occur over time: Year-over-year analysis revealed variations in key metrics, suggesting the need for continuous monitoring and adaptation of lending policies.
- Refined risk assessment models can improve loan approval decisions: Incorporating additional factors and alternative data sources can enhance the accuracy of risk assessment and minimize potential losses.

By implementing the recommendations outlined in this report and continuously monitoring key performance indicators, the financial institution can optimize its lending practices, mitigate financial risks, and achieve sustainable growth.
