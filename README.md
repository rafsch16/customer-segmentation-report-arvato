# Customer Segmentation Report for Arvato Financial Services

### Table of Contents 
1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Instructions](#instructions)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation<a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

This project is part of the Udacity Data Scientist Nanodegree program. The aim is to analyze demographics data for customers of a mail-order sales company in Germany. This requires to identify parts of the population that best describe the core customer base of the company. These findings are the applied using a model to predict which individuals are most likely to convert into becoming customers for the company.

First a Mann-Whitney U test was used to identify statistical differences in the attributes of the customer base and the general population. The most significant attributes were then used for customer classification using a training dataset from a previous marketing campaing of the company. The best results were obtained using a Random Forest classifier which achieved a ROC-AUC score of 0.75 for on a test dataset. A general discussion of the results can also be found in a [blog post](https://rafsch16.github.io/demographics/avrato/datascience/2021/11/16/customer-segmentation-report.html).

## File Descriptions<a name="files"></a>

The jupyter notebook file **'../Arvato Project Workbook.ipynb'** contains all of the code for this project.
- Loads the datasets for the customers and the general population
- Cleans the data and creates dummy variables for the categorical data
- Performs a Mann-Whitney U test for each attribute of the data
- Trains and tunes a model using scikit-learn's Pipeline and RandomSearchCV for customer prediction
- Compares models for scikit-learn's RadomForestClassifier, LogisticRegression, GradientBoostingClassifier

## Instructions<a name="instructions"></a>

Run the cells in the jupyter notebook file.

See the [blog post](https://rafsch16.github.io/demographics/avrato/datascience/2021/11/16/customer-segmentation-report.html) for a general discussion of the results.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
The datasets were provided by **Bertelsmann Arvato Analytics** and are accessible within the Udacity Data Scientist Nanodegree program only.
