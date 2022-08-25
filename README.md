# Air_bnb@Rental-Price
The selected dataset belongs to the in-depth details of Airbnb rental stays and the property  description with stay feedback. The records of stay in the dataset about 500,000 entries and 89  attributes in it including target variables such as daily price, weekly price and monthly price. Problem statement of the dataset is to predict prices for the upcoming future. This problem  statement puts us in the domain of Sales Prediction. 

# Attribute Information:
* The dataset has information related to property type, area, date, price, reviews, etc. which is useful in predicting future price.
* Data also has information about amenities , location, host, host whereabouts, feedbacks, availability and other important features. 
* Data contains globally made bookings in detail.
* Since our target variable is numeric so it is an end to end Regression problem.

# Further Analysis and EDA:
* At the initial stage, in the dataset many of the variables were totally redundant, there was no significance to consider them in the further modelling process we dropped them.
* After exploring the dataset and brainstorming we concluded that, global dataset correlation of attributes with price (Tgt var) is very weak thus we agreed to work on data of one country i.e. US.
* After filtering records of US, we found correlation of attributes with our target variable and manually picked numerical attributes out of 32 numerical attributes with moderate and above better correlations.
* Some attributed (e.g. Square feet) had more tan 70% of missing values in it, which had to be dropped.
* We dropped null values from attributes which were negligible in count as compared to total data.
* We also imputed some of the missing values accordingly, if a particular variable is numerical than we imputed mean value or if the variable is categorical then we imputed mode value.

# Statistical Analysis:
* We performed some statistical tests to check the significance of any particular variable for the modelling or to see the significance with target variable.
* After performing tests we were able to see some of the variables has a relation in explaining the target variable (e.g. Location,Accomodation are some of them which explains rental price of any particular property.)

# Model:
* We considered Logistic Regression as our base model, in ols summary we were able to see some of the variables were showing p-value more than 0.05 so for the next model we removed those variables.
* After considering the significant variables on the basis of p-value we were able to get approx 58 r2 score value.
* For the next model we perform some hyper-parameter tuning and also used feature selection techniques such as RFE and SFS.
* At the final model we were able to get a r2 score value approx 73.
* From the above analysis and modelling, for business perspective we see which variables show impact on rental price of an air_bnb property.




