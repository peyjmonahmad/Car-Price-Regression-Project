# Predicting Used Car Prices

This repository includes used car data gathered from Autotrader.com and a linear regression model to accurately predict prices of each car.

First, I constructed a robust web scraper to extract meaningful vehicle information directly from the Autotrader web site.  Using a Selenium web automation tool and web page inspections,  I automatically clicked through web pages for each car to extract many vehicle specifications based on the tag of each web element.  The full details of this extensive process can be found in the Autotrader Web Scraper (.ipynb) notebook in this repository.

Once the data was gathered, I utilized correlation matrices as well as statistical metrics with Ordinary Least Squares to determine which features were necessary and relevant for further analysis.  I tested different combinations of features, and was left with five main features to effectively predict the price of a used car.

The following steps were performing linear regression with the remaining features.  After intial modeling resulted in decent predictive power,  I improved accuracy with grid search CV to find the optimal hyperparameters for this model.  Finally, using Lasso regression, I predicted prices with the highest accuracy scores yet.  The whole process of this modeling can be found in the Used Car Linear Regression (.ipynb) notebook.
