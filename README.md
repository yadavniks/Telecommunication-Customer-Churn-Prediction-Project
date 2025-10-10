# 📞 Telecommunication Customer Churn Prediction

## 🧠 Project Overview
This project focuses on analyzing a **telecommunication company’s customer data** to predict customer **churn** — the likelihood that a customer will stop using the company’s services.  
By building a predictive machine learning model, the company can identify customers who are likely to leave and take proactive steps to **improve retention and reduce losses**.

## 🎯 Objectives
- Identify key factors influencing customer churn.
- Build a predictive model to classify churn vs. non-churn customers.
- Provide actionable insights to help reduce churn rate.

## 📊 Dataset Description
The dataset contains information about telecom customers and their usage behavior.

account.length: how long the account has been active.
 voice.plan: yes or no, voicemail plan.
 voice.messages: number of voicemail messages.
 intl.plan: yes or no, international plan.
 intl.mins: minutes customer used service to make international calls.
 intl.calls: total number of international calls.
 intl.charge: total international charge.
 day.mins: minutes customer used service during the day.
 day.calls: total number of calls during the day.
 day.charge: total charge during the day.
 eve.mins: minutes customer used service during the evening.
 eve.calls: total number of calls during the evening.
 eve.charge: total charge during the evening.
 night.mins: minutes customer used service during the night.
 night.calls: total number of calls during the night.
 night.charge: total charge during the night.
 customer.calls: number of calls to customer service.
churn: Categorical, yes or no. Indicator of whether the customer has left the company (yes or no).

## ⚙️ Steps Involved

### 1. Data Collection
- Imported telecom dataset from a CSV file.
- Loaded and inspected data using **pandas**.

### 2. Data Cleaning & Preprocessing
- Handled missing values and duplicates.
- Encoded categorical variables using **LabelEncoder** and **OneHotEncoder**.
- Scaled numerical features for model efficiency.

### 3. Exploratory Data Analysis (EDA)
- Visualized churn distribution and feature relationships using:
  - **Matplotlib** and **Seaborn**
- Found important churn indicators:
  - Short tenure
  - Month-to-month contracts
  - High monthly charges

### 4. Model Building
- Applied classification algorithms:  
  - Random Forest  
  - xgBoost 

### 5. Model Evaluation
- Evaluated models using metrics:
  - Accuracy  
  - Precision  
  - Recall  
  - F1-Score  
  - Confusion Matrix  

### 6. Results
out of 667/566 are non churn customers
out of 667/101 are churn customers
so the accuarcy is 98% which is an excellent model
so here we applied xg boost algorithm to increase the accuracy more 
when we used random forest we got 97%  but here we get 98% so it is better algorithm.

## 🧩 Tools & Technologies Used
- **Programming Language:** Python  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn  
- **Environment:** Jupyter Notebook / Google Colab  

## 📈 Key Insights
- Customers with **month-to-month contracts** and **higher monthly charges** are more likely to churn.
- Long-term contracts and discounts can improve customer retention.
- Providing better support and loyalty programs helps reduce churn.

## 💡 Conclusion
The model helps telecom companies **predict and prevent customer churn** effectively.  
Using this predictive approach, businesses can focus their retention efforts on at-risk customers and improve overall profitability.

## 🧰 How to Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/telecom-churn-prediction.git
