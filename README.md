# PyCaret-Regression-Models--HousePricePrediction-Kaggle-Competition-


![pycaret](https://user-images.githubusercontent.com/65406908/88789101-4dc65600-d164-11ea-932e-b645e64f64ab.PNG)



Step 1: The data files used for this repository are stored with in this repository (train_hp.csv, test_hp.csv and hp_sample_submission.csv)

Step 2: The code to build Machine Learning Models is with in "PyCaret- Predicting House Price.ipynb" Notebook


# Setting up the PyCaret with several parameters

###### numeric_imputation= mean (Mean value is used to impute the missing values for numeric variables)

###### ignore_features= [var] (Forcing the algorithm to remove these features while training the model)

###### normalization= True (is a technique often applied as part of data preparation for machine learning. The goal of normalization is to rescale the values of numeric columns in the dataset without distorting differences in the ranges of values or losing information.)

###### transformation= True (Transformation is a more radical technique. Transformation changes the shape of the distribution such that the transformed data can be represented by a normal or approximate normal distribution)

###### transform_target= True (This is similar to transformation, but applied to target variable)

###### feature_interaction= True (It is often seen in machine learning experiments when two features combined through an arithmetic operation becomes more significant in explaining variances in the data, than the same two features separately)

###### feature_selection= True (Feature Importance is a process used to select features in the dataset that contributes the most in predicting the target variable. Working with selected features instead of all the features reduces the risk of over-fitting, improves accuracy, and decreases the training time. In PyCaret, this can be achieved using feature_selection parameter)

###### remove_multicollinearity=True (Multicollinearity (also called collinearity) is a phenomenon in which one feature variable in the dataset is highly linearly correlated with another feature variable in the same dataset. Multicollinearity increases the variance of the coefficients, thus making them unstable and noisy for linear models. One such way to deal with Multicollinearity is to drop one of the two features that are highly correlated with each other. This can be achieved in PyCaret using remove_multicollinearity parameter within setup)

###### multicollinearity_threshold (Threshold used for dropping the correlated features. Only comes into effect when remove_multicollinearity is set to True)

###### ignore_low_variance= True (Sometimes a dataset may have a categorical feature with multiple levels, where distribution of such levels are skewed and one level may dominate over other levels. This means there is not much variation in the information provided by such feature. Such features are eliminated when this is set as True)



Step 3: The final submission file (with RMSE value of 0.14) that is submitted to the competition is named under this directory "submission_house_price_pycaret.csv"

Step 4: The saved model is loaded in the form of .pkl file which can be used for deployment. .pkl file is large to upload. It was compressed and stored with in repository as "Final CatBoost Model 27Jul2020.rar"

A PKL file is a file created by pickle, a Python module that enabless objects to be serialized to files on disk and deserialized back into the program at runtime. It contains a byte stream that represents the objects.

The process of serialization is called "pickling," and deserialization is called "unpickling." A PKL file is pickled to save space when being stored or transferred over a network then is unpickled and loaded back into program memory during runtime


![house price](https://user-images.githubusercontent.com/65406908/88789991-726efd80-d165-11ea-95ba-671a7f2c1fb5.PNG)



## Goal:
It is your job to predict the sales price for each house. For each Id in the test set, you must predict the value of the SalePrice variable. 

## Metric
Submissions are evaluated on Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted value and the logarithm of the observed sales price. (Taking logs means that errors in predicting expensive houses and cheap houses will affect the result equally.)

## Submission File Format
The file should contain a header and have the following format:

Id,SalePrice

1461,169000.1

1462,187724.1233

1463,175221
etc.



## Data fields
Here's a brief version of what you'll find in the data description file.

SalePrice - the property's sale price in dollars. This is the target variable that you're trying to predict.

MSSubClass: The building class

MSZoning: The general zoning classification

LotFrontage: Linear feet of street connected to property

LotArea: Lot size in square feet

Street: Type of road access

Alley: Type of alley access

LotShape: General shape of property

LandContour: Flatness of the property

Utilities: Type of utilities available

LotConfig: Lot configuration

LandSlope: Slope of property

Neighborhood: Physical locations within Ames city limits

Condition1: Proximity to main road or railroad

Condition2: Proximity to main road or railroad (if a second is present)

BldgType: Type of dwelling

HouseStyle: Style of dwelling

OverallQual: Overall material and finish quality

OverallCond: Overall condition rating

YearBuilt: Original construction date

YearRemodAdd: Remodel date

RoofStyle: Type of roof

RoofMatl: Roof material

Exterior1st: Exterior covering on house

Exterior2nd: Exterior covering on house (if more than one material)

MasVnrType: Masonry veneer type

MasVnrArea: Masonry veneer area in square feet

ExterQual: Exterior material quality

ExterCond: Present condition of the material on the exterior

Foundation: Type of foundation

BsmtQual: Height of the basement

BsmtCond: General condition of the basement

BsmtExposure: Walkout or garden level basement walls

BsmtFinType1: Quality of basement finished area

BsmtFinSF1: Type 1 finished square feet

BsmtFinType2: Quality of second finished area (if present)

BsmtFinSF2: Type 2 finished square feet

BsmtUnfSF: Unfinished square feet of basement area

TotalBsmtSF: Total square feet of basement area

Heating: Type of heating

HeatingQC: Heating quality and condition

CentralAir: Central air conditioning

Electrical: Electrical system

1stFlrSF: First Floor square feet

2ndFlrSF: Second floor square feet

LowQualFinSF: Low quality finished square feet (all floors)

GrLivArea: Above grade (ground) living area square feet

BsmtFullBath: Basement full bathrooms

BsmtHalfBath: Basement half bathrooms

FullBath: Full bathrooms above grade

HalfBath: Half baths above grade

Bedroom: Number of bedrooms above basement level

Kitchen: Number of kitchens

KitchenQual: Kitchen quality

TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)

Functional: Home functionality rating

Fireplaces: Number of fireplaces

FireplaceQu: Fireplace quality

GarageType: Garage location

GarageYrBlt: Year garage was built

GarageFinish: Interior finish of the garage

GarageCars: Size of garage in car capacity

GarageArea: Size of garage in square feet

GarageQual: Garage quality

GarageCond: Garage condition

PavedDrive: Paved driveway

WoodDeckSF: Wood deck area in square feet

OpenPorchSF: Open porch area in square feet

EnclosedPorch: Enclosed porch area in square feet

3SsnPorch: Three season porch area in square feet

ScreenPorch: Screen porch area in square feet

PoolArea: Pool area in square feet

PoolQC: Pool quality

Fence: Fence quality

MiscFeature: Miscellaneous feature not covered in other categories

MiscVal: $Value of miscellaneous feature

MoSold: Month Sold

YrSold: Year Sold

SaleType: Type of sale

SaleCondition: Condition of sale
