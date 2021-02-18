# Quick View 
This project contains a  dataset for an airline passenger satisfaction survey. What factors are highly correlated to a satisfied (or dissatisfied) passenger? Can you predict passenger satisfaction?

# Project Summary
The aviation industry, like most fast-paced businesses, requires swift action to retain or attract customers. With the aid of data analytics, creating a business model that reflects on customer demands through uncovering patterns in a data-driven model is paramount.

Other essential tasks will involve correlation tests; this will generate a mapping of variables in relation to multicollinearity. Variables with high variance from the "Satisfaction" independent variable will play a vital role in the modeling stage while ones with little or no variance will be excluded.

Understanding the service dimensions such as "Leg Room Service", "Inflight Entertainment", "On-board Service" and "Checkin Service" will possibly lead to feature engineering. The target variable (Satisfaction) can undergo data transformation through either label encoding with "Yes" or "No" (0 or 1) outcomes.

Correspondingly, we will treat this as a binary classification problem, where we will try to create a model that predicts whether the customer is satisfied or not with the experience and/or service provided by the airline.

The following sections will illustrate the steps taken to develop the model;

# I. Data Collection
The Airline Passenger Satisfaction data was collected from Kaggle.com, which contains responses from a US airline passenger satisfaction survey.

# II. Data Cleaning
Based on the data, there are several things that we need to do to prepare the data before fitting it to a model. There are a few categorical variables that need to be encoded, including the target variable "Satisfaction". There are also a couple of columns that can be dropped, such as "Unnamed: 0" and "id", since they don't contain useful information.

# III. Exploratory Data Analysis
The EDA will involve processes related to understanding characteristics of given fields in the underlying data such as variable distributions, whether the dataset is skewed towards a certain demographic, and the data validity of the fields. For instance, a training dataset may be highly skewed towards Class. If so, how will this impact the results when using it to predict the remaining customer base. In addition, we might ask some interesting questions like: Is the business class generally better rated than the other two classes? Which features/services are poorly rated across all classes?

Secondly, identifying limitations surrounding the data and gather external data which may be useful for modelling purposes. This may include exploring other airline data at different service dimensions and creating additional features for the model. For example, (provide possible feature engineering idea) Exploration of interactions between different variables through correlation analysis and look out for multicollinearity by creating interaction variables. An example of this correlation may occur between independent variables "Age" and "Class" – i.e. people of the older brackets will be more inclined to a particular class offering.

Furthermore, transformation of required data so that it is in an appropriate format for analysis. This may include steps such as ensuring that the data types are appropriate and rolling data up to an aggregated level. Or, joining in already aggregated external source data (provide example) to create additional variables.

Another possible step to do is factor analysis, where we describe the variability among correlated variables in fewer variables (factors). For instance, instead of having multiple variables to describe the service (On-board Service, Baggage Handling, Inflight Service, etc.), we could work with one factor called "Service".

# IV. Modeling Data
This will involve providing questions that the model should have answers to. For instance, understanding which type of customers are the least satisfied with the airline service, whether or not there is a demographic bias towards such customer's rating. In addition, understanding the limitations poised by the given data, performing feature engineering and data transformation as stated above to create a data model that will effectively attempt to clarify such questions is essential. Other considerations regarding customer demographics can be obtained through data transformations such as binning the "Age" variable into groups to better understand customer persona.

Identifying the relationship between "Loyal Customers" and multiple airline service dimensions, such as "Type of Travel" and "Class" are also necessary. High value customers will be identified through ranking the "Flight Distance" variable into "High", "Medium", or "Low". This will be useful in creating actionable insights to target particular clients for more services. The model's output will be useful in acknowledging the levels of satisfaction from the client and will spur service improvement from the airline.

Finally, testing all variables for multicollinearity and detecting outliers will allow for a well-performing model. Additionally, acknowledging which of the variables has the most important predictor variables through regression coefficients, changes in the R-Squared value, and ANOVA tests. Various metrics such as AUC or ROC Curves, R Squared, Precision-Recall and the F-Measure will serve as our baseline for performance evaluation. Once multiple evaluations have been successfully deployed, documenting the model’s performance, assumptions and limitations will be satisifed.

V. Data Intepretation
Visualization and presentation of findings.
This will involve interpreting the significant variables and coefficient from a business perspective.
Practical and actionable insights that can be taken by the airline to improve overall service and customers' satisfaction.
