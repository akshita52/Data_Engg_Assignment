### Data_Engg_Assignment

## Problem 1:
A company wants to predict employee productivity scores to improve workforce planning and training programs. You are hired as a Data Scientist to build a multivariate linear regression model that predicts an employee’s Productivity Score based on multiple work-related factors. 

# Experience (yrs), Training Hours, Working Hours, Projects, Productivity Score 
2,40,38,3,62 
5,60,42,6,78 
1,20,35,2,55 
8,80,45,8,88 
4,50,40,5,72 
10,90,48,9,92 
3,30,37,4,65 
6,70,44,7,82 
7,75,46,7,85 
2,25,36,3,60 

# Interpretation:
1. Which factor most strongly impacts productivity? 
2. How does training affect productivity? 
3. Should the company increase training hours or working hours? 
4. What happens if Working Hours increase beyond optimal limits? 
5. Can productivity ever decrease with more experience? 
6. How would you detect overfitting in this model? 
7. Suggest one new feature to improve prediction accuracy. 

## Problem 2:
A bank wants to detect fraudulent transactions in real time. 
Each transaction must be classified as: 
0 → Legitimate  
1 → Fraud 

# Data Set: 
# TransactionID,Amount,TimeSinceLastTxn,LocationChange,AvgTxnAmount,IsForeignTransaction,IsHighRiskCountry,CardPresent,IsFraud
1,1200,2,1,500,1,1,0,1 
2,50,24,0,200,0,0,1,0 
3,5000,1,1,450,1,1,0,1 
4,200,48,0,300,0,0,1,0 
5,1500,3,1,700,1,0,0,1 
6,75,72,0,150,0,0,1,0 
7,3200,2,1,400,1,1,0,1 
8,40,96,0,100,0,0,1,0 
9,2100,5,1,600,1,1,0,1 
10,60,120,0,120,0,0,1,0 

# Feature Explanation:  
Amount → Transaction amount  
TimeSinceLastTxn → Hours since last transaction  
LocationChange → 1 if location differs from previous  
AvgTxnAmount → User’s average spending  
IsForeignTransaction → International transaction  
IsHighRiskCountry → Risky country flag  
CardPresent → Physical card used (0 = online, 1 = swipe)  
IsFraud → Target variable 

# Interpretation:  
1. Write the logistic regression equation for this dataset.  
2. How do you interpret model coefficients (e.g., for Amount)?  
3. What happens if two features are highly correlated?  
4. Train a logistic regression model on this dataset  
5. Plot ROC curve  
6. Tune threshold (not just 0.5)  
7. Add regularization (L1/L2) and compare results 

## Problem 3: 
An e-commerce company wants to segment its customers into groups to: 
a. Personalize marketing campaigns  
b. Recommend products  
c. Improve customer retention  
Since there are no labels, we use Clustering (e.g., K-Means). 
CustomerID, Age, AnnualIncome, SpendingScore,VisitsPerMonth,AvgOrderValue 
1,22,15000,39,4,200 
2,25,18000,81,6,500  
3,47,60000,6,2,150 
4,52,65000,20,3,200 
5,23,20000,77,5,450 
6,45,70000,15,2,180 
7,33,40000,50,4,300 
8,35,42000,55,5,320 
9,60,80000,10,1,100 
10,28,30000,70,6,400 

# Feature Explanation:  
Age → Customer age  
AnnualIncome → Income in ₹  
SpendingScore → Engagement score (1–100)  
VisitsPerMonth → Platform usage frequency  
AvgOrderValue → Average purchase value 

# Interpretation:
1. Why should you scale features before clustering?  
2. What happens if features are on different scales?  
3. Would you include CustomerID in clustering? Why/why not?  
4. How do you decide the optimal number of clusters (K)?  
5. Explain Elbow Method and Silhouette Score. Implement the Elbow Method (plot WCSS vs K from 1 to 10). Compute the Silhouette Score for different values of K.  
6. Load the dataset and perform basic EDA (check nulls, summary stats).  
7. Normalize/standardize the features using StandardScaler.  
8. Apply K-Means clustering with k=3.  
9. Print the cluster labels for each customer.  
10. Find the centroids of each cluster. 
11. Based on both methods, choose the optimal K. 
