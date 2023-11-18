# Hotel-Booking-Cancellation-Prediction
This project will mainly focus on leveraging data mining techniques to conduct exploratory data analysis (EDA) of bookings to address the business needs of customers and also build models to predict whether a booking will be canceled.

**(More details in the Code.ipynb and Presentation.pdf file)**

## Data Source
Hotel Booking Demand Datasets: Nuno Antonio, Ana Almeida, Luis Nunes, Data in Brief, 2019
https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand?datasetId=511638&sortBy=voteCount

## Techniques Used
 - Exploratory Data Analysis (EDA): This would involve looking at the distribution of the data, identifying any missing values, and visualizing the relationships between features using plots such as scatterplots and histograms.
 - Upsampling and SMOTE (which are used to address data imbalance problems)
 - Time series analysis: identify trends in booking demand or cancellation over time, such as seasonal patterns and fluctuations.
 - Clustering: K-Means & DBSCAN
 - Predictive modeling(Logistic Regression, Decision Tree, Random Forest, XGBoost, etc.): forecast future bookings or cancellations based on past data.

## Result
### Classification:
Our models' performance can be seen as follows:
<img width="1119" alt="Screen Shot 2023-11-17 at 10 37 44 PM" src="https://github.com/EllieZhangy/Hotel-Booking-Cancellation-Prediction/assets/133906690/aa0e02ef-7e26-4513-b873-8e363616a23d">
In this project, our primary focus was on the **recall rate**. Based on the data presented in the table, we selected **XGBoost** as our final model. Notable features influencing this decision include:
 - Requirement for Parking Spaces (Yes/No)
 - History of Previous Cancellations (Yes/No)
 - Market Segment Category

### Customer Segmentation:
Our analysis resulted in the segmentation of customers into **four distinct groups**:
 - Business Travellers: Prefer city hotels.
 - Self-driving Enthusiasts: Require parking spaces.
 - Group Travel Aficionados: Favor traveling in groups.
 - Loyal Guests: Tend to be repeat visitors.
The geographical distribution of these customer groups can be seen in the following chart:
<img width="753" alt="Screen Shot 2023-11-17 at 10 40 39 PM" src="https://github.com/EllieZhangy/Hotel-Booking-Cancellation-Prediction/assets/133906690/f5995b04-c715-4f51-bb54-ecbf5929292c">
