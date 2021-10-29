# CustomerChurn
![logo](https://upload.wikimedia.org/wikipedia/commons/thumb/6/69/Syriatel_Logo.svg/1280px-Syriatel_Logo.svg.png)

Resource https://www.kaggle.com/becksddf/churn-in-telecoms-dataset

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
![FirstChurn](https://user-images.githubusercontent.com/74070082/139340906-5b2f62f4-9e95-4caa-9222-47969511b6d1.png)

Overall, this data set is very clean. There are no missing values or NaNs to handle. We have dropped the area code and phone numbers for the privacy of the customer. We have added the total number of domestic minutes, calls and charges to gauge the total bill's effect on turn rate.

![Bills](https://user-images.githubusercontent.com/74070082/139340724-8c302231-0b00-4f85-af86-37edbbf5a24b.png)

Average bill for:
- All customers - $59.45
- Customers who stay -$58.45 
- Customers who churn- $65.36

$60 Flat rate option


![byState](https://user-images.githubusercontent.com/74070082/139340744-1336e73c-d93b-4854-956c-8098d4ccd644.png)

- Over 20% churn
- Targeted Marketing Campaigns 


![CustomerService](https://user-images.githubusercontent.com/74070082/139340852-b12cfcdc-5f9f-4173-a0d8-0609117dd873.png)

- The graph also shows that in proportion customers who stay with the company make fewer service calls. At 4 customer service calls there is a large increase in customer churn.

## Modeling


## Project Analysis

Offer discount on 4th customer service call
- Monitor calls

Provide a monthly rate option to customers
- Monitor enrollment

Target marketing campaign to high churn states
- Monitor state churn



## Navigating the Repository

```
├── notebooks
│         ├──Dave
│         └──Mellissa
├── images
│         ├──Bills.JPG
│         ├──byState.JPG
│         ├──CustomerService.JPG
│         └──FirstChurn.JPG
├── README.md
├── presentation.pdf
└── notebook.ipynb
```
