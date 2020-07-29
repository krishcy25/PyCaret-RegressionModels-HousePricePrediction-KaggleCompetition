# PyCaret-Regression-Models--HousePricePrediction-Kaggle-Competition-

Step 1: The data files used for this repository are stored with in this repository (train_hp.csv, test_hp.csv and hp_sample_submission.csv)

Step 2: The code to build Machine Learning Models is with in "PyCaret- Predicting House Price.ipynb" Notebook

Step 3: The final submission file (with RMSE value of 0.14) that is submitted to the competition is named under this directory "submission_house_price_pycaret.csv"

Step 4: The saved model is loaded in the form of .pkl file which can be used for deployment. .pkl file is large to upload. It was compressed and stored with in repository as "Final CatBoost Model 27Jul2020.rar"

A PKL file is a file created by pickle, a Python module that enabless objects to be serialized to files on disk and deserialized back into the program at runtime. It contains a byte stream that represents the objects.

The process of serialization is called "pickling," and deserialization is called "unpickling." A PKL file is pickled to save space when being stored or transferred over a network then is unpickled and loaded back into program memory during runtime


#Goal:
It is your job to predict the sales price for each house. For each Id in the test set, you must predict the value of the SalePrice variable. 

Metric
Submissions are evaluated on Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted value and the logarithm of the observed sales price. (Taking logs means that errors in predicting expensive houses and cheap houses will affect the result equally.)

Submission File Format
The file should contain a header and have the following format:

Id,SalePrice
1461,169000.1
1462,187724.1233
1463,175221
etc.
