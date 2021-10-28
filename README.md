# CustomerChurn
![logo](https://upload.wikimedia.org/wikipedia/commons/thumb/6/69/Syriatel_Logo.svg/1280px-Syriatel_Logo.svg.png)

## Table of Contents
* [Business Overview](#business-overview)
* [Data Overview](#data-overview)
* [Modeling](#modeling)
* [Project Analysis](#project-analysis)
* [Navigating the Repository](#navigating-the-repository)

## Business Overview
The stakeholder is the telecom business. They are interested in reducing how much money is lost because of customers who don't stick around very long. If we can accurately identify any patterns, we can minimize the turn rate for the company, and as a result decrease costs associated with losing and having to regrow its customer base. We will be delivering an analysis of what factors go into causing customer churn. Our stakeholder is not constrained to any particular model. We will be able to investigate several different types of models. 
In our context, a false positive is identifying someone will leave when they actually stay. Alternatively, a false negative would be identifying someone who will stay but they will actually leave. A false negative is much worse for our stakeholders because missing customers that will leave defeats the purpose of analyzing this data set and developing the model. Missing these customers costs the company more money than a false positive. For this reason we will need to optimize our recall score for the models.

## Data Overview
The data comes from SyriaTel and includes information about their customers. The dataset has the customer's state of residence, telephone numbers and length of the account. There are columns indicating if the customer has an international plan and voicemail plan, how many voicemails they receive. The dataset includes how many minutes they spend talking, how many calls they make and how much they are charged during day, evening and night periods. Additionally, the data includes how many customer service calls each customer has made. And, the target variable, the customer's churn status. For our analysis, we will focus on the number of customer service calls each customer makes, what is each customer's total bill and if it affects the likelihood of churn and which states have the highest turn rate.

### Data Preparation
Overall, this data set is very clean. There are no missing values or NaNs to handle. We have dropped the area code and phone numbers for the privacy of the customer. We have added the total number of domestic minutes, calls and charges to gauge the total bill's effect on turn rate.


## Modeling
## Project Analysis
## Navigating the Repository

```
├── data
│        └── bigml_59c28831336c6604c800002a.csv
├── notebook
│         ├──Dave
│         └──Mellissa
├── images
│         ├──Capture.JPG
│         ├──Capture2.JPG
│         ├──Cat plot.JPG
├── README.md
├── presentation.pdf
└── notebook.ipynb
```
