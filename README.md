# House Price Prediction
### Dimension reduction and clustering analysis

## Table of contents
* [Introduction](#introduction)
* [Technologies](#technologies)
* [Installation](#installation)
* [Data Preparation](#data-preparation)
* [Description](#description)

## Introduction
The project is to predict house sale price. With 79 explanatory variables describing (almost) every aspect of residential homes, the challenge is to predict the final price of each home. The data includes many categorical variables and traditional dimension reduction and clustering techniques cannot be applied directly to categorical data. This project explores two methods to perform house price prediction using numerical and categorical features.
1. Dimension reduction using
*	i. PCA for numerical variables
*	ii. MCA for categorical variables
2. K-medoids clustering using Gower distance 
	
## Technologies
Project is created with:
* Python : 3.7
	
## Installation
To use gower_matrix, install gower using:
pip install gower

## Data Preparation
Download the dataset from https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview
Remove missing value records before proceeding.

## Description
Part 1 - Dimension reduction: 
Dimension reduction is performed using Principal componenet analysis (PCA) for numerical features and Multiple correspondence analysis (MCA) for categorical fatures. Prediction is performed on the new features using linear regression with ridge regularization model. The model results are then compared with base model to test the performance.

Part 2: Clustering Analysis:
K-medoids clustering is performed using Gower distance as a distance measure. The Gower distance is essentially a special distance metric that measures numerical data and categorical data separately, then combine them to form a distance calculation