# Airline-Passenger-Satisfaction


**Classification of Airline Passenger Satisfaction**

![image](https://user-images.githubusercontent.com/29515861/191596044-731342c4-b720-4944-9be5-42a4e4421c8f.png)


**Problem Setting**

Classification is the process of recognizing, understanding, and grouping ideasand objects into 
preset categories. The process involves the use of data which consists of input training data to 
predict the likelihood that subsequent data will fall into one of the predeterminedcategories. This 
data is related to an airline organization and consists of the details of customers who have 
already flown with them. The opinion of the customers on various features, attributes, and flight 
data has been consolidated. The airline industry has proven to be very beneficial but along with 
that it also faces several issues ranging from a high level of competition among airlines to 
increasing customer demands for better services. All these factors require the airline industry to
constantly evolve, innovate and transform to provide better hospitality and services.
Hence it is vital for thi3s industry to understand the various factors that drive to make 
conclusivedecisions and deliver them to keep up with customers’ expectations.

**Problem definition**

The intention of this project is to showcase how Data mining and Machine learning approaches 
can be used to tackle business problems faced in the airline domain. The project is an attempt to 
build various classification models and choose the best model that predicts Airline passenger 
satisfaction. The main purpose is to classify whether a future customer would be satisfied with 
their service given the details of the various parameters’ valuesthat constitute customer’s 
satisfaction. One of the outcomes is also to understand which variablesplay a crucial role in 
shifting passenger feedback towards ‘satisfied’.

**Data Sources** 

We will be taking the data source from Kaggle. Link: https://www.kaggle.com/teejmahal20/airline-passenger-satisfaction

**Data Description**

The Dataset (test.csv &train.csv) consists of various factors and attributeswhich will be utilized to
understand customer satisfaction. Below are its properties:

• Number of columns - 24
• Number of rows- More than 1 lakh records
• Variable names: Gender, Customer Type, Age, Travel Type, Class, Flight Distance Seat
comfort, Departure/Arrival time convenient, Food and drink, Inflight Wi-Fi service etc.

**Data Understanding**

The dataset consists of 129880 instances and 24 columns. There is one target variable called 
satisfaction. By analyzing the data, we observe that the dataset contains both numerical and 
categorical data. The attributes are divided into three parts ‘Customer related attributes’, 
‘Airline related attributes’ and ‘others. The target variable is of binary nature where 1 
represents the satisfactory customers and 0 represents neutral/Dissatisfactory customers. There 
are 71,088 customers who are satisfies by the services provided by the airline and 58,794 
customers fall under the neutral/Dissatisfactory class.

**Data Processing**

The attribute ‘ID’ was removed from the dataset as it was not significant for the classification 
problem. On analyzing the summary of the data, we observed that the attribute ‘Arrival delay in 
minutes’ was having NULL values. In order to handle these NULL values, we correlated the 
variable ‘Arrival delay in minutes’ with ‘ Departure delay in minutes’. It was found that both 
variables are linearly co-related with each other. Also, it is quite logical to expect that if the 
departure of flight is delayed, the arrival time will also be delayed approximately by the same 
time. In order to handle the NULL values in the attribute ‘Arrival delay in minutes’ it will be 
filled with corresponding row values of ‘Departure delay in minutes’. Lastly, the categorical 
variables are being transformed into dummy variables. 

**Data Exploration** 

We have 129880 attributes and 24 columns. The attributes are divided into three parts.

1. Customer related attributes: Gender, Age, Customer Type, Type of Travel, Class
2. Airline Service-Related Attributes : Seat comfort, Departure/Arrival time convenient, 
Food and drink, Gate location, Inflight Wi-Fi service, Inflight entertainment, Online 
support, Ease of Online booking, On-board service, Leg room service, Baggage 
handling, Check in service, Cleanliness, Online boarding, Departure Delay in Minutes, 
Arrival Delay in Minutes.
3. Other : Flight Distance

We have mixture of numerical and categorical attributes, and attribute like "id" which will be 
not useful for classification. From the summary of attributes, we can see that the "Arrival Delay 
in Minutes" is having missing values. Apart from this we also have categorical variables which 
need to be transform into dummy variables.

Our Target column is having a balanced proportion of "Neutral or Dissatisfied" and "Satisfied" 
records.


![image](https://user-images.githubusercontent.com/29515861/191599872-411760f6-cbac-4c80-9871-608860912aa7.png)

**Model Exploration:**

Once we have the intuition of the Data and some insights of our predictor variables. Next step is to 
explore various Classification Models. We will implement the below models to understand the 
accuracy of each one of them and select the best performing one. Below we have explored various 
models and their advantages and disadvantages.

-Logistic Regression

-KNN Classifier

-Decision Tree

-Random Forest

**Impact of Project Outcomes**

-We have created a highly precise classification model for airline company to identify customer 
satisfaction. 
-After doing exploratory data analysis we would recommend the airline company to focus on improving seat comfort service, departure arrival time convenient. 
-We believe that this model will help business add value by considering this model as a reference to 
identify the customer behavior.

**Challenges faced during Project Execution**

-High Computation time for KNN and Decision Tree Classifier.
-Data handling of Null values and Data imputation. 



