# Predicting Customer Churn
Predicting customers churn using three predictive models and comparing their performances.

[**See full presentation here.**](https://github.com/hu-zhiling-540/Predicting-Customer-Churn/blob/master/Presentation.pdf)

## Predictive models

### Best Model: Random Forest Classification
### Details:
- Split data to train set and test set
- By calculating the percentage of “Yes” and “No” in churn column, identify whether data is imbalanced
- Use SMOTE oversampling to balance data
- Fitting multiple models using KFold

###
- Among 3 different models we tried, Random Forest and Logistic Regression are better in scores.
- Select Random Forest for further analysis Accuracy with Random Forest: 0.845593
- Mean cross validation score: 0.828476

| ![space-1.jpg](https://github.com/hu-zhiling-540/Predicting-Customer-Churn/blob/master/Visulizations/Feature%20Importances.png) | 
|:--:| 
| *Feature importances with forests of trees* |

 
## Recommendations/ Suggestions
- Customers with lower tenure are more likely to terminate the contract. 
We suggest to target customers with less than 12 month tenure.
- As total charges rise up, people feel more pressured to leave the program. We suggest to find a threshold/ trade-off between profit earned and the number of customers.
- The other factors that could be taken into account are contract plans and payment methods. We had a rough guess that customers with long-term contracts, such as one and two year’s, are much less likely to churn than the monthly ones. We suggest to promote customer to switch to long term contracts
