# CustomerChurn
![logo](https://upload.wikimedia.org/wikipedia/commons/thumb/6/69/Syriatel_Logo.svg/1280px-Syriatel_Logo.svg.png)


## Table of Contents
* [Business Overview](#business-overview)
* [Data Overview](#data-overview)
* [Modeling](#modeling)
* [Project Analysis](#project-analysis)
* [Navigating the Repository](#navigating-the-repository)

## Business Overview

The stakeholder is the telecom business. They are interested in reducing how much money is lost because of customers who don't stick around very long. If we can accurately identify any patterns, we can minimize the turn rate for the company, and as a result decrease costs associated with losing and having to regrow its customer base. 

## Data Overview

The data contains 3333 entries and the target variable, the customer's churn status. 

Overall, this data set is very clean. There are no missing values or NaNs to handle. We have dropped the area code and phone numbers for the privacy of the customer. We have added the total number of domestic minutes, calls and charges to gauge the total bill's effect on turn rate.
Resource https://www.kaggle.com/becksddf/churn-in-telecoms-dataset

## Modeling

Base on out businness problem we are looking to minimize False Negatives, so we will focus on optimizing our Model's Recall Score.
In our context, a false positive is identifying someone will leave when they actually stay. Alternatively, a false negative would be identifying someone who will stay but they will actually leave. A false negative is much worse for our stakeholders because missing customers that will leave defeats the purpose of analyzing this data set and developing the model. Missing these customers costs the company more money than a false positive. For this reason we will need to optimize our recall score for the models.

Models we tried:

- Logistic Regression
- Nearest Neighbor 
- Decision Tree
- XGBoost

![FirstChurn](https://user-images.githubusercontent.com/74070082/139453526-8e046a69-56f3-4fee-b7b4-6b992c0991e3.png)

This is baseless model based on raw data

![BaseMatrix](https://user-images.githubusercontent.com/74070082/139453943-46d7ec39-abd5-4981-b851-745fb3ec5aed.png)

This is our Logistic Regression model we used as a baseline model.

![CMatrix](https://user-images.githubusercontent.com/74070082/139453124-a24b17ca-5a29-4135-a7fa-1abddcd170b6.png)

This is our final model, tuned Decision Tree


## Project Analysis

Our final model produced a 87% recall score. And, it determined 3 of the most important features, which were Customer Services Calls, total price of the bill, and states with high churn.

### Business Recommendations:

Offer discount on 4th customer service call

Provide a monthly rate option to customers

Target marketing campaign to high churn states


## Navigating the Repository

```
├── notebooks
│         ├──Dave
│         └──Mellissa
├── images
│         ├──CMatrix.JPG
│         ├──BaseMatrix.JPG
│         └──FirstChurn.JPG
├── README.md
├── presentation.pdf
└── notebook.ipynb
```
