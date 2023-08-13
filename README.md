# Nutritional Label for Give Me Some Credit Kaggle Competition

## By: Akshay Srinivasan and Rashed Rifat

## Introduction

This is a project completed for NYU's Responsible Data Science. The goal of this project is to create a nutritional label for an Automated Decision System (ADS),

A nutritional label refers to a simple, standard label for an ADS that allows users to determine the "fitness for use" for a particular objective. This tool was originally developed develop interoperability and transparency. To learn more about nutrional labels, refer to [this article by Professors Julia Stoyanovich and Bill Howe.](http://sites.computer.org/debull/A19sept/p13.pdf)

## Automated Decision System (ADS)

A solution for the [Give Me Some Credit Solution](https://www.kaggle.com/code/caesarlupum/modeling-give-me-some-credit) Kaggle competition was chosen (and ran) within Google Colab with the following modifications. The posting for the original competition can be found [here](https://www.kaggle.com/competitions/GiveMeSomeCredit/overview).

## Code

We provide links to the raw and Google Compatible Code as well. Alternatively, these files are also located with the code folder

- [Google Colab Compatible Code](https://colab.research.google.com/drive/1gqXJGckAZ2e-mpc812PgzILmvIYC3B_c?usp=sharing)
  - Requires NYU Email Address to access.
  - Follow instructions within the notebook to run properly. 

## Data

- The data was downloaded from Kaggle. This project uses the test.csv and train.csv files. The data can be downloaded from the [Kaggle Competition](https://www.kaggle.com/competitions/santander-customer-transaction-prediction/data).

## Modifications

- The original Jupyter Notebook was converted such that ti could be run within Google Colab. The following modifications amde this possible:
  
1. We mount the users Google Drive within the Notebook. We then specify the input path for the data using the mounted Google Drive.
2. We pickle the list of models after an initial execution of the program so as to save on time and resources. Subsquent runs of this program will rely on the pickled models, instead of training them from the start. 

## Pickling

We note that due the time required to build the model and the limited resources afforded to train this algorithm, the list of models is pickled (saved as binary file). These models are noted within the pickled-models directory. We note the variables that are pickled below.
