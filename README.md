# Customer-Churn prediction
![customer churn](https://user-images.githubusercontent.com/94622826/218079040-89be92ae-9ca7-4050-9220-2a1c8b0f09a9.png)

## Overview 

It is important for companies to stay competitive and ensure **customer satisfaction** for several reasons. Firstly, customers have numerous options to choose from, and companies need to stand out in order to retain their business. If a company fails to provide a good experience, customers are likely to switch to a competitor. Secondly, happy customers are more likely to spread positive word of mouth and refer others, which can help a company to attract new customers and grow. On the other hand, unhappy customers can harm a company's reputation through negative word of mouth. Lastly, retaining existing customers is more cost-effective than acquiring new ones, and keeping them happy can lead to increased customer loyalty and repeat business. Therefore, staying competitive and ensuring customer satisfaction is crucial for a company's success and growth.

## Business understanding 

**Customer churn** refers to loss of customers over time and directly affects company revenue. Retaining customers is more cost-effective than acquiring new ones, so reducing churn is key to maintaining and growing customer base and revenue. Monitoring and reducing churn through understanding customer behavior and taking steps to improve satisfaction and loyalty is important for business growth.
### Main objective 

With the goal of retaining current customers, the primary objective of this project is to develop a predictive model that can identify customers who are at risk of churning. This will allow for targeted interventions to be focused on these customers, ultimately preventing them from leaving.

## Data understanding

This dataset contains 3333 instances and 21 columns and was sourced from https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset. Columns contain different information on customers such as 'state', 'account length', 'area code', 'phone number','international plan', 'voice mail plan', 'number vmail messages','total day minutes', 'total day calls', 'total day charge','total eve minutes', 'total eve calls', 'total eve charge','total night minutes', 'total night calls', 'total night charge','total intl minutes', 'total intl calls', 'total intl charge','customer service calls', 'churn (target)'

## Modelling 

In coming up with the best model, the following approach will be taken:

- Fitting a baseline model( logistic regression) to act as the benchmark

- Fitting other potential models such a random forest classifier, a support vector classifier, a Adaboost classifier and a XgBoost classifier

- Hyperparameters tuning of the two best models ( taking into account prediction accuracy and recall)

- Comparing vanilla versions of the two best models with the tuned versions of the models and selecting the best model to optimize our business problem

Capturing churning customers is of great importance as losing customers equits to losing business. The model with the highest recall and prediction accuracy score will be chosen as the final model as it will optimize the business problem

## Evaluation 

A randomforest classifier and a xgboost classifeirs were chosen as the two best models and compared against each other according to their performance on predicting new unseen data. in line with the business problem. The xgboost model was chosen as the model for deployment as it had and accuracy of 90% and a recall of 79%.

## Recommendations 

◍ There should be more emphasis on customer service calls as they can ultimately determine if a customer will churn or not. Customer calls are important because of the following reasons.

* Customer Retention: Good customer service can improve customer satisfaction and help to retain customers. Satisfied customers are more likely to continue doing business with a company and recommend it to others.

* Problem Resolution: Customer service calls provide a way for customers to quickly and easily resolve problems or get answers to questions about products or services. This can improve customer satisfaction and reduce frustration.

* Feedback: Customer service calls can provide valuable feedback to a company about its products, services, and customer experience. This feedback can be used to improve the customer experience and make changes that benefit both the company and its customers.

* Reputation Management: Good customer service can help to build and maintain a positive reputation for a company, while poor customer service can harm its reputation and negatively impact its brand.

◍ There should also be a strong emphasis on marketing and pricing to ensure that customers can opt into international plan as there is evidence that customers who have international are less likely to churn compared to those who do not have such a plan

◍ Review of marketing and pricing strategies to have more customers opt into the voice mail plan could also have the potential ensuring that a customer does not churn quickly as customers who do not have a voicemail are five times likely to churn than people who have a voicemail plan

◍ Review of marketing and pricing policies to ensure that customers enjoy favourable offers when making calls

◍ Consideration of collecting more demographic data on customers such as age and gender as it would provide extra information that the predictive model can use in identifying if a customer will churn or not
