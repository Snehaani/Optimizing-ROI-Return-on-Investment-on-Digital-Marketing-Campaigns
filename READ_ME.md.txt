# 📊 Optimizing ROI on Digital Marketing Campaigns

### *Predictive Modeling for Airline Product Uptake*

This project aims to build a robust machine learning model to predict which airline customers are most likely to take up a specific product. By analyzing customer engagement metrics such as comments, views, likes, and check-ins, the model helps optimize digital marketing campaigns and improve ROI.



## 🚀 Project Overview

Airlines generate massive engagement across digital touchpoints. This project leverages machine learning to analyze this data and identify high-potential customers for targeted marketing efforts.

The workflow includes:

* Exploratory Data Analysis (EDA)
* Data preprocessing & feature engineering
* Handling class imbalance with SMOTE
* Model building using Logistic Regression, Decision Tree & Random Forest
* Hyperparameter tuning with GridSearchCV
* Performance evaluation & cross-validation
* Saving final model for deployment

## 📁 Repository Structure


📦 project-folder
 ├── README.md  
 ├── EDA.ipynb  
 ├── Model_Building.ipynb  
 ├── final_model.pkl  
 ├── smote_object.pkl  
 

## 📚 Dataset Summary

The dataset includes:

| Feature                            | Description                                    |
| ---------------------------------- | ---------------------------------------------- |
| yearly_avg_comments                | Avg yearly comments on travel pages            |
| yearly_avg_views                   | Avg yearly views on travel pages               |
| total_likes_on_outstation_checkins | Likes on outstation check-ins                  |
| yearly_avg_outstation_checkins     | Avg outstation check-ins                       |
| member_in_family                   | Number of family members                       |
| **target**                         | Whether the customer took the product (Yes/No) |

**Class Imbalance:**

* Yes → 1,896
* No → 9,824
  Balanced using **SMOTE**.


## 🔍 Exploratory Data Analysis (EDA)

Key steps:

* Data cleaning & preprocessing
* Outlier detection
* Distribution & correlation analysis
* Feature understanding

Insights:

* Engagement features highly correlate with product uptake
* Likes, views, and comments are the strongest indicators


## 🤖 Machine Learning Models

Models tested:

* Logistic Regression
* Decision Tree Classifier
* **Random Forest Classifier — Best Model**

### 🏆 Random Forest Performance

| Metric    | No   | Yes  |
| --------- | ---- | ---- |
| Precision | 0.98 | 0.92 |
| Recall    | 0.98 | 0.89 |
| F1-Score  | 0.98 | 0.91 |

**Overall Accuracy:** 97%
**Cross-Validation:** Highly consistent results

Top Features:

1. total_likes_on_outstation_checkin_given
2. yearly_avg_view_on_travel_page
3. yearly_avg_comment_on_travel_page
4. yearly_avg_outstation_checkins
5. member_in_family


## 🛠 Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Imbalanced-Learn (SMOTE)
* Joblib
* Jupyter Notebook


## 💡 Business Value

* Improve targeting in digital marketing campaigns
* Increase conversion rate & ROI
* Understand customer engagement behavior
* Deployable ML model for prediction


## 🔮 Future Enhancements

* Add demographic & transactional features
* Use SHAP/LIME for better interpretability
* Build an automated ML pipeline
* Deploy as an API
* Monitor & retrain model periodically


## 👩‍💻 Author

**Sneha M**
MBA — Data Science
Jain University

