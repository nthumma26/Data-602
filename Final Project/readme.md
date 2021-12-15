**Exploratory Data Analysis & Prediction of Nature of property ownership**

**Business Objective**: To identify trends in the property taxes of Baltimore city by exploring the dataset and predicting the kind of property ownership by their respective attributes. From the last several years we have seen a tremendous rise in the property exchanges, and we are also paying the property tax bills for the charges levied according to state and locality. This project deals with analyzing historical data on property taxes and predicting the kind of ownership. 

**Target Audience**: This project assists government officials and other real estate exchange trusts i.e., who manage a wide range of properties to predict the kind of ownership of the property.

**Dataset Description**:

X: Longitude coordinate

Y: Latitude coordinate

address: Address of the property located

ownership: Indicator for type of ownership on property. H : Owner occupied principal residence, D : Dual use, N: Not owner occupied

land_use_c: The land use code of the property. R : residential, C : commercial, I : Industrial

total_lien: The total amount of liens on the property.

neighbourho: The neighborhood where the property is located.

when_sold: Category of the property sold type

block: The block number for the property.

lot: The lot number for the property.

pin: Zip code of the property located

soldto: Name of the buying party to whom the property is sold

ownername:The name of the owner of the property.

tax_base: The value of the property.

city_tax: The annual city property tax based on the assesed value of the property.

state_tax: The annual state property tax based on the assesed value of the property.

total_tax: The sum of the "City Tax" and "State Tax" columns.

total_3yea: Total tax paid for 3 years.

years_elig: The number of years the property has been eligible for tax sale in the past.

deed_date: The date that ownership of the property was transferred to the owner.

council_di: The city council district where the property is located.

objectid: The object id of the property.

**Execution Steps**:
1. Collecting the data and defining the data into a pandas DataFrame in python.

2. Observing basis statistics on the data

3. Performing Exploratory Data Analysis

4. Feature Engineering & Feature Selection 

5. Applying various classification algorithms

6. Choosing a metric to evaluate

**Explorative Data Analysis Outcomes**:

1) We can see that the total_tax values are between 1000 and 20000.

2) We can see that most of the properties have deed dates in June.

3) Most of the deeds happened in the year 2019.

4) Most of the properties are eligible for 11 years of taxation

5) The properties in council id 9 is paying the highest total taxes

6) The properties with 2 years of taxation are paying the highest taxes as compared to the other years

7) The properties with the "D" ownership indicator is paying the highest taxes

8) The properties with land use CC as the indicator has paid the highest total taxes and the properties with an indicator "I" has paid the next highest total taxes

9) It can be inferred that the properties that have labeled as sold in 4 years have paid the highest total tax with properties of 'D' indicator

**Outcomes:**

1) The logistic regression with l2 penalty has obtained a ROC_AUC score of 76%. 

2) The Logistic Regression with l2 penalty and liblinear solver has obtained a greater ROC_AUC score of 78% at 100 as the coefficient of regularization strength.

3) The Logistic Regression with l2 penalty and saga solver has obtained a ROC_AUC score of 76%, which is lower than liblinear solver.

4) Logistic regression with a liblinear solver at various regularization strengths has improved the performance of the model.

5) Decision trees classification model has improved the model, with a score of 86%. 

6) Support Vector Machine using grid search has also improved the model with the score of 87% with the hyper-parameters of C=1000 and Gamma =0.1. 

7) KNN algorithm has ROC_AUC score around 83%

8) We can infer that the SVM using grid search and decision trees classification model has improved the model.

9) Z-Scores are determined to remove the outliers. A Z-Score value greater than 3 is used to eliminate the outliers.

10) Chi-Square test is used to determine the most independent features and they are used for further modeling.

11) Total_tax, State_tax, city_tax, being_remo_WILL BE SOLD, years_eligible are the most important features of the model.

12) As we obtained a score of 87%, we must also consider other features as well for effective modeling.

**Further Developments**:

Enough number of training instances for all kinds of ownership indicators and the rich availability of training data lead to the development of a better model with improved scores. Model performance score could be improved by using neural network techniques. Rather than the statistical methods of determining the important features, business domain knowledge plays a key role in determining the useful features. Outliers treatment is also confined to the kind of business problem we are solving.

Further, Neural networks and ensembling learning can improve the performance of the model.
