# LendingClub

## Introduction

Lending Club is an online lending platform that follows the Peer-to-Peer(P2P) lending business
Model. This model enables borrowers and lenders to engage in online borrowing and lending
processes dodging the traditional loan process. One of the biggest advantages of the P2P platform
is that the loans are offered at a much lesser interest rate than the loans offered by conventional
banks. (https://www.lendingclub.com/)

In this project, I analyzed Lending Club data from 2013 to 2015, totaling 100K observations. The goal is to create various models that can predict which loans are likely to default. To predict loan default rates and devise an investment strategy, various models such as Decision Trees, Random Forest, Boosting models, and linear models were developed.

## Data Exploration 

### Distribution of the loans:
![image](https://user-images.githubusercontent.com/22790699/150661828-1e3adab9-6b36-422b-8451-8ce94502f0bb.png)

### Sub-grade wise distribution:
![image](https://user-images.githubusercontent.com/22790699/150661844-f855b95a-5d7a-4e96-8c65-0ec0aa39a519.png)

### We can see that the average intrest rate of loans increase as we go from Grade-A to Grade-G
![image](https://user-images.githubusercontent.com/22790699/150661918-01e11e2b-89e4-47fb-ae08-c3bb9146b62b.png)

### The time is taken to pay off the loans from Grade A to G increases.
![image](https://user-images.githubusercontent.com/22790699/150661936-09b56708-a2b9-4925-8651-269ff34c9357.png)

## Data Cleaning

I am removing two sets of variables:

1: Variables for which for which data may not be available for new loans before they are funded.

2: Variables for which the data which may have been updated during the loan period (ie., after the loan is funded).

Examples: emp_title, title, zip_code, addr_state, out_prncp, term, total_pymnt_inv, funded_amnt_inv, out_prncp_inv, total_pymnt_inv, total_rec_prncp

## Variable Selection:

Univariate Analysis:
I calculated the area under the curve for the ROC curve. I then used the pROC library to perform the analysis. This is to compare the area under the curve between different variables (response/dependent and prediction variables) to prevent overfitting in the data.

### Descending order of their AUC values
![image](https://user-images.githubusercontent.com/22790699/150662104-fa895d16-af4d-4388-ba8c-8ba8aaa72b56.png)


## Part-3: Decison Tree models

## Part-4: Random Forest

## Part-5: xgBoost

## Part-6 Linear Models

##Which grades to invest in to maximize the the profit from investing in LC loans





