# Telecom-Customer-Churn-Prediction

## What is Customer Churn?
Customer churn is defined as when customers or subscribers discontinue doing business with a firm or service.

Customers in the telecom industry can choose from a variety of service providers and actively switch from one to the next. The telecommunications business has an annual churn rate of 15-25 percent in this highly competitive market.

Individualized customer retention is tough because most firms have a large number of customers and can't afford to devote much time to each of them. The costs would be too great, outweighing the additional revenue. However, if a corporation could forecast which customers are likely to leave ahead of time, it could focus customer retention efforts only on these "high risk" clients. The ultimate goal is to expand its coverage area and retrieve more customers loyalty. The core to succeed in this market lies in the customer itself.

Customer churn is a critical metric because it is much less expensive to retain existing customers than it is to acquire new customers.

To detect early signs of potential churn, one must first develop a holistic view of the customers and their interactions across numerous channels.As a result, by addressing churn, these businesses may not only preserve their market position, but also grow and thrive. More customers they have in their network, the lower the cost of initiation and the larger the profit. As a result, the company's key focus for success is reducing client attrition and implementing effective retention strategy.

Customer churn is a significant issue for big business companies. Companies are attempting to create methods for predicting customer churn to get a direct impact on getting more revenues, particularly in telecom companies. Finding these characteristics is crucial to ensure appropriate steps can be taken to reduce customer churn.

In this project, i made machine learning models to predict customers who churn and not churn. 
We will analyze three characteristics 
(1) services that the customer signed up for, 
(2) account information about the customer, and 
(3) demographic info. 
We use two machine learning models, K-Nearest Neighbors and Logistic Regression

## Dataset
The data set used for this article's classification problem is taken from Kaggle and IBM sample data set collection. 
[DataSet](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

### The data set includes information about:

- Customers who left within the last month – the column is called Churn
- Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
- Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
- Demographic info about customers – gender, age range, and if they have partners and dependents
## Implementation:

*Libraries:* sklearn, Matplotlib, pandas, seaborn, and NumPy

## Conclusion
In this project, using the Telco Customer Churn dataset i have demonstrated an end-to-end machine learning project from beginning to end. Data cleaning and visualization were our first steps. Then, to give better data to train with the machine learning model we have to change categorical data to numerical data and we scale the numerical data (feature engineering). After that, we tried to build two machine-learning models and we evaluated that. Logistic regression has a high accuracy compared with KNN. The ability to recognize potential customer scenarios where churn can be prevented requires a high level of accuracy since the benefits of the customer’s eventual returns must balance the expenses of associated retention initiatives.


## Few glimpses of EDA:
### 1. Data Overview:
![Data Overview](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/Data%20Overview.jpg)

- **Senior Citizen**: A relatively small percentage of customers are senior citizens (16.21%).

- We observed that the average customer tenure is 32 months, with 75% of customers staying up to 55 months.

- The average monthly charges for customers are around USD 64.76, with 25% of customers paying more than USD 89.85, suggesting a significant segment of customers are paying premium rates.

### 2. Analysis Services Each Customer
![Analysis Services Each Customer](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/Analysis%20Services%20Each%20Customer.jpg)

- Customers with phone service have a moderately higher churn rate compared to those without.
- Customers using fiber optic internet were more likely to churn compared to those using DSL or who have no internet service.
- Customers without online security have a significantly higher churn rate.
- Customers without tech support were found to leave more frequently, emphasizing the value of customer support services in retention strategies.
- The churn rate was also higher for customers who did not subscribe to online backup and device protection, suggesting that these add-on services help in retaining customers.

### 3. Customer services
![Customer services](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/customer%20services.jpg)

- Month-to-month contracts have a significantly higher churn rate compared to one-year or two-year contracts, suggesting that long-term contracts may reduce the likelihood of churn and contribute to customer retention.
- Customers who opted for paperless billing showed a higher churn rate, suggesting that these customers might be less engaged or feel less committed compared to those receiving paper bills.
- A moderately higher churn rate was observed for customers using electronic check as their payment method. This could indicate that certain payment methods are associated with less stable or more dissatisfied customers.

### 4. Comparing Churn Rates by Tenure, Monthly Charges, and Total Charges
![Comparing Churn Rates by Tenure, Monthly Charges, and Total Charges](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/Comparing%20Churn%20Rates%20by%20Tenure%2C%20Monthly%20Charges%2C%20and%20Total%20Charges.jpg)

- Customers with short tenure (newer customers) are more likely to churn. This indicates that early-stage customer retention is crucial for reducing churn.
- Customers paying higher monthly charges tend to have a higher churn rate. This suggests that high pricing might contribute to customer dissatisfaction or their decision to leave.
- Customers with high total charges also tend to churn, which may imply that the overall cost accumulated over time could be a factor in driving customers away.

### 5. Customer's Demographic Info
![Customer's Demographic Info](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/Customer's%20Demographic%20Info.jpg)

- There is no significant difference in churn rates between male and female customers, indicating that gender is not a major factor in predicting churn.
- Younger customers are more likely to churn compared to senior citizen customers, suggesting that age may influence customer stability and loyalty.
- Customers with a partner are less likely to churn than those without a partner, highlighting that family or relationship status may play a role in customer retention.

### 6. Outlier Checking
![Outlier Checking](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/Outlier%20Checking.jpg)

- Upon examining the boxplots for numerical variables such as tenure, MonthlyCharges, and TotalCharges, we found no significant outliers in the dataset. This indicates that the data is well-distributed, and there is no need for outlier removal or special handling to improve the accuracy of the machine learning model.

### 7. Correlation Analysis
![Correlation Analysis](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/Correlation%20Analysis.jpg)

- The variable Contract_Month-to-month has the highest positive correlation with churn. This indicates that customers with month-to-month contracts are significantly more likely to churn, making it a key predictor in the model.
  
- The tenure variable has a negative correlation with churn, meaning that customers with longer tenure (who have been with the company longer) are less likely to churn. This reinforces the importance of retaining customers during their early months.

### 8. Checked Accuracy Of Machine-learning models
![KNN - confusion matrix](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/KNN%20-%20confusion%20matrix.jpg)
![Logistic Regression - confusion matrix](https://github.com/heyamay/Teelecom-Customer-Churn-Prediction/blob/main/Logistic%20Regression%20-%20confusion%20matrix.jpg)

- After that, we tried to build two machine-learning models and we evaluated that. Logistic regression achieved an accuracy of 80.45% while KNN achieved an accuracy of 75.93%. Logistic regression has a high accuracy compared with KNN.

### 🚀 About Me
#### Hi, I'm Amay Jaiswal! 👋
I am a Data Analytics Enthusiast and  Data science practitioner

[Linkedin](https://www.linkedin.com/in/heyamay/)

Resume content -
• Developed a customer churn prediction model using Logistic Regression in Python with Scikit-learn, achieving 80% accuracy and outperforming KNN at 75%
• Conducted data cleaning and processing of over 7,000 customer records using Pandas and NumPy, improving model performance by 15% through feature engineering.
• Identified 20% higher churn for fiber optic users and 35% higher churn for month-to-month contracts.
  
