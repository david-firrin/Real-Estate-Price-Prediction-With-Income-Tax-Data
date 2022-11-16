# Team-48
Team 48's group project GitHub repository for MGT 6203 (Canvas) Fall of 2022 semester.

# Installation & Running Instructions

## Packages Required
The packages used in this project are as follows:
- tidyverse (includes dplyr)
- caret
- randomForest
- stats
- glmnet
- xgboost
- fastDummies

## Step 1 - Data Download
The data required can be downloaded from the following two data sources:
1. https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset?resource=download
2. https://www.kaggle.com/datasets/irs/individual-income-tax-statistics

Once the data is downloaded, it needs to be placed in the Data > Raw folder. In addition, the income tax data (which downloads as a zip) should be decompressed, so that all income tax data exists at Data > Raw > income_data > \[all income tax data files\].

## Step 2 - Data Transformation
To perform data transformation, the notebook Final Code > 01-DataJoin.Rmd needs to be run. This will create a number of processed datasets in the Data folder. 

If you've made updates to the code, perform the following actions. If not, proceed to the next step.
* Open merged_data.csv in Excel, and save it as an .xlsm file
* Add a new column G and I, labeled `house` and `house*acre lot` 
* Populate these columns with the formulas in the yellow-highlighted columns in the existing file at Data > 'merged_data_vF.xlsm' 
* Save file at Data > merged_data_vF.csv

## Step 3 - EDA
To perform EDA, simply run the notebook at Final Code > 02-EDA.Rmd.

## Step 4 - Model Selection & Evaluation
To perform model selection and evaluation, simply run the notebook at Final Code > 03-ModelDevSelection.Rmd

# Directory Overview
Please see below for general descriptions of the directory.

> - **Data:** Raw and processed data for use during models. The 'Raw' directory will contain a .md file with description of how to download the data
> - **Final Code:** Final R-markdown notebooks as well as .html versions with outputs included.. *These should be referenced as master versions of code*
> - **Final Presentation Slides:** Powerpoint file with final presentation slides
> - **Final Report:** Word and PDF docs with final report file
> - **Progress Presentation:** Powerpoint file with progress report presentation slides
> - **Progress Report:** Word and PDF docs with progress report file and R-markdown file with code to pull some additional figures
> - **Project Proposal:** Word and PDF docs with project proposal file
