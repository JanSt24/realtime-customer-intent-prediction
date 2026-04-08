# realtime-customer-intent-prediction
Machine learning model predicting purchase intent at the start of a webshop session using real user‑behavior logs. Enables cost‑efficient targeting by offering discounts only to non‑buyers, increasing conversions while reducing unnecessary incentive spend. Includes data prep, modeling, and business impact analysis.  

# Predicting Purchase Intent in an E‑Commerce Webshop (TradeSphere Case Study)
 
This project combines **Tableau Prep** for data preparation and **Orange Data Mining** for model training and evaluation. The goal is to predict **purchase intent at the start of a webshop session**, enabling TradeSphere to target incentives only to users unlikely to buy.
 
---
 
## Business Problem
 
TradeSphere offers a **5 CHF incentive** to users who are unlikely to buy.  
The incentive converts **30% of non‑buyers into buyers**, but offering it to users who would buy anyway leads to unnecessary costs.
 
**Objective:**  
Predict purchase intent early to **avoid wasted incentives** and **increase revenue** from low‑intent users.
 
---
 
## Data Preparation in Tableau Prep
 
All preprocessing steps were performed in **Tableau Prep**, including:
 
### Data Cleaning & Standardization
- Converting data types  
- Fixing inconsistent values  
- Removing incomplete or unusable entries  
 
###  Feature Engineering
New, more informative attributes were created to improve prediction quality.  
These features capture user behavior, session characteristics, and interaction patterns.
 
###  Removal of Irrelevant Fields
Attributes that did not contribute to predictive performance were removed.  
This reduced noise, improved model accuracy, and simplified the dataset.
 
The final, cleaned dataset was exported for modeling in Orange.
 
---
 
##  Modeling in Orange
 
Several machine learning models were tested in **Orange**, including:
- Logistic Regression  
- Random Forest  
- Gradient Boosting  
- Naive Bayes  
- k‑Nearest Neighbors  
 
**Final model:** Gradient Boosting  
Chosen for:
- Strong performance on imbalanced data  
- Ability to capture non‑linear relationships  
- Clear feature importance insights  
 
Additional techniques:
- Oversampling / undersampling  
- Regularization  
- Cross‑validation  
- Cost‑sensitive evaluation  
 
---
 
##  Evaluation Strategy
 
Evaluation metric: **AUC**, ideal for imbalanced classification.  
Validation method: **k‑fold cross‑validation** in Orange.
 
Results:
- AUC: *[insert your value]*  
- Precision/Recall: *[insert]*  
- Confusion matrix: *[insert]*  
 
---
 
##  Business Impact
 
The model enables:
- **Reduced incentive waste** by avoiding discounts for high‑intent users  
- **Higher conversion rates** among low‑intent users  
- **Improved ROI** on marketing spend  
- **Real‑time personalization** at session start  
 
Example impact (hypothetical):
- 20% fewer unnecessary discounts  
- 30% uplift among low‑intent users  
- Significant margin improvement per 1,000 sessions  
 
---
 
## Tech Stack
- **Excel** (initial cleaning, CSV handling)
- **Tableau Prep** (data cleaning, feature engineering)  
- **Orange Data Mining** (modeling, evaluation, visualization)  
