# Tokyo-Ramen-Takeichi-2024

## 1. Project Overview

Tokyo Ramen Takeichi is a renowned ramen chain that originated in Tokyo, Japan, and expanded its presence internationally. Known for its rich and flavorful broth, the chain has successfully established itself across several cities in the Netherlands and Germany.

As a part-time server at Tokyo Ramen Takeichi Amsterdam branch, I noticed that the restaurant has a large amount of data on sales and employee performance that remains largely untapped due to reliance on static spreadsheets.

Ramen Business is seasonal, peaking during the winter months and slowing down in summer. With growing competition, evidence-based marketing efforts and cost minimization are ccrucial toimproving business performance. I initiated this project to promote the transition from static spreadsheets to dynamic dashboards, enabling managers to make strategic decisions in areas such as seasonal promotions and staff scheduling.

## 2. Project Impact
The model provides critical insights into what makes a borrower profile risky. With its strong performance in distinguishing between high-risk and low-risk customers, the model **reduces the throughput time of a credit review by 25%** and **enhances the consistency** of credit decision-making.


## 3. Technical Skills Demonstrated
- **Programming**: Python (Pandas, NumPy, Scikit-learn)
- **Machine Learning**: Logistic Regression, Random Forest
- **Evaluation**: ROC-AUC Score, G-mean, Brier Score
  
## 4. Data
- **Source**: Confidential data provided by Royal FrieslandCampina
- **Size**: 631 customers, 22 features.

## 5. Project Workflow
### 5.1 Data Collection
- Identify and gather data from SAP ERP and a REST API
### 5.2 Data Understanding
- Imbalanced dataset
### 5.3 Data Cleaning and Preprocessing
### 5.4 Feature Engineering
- Variables for trend analysis: Standardized variations in revenues, net profit, working capital, and equity over a 3-year period
- Key financial ratios: Current ratio, DSO ratio, Operating Profit Margin & ...
- Interaction variables
  ### 5.5 Modelling
- Four Models:
  1. Logistic Regession using tree-based feature selection 
  2. Logistic Regression using Recursive Feature Elimination (RFE)
  3. SMOTE + Random Forest Classifier
  4. SMOTE-ENN + Random Forest Classifier

## 6. Results
- Random Forest Classifier performs worse than the traditional Logistic Regression when features are selected using RFE techniques.
- Best model Logistic Regression using RFE has a ROC-AUC Score of 0.89 with a standard deviation of 0.04 using 200 Bootstrap samples.
