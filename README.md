# PREDICTING-REAL-ESTATE-PRICES-WITH-MACHINE-LEARNING-IN-R
PREDICTING REAL ESTATE PRICES WITH MACHINE LEARNING IN R



#Introduction:

I've grabbed a dataset from Kaggle for housing sales price prediction. I've applied linear and
neural network operations to it to obtain the desired output, and then I compared the results with the
predefined values.
#Research Question:
When I found out about the final project for this subject, I was really excited to apply what
I've learned throughout the class. So, I began searching for a dataset on Kaggle. During my search, I
stumbled upon a competition focused on predicting housing prices using machine learning models. As
an undergrad student in civil engineering, this caught my attention because I've previously worked on
a final project about estimating and costing a four-storied building. Interestingly, my estimate for the
project had a 98% accuracy rate. However, I later discovered that the building sold for nearly 1.5 times
more than my quoted price. This discrepancy intrigued me, prompting me to delve deeper into
understanding the factors influencing housing prices. Hence, I decided to undertake this project to
gain insights into the variables considered in determining house prices.
#Data Description:
I grabbed this dataset from Kaggle, where a competition was ongoing. The task required
advanced regression techniques, including neural networks. The dataset, compiled by Dean De Cock,
was designed for data science education. It details the sale of individual residential properties in Ames,
Iowa, spanning from 2006 to 2010.
To handle missing values, I opted for mean and median imputation where there were only a few null
values. For columns with a significant number of missing values, I simply removed them. Additionally,
for categorical data, I filled in missing values with the most frequent value.
The House Prices dataset comprises 79 variables that describe various features of residential
properties in Ames, Iowa. Here's a brief overview of some key variables:
SalePrice: The target variable, the sale price of the property in dollars.
MSSubClass: Identifier for the type of dwelling structure.
LotArea: Size of the land parcel in square feet.
OverallQual: Overall material and finish of the house. Ranked on a scale from 1 (poor) to 10 (excellent).
GrLivArea: Above grade (ground) living area square footage.
TotalBsmtSF: Total square footage of basement area.
FullBath: Number of full bathrooms.
HalfBath: Number of half bathrooms.
BedroomAbvGr: Number of bedrooms above grade.
GarageCars: Number of cars the garage can hold.
GarageArea: Size of garage in square feet.
YearBuilt: Original construction year.
YearRemodAdd: Year of the latest remodeling or addition.
Neighborhood: Physical location of the house within Ames, Iowa.
#Methods:
Linear Regression:
Method: Linear regression is a statistical technique used to model the relationship between a
dependent variable (in this case, the sale price) and one or more independent variables (the house
features).
Justification: Linear regression offers a straightforward approach to understanding the linear
relationship between features and the continuous outcome variable, the sale price. It provides
interpretable coefficients indicating the direction and strength of influence of each feature on the sale
price.
Linear Relationship: The association between features and the sale price is assumed to be linear.
Random Forest (RF):
Method: Random forest is a machine learning technique that constructs an ensemble of decision
trees. Each tree makes predictions based on a random subset of features, and the final prediction is
the average of all tree predictions.
Justification: After considering the pros and cons of both models, I have chosen the Random Forest
(RF) model. RF is well-suited for handling complex, non-linear relationships between features and the
sale price. It offers robustness against outliers and can accommodate a larger number of features
without overfitting the data.
Assumptions: While Random Forest makes fewer assumptions compared to linear regression, it
assumes that the features are independent or weakly dependent on each other.
Choosing the Right Method:
Given the complexity of the data and the need for accurate predictions, the Random Forest model
was selected as the preferred choice for house price prediction.
Implications:
These findings hold practical implications for real estate agents or homeowners, providing valuable
insights into estimating the value of similar properties based on the model's included features. If the
Random Forest model significantly outperformed others, it indicates that capturing non-linear
relationships between features and price could be crucial for accurate predictions within this
dataset.
Limitations:
The accuracy of the models is inherently tied to the quality and completeness of the data. Factors
not accounted for in the dataset, such as specific location details or property conditions, could
potentially influence sale prices but are not considered. Additionally, the models represent a specific
point in time (sale prices from 2006-2010) and may not directly translate to current market
conditions. Furthermore, it's important to note that the code's removal of columns with a high
percentage of missing values could introduce bias if the missing data is not randomly distributed.
Missing Values:
Addressing missing data posed a primary challenge due to its potential impact on model
performance. Various imputation techniques were explored, including mean and median imputation
for variables with minimal missing values. However, for columns with a substantial amount of
missing values, removal was deemed necessary to ensure dataset integrity while preserving
relevance.
Feature Selection:
Feature selection plays a crucial role in enhancing model performance by reducing noise, improving
interpretability, and preventing overfitting. The removal of columns with a high percentage of missing
values serves as a common preprocessing step, indirectly aiding feature selection by reducing noise
and improving interpretability. However, this approach may lead to information loss, emphasizing the
importance of considering alternative techniques like imputation or feature engineering before
resorting to removal to effectively utilize the data.
Summary:
This study investigates the application of machine learning models for predicting house prices using a
dataset on houses in Ames, Iowa (2006-2010). The analysis focuses on two primary models: linear
regression and Random Forest.
Feature Selection: The code implements feature selection for the linear regression model, retaining
only features with statistically significant p-values.
Random Forest: The Random Forest model incorporates missing value imputation for both numerical
and categorical features.
Model Comparison: In terms of model comparison, the linear model achieved an accuracy of
approximately 0.79 on the test dataset, while the Random Forest model boasted an accuracy of 0.91.
Given this significant difference in accuracy and the Random Forest's ability to handle missing values
effectively, I've decided to confirm the Random Forest model as it outperforms the linear model and
demonstrates higher accuracy overall.
Significance:
Accurate prediction of house prices is essential for various stakeholders in the real estate market. This
study contributes to real estate valuation by.
Demonstrating model-based approaches: It underscores the potential of machine learning models for
predicting house prices using relevant features.
Comparing model complexity: By examining both linear regression and Random Forest, it offers
insights into the benefits of leveraging more complex models to capture non-linear relationships in
the data.
Future Research:
Several avenues for future research could build upon this study:
Improved Feature Engineering: Techniques such as feature creation or dimensionality reduction could
be explored to extract more informative features from the data.
Model Selection and Tuning: Experimenting with different machine learning algorithms and finetuning hyperparameters for the selected models (linear regression and Random Forest) could
potentially enhance performance.
Incorporating Additional Data: Integrating external factors like location data or economic indicators
might augment the model's ability to capture real-world influences on house prices.
Model Generalizability: Evaluating the models on a more recent dataset or data from different
locations would assess their generalizability to current market conditions and broader geographical
contexts.
Reference:
Kaggle Data Set: - https://www.kaggle.com/competitions/house-prices-advanced-regressiontechniques
Library: - randomForest
ChatGPT: - I employed grammatical error-checking tools while crafting this document, striving for
linguistic accuracy and coherence. Furthermore, I endeavored to integrate sophisticated English
terminology to elevate the presentation and enhance the overall professionalism of the report.
