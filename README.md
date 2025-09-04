📊 Customer Product Analysis

📌 Project Overview
This project analyzes the Bank Marketing dataset (UCI) to identify factors influencing the subscription of term deposits. The bank currently faces a low subscription rate (~11%) with high outbound calling costs. This project combines EDA, feature engineering, logistic regression modeling, and cost–benefit analysis to provide actionable recommendations.

📂 Project Structure

Customer-Product-Analysis/

│

├── data/                       Raw dataset (bank-additional-full.csv)

├── notebooks/                  Colab notebooks with code

│   └── analysis.ipynb

├── reports/                   

│   └── REPORT.pdf              Full business report with insights

├── requirements.txt           

└── README.md         

🗂 Dataset

Source: UCI Bank Marketing Dataset

Rows: 41,188

Features: demographics, contact history, campaign details, macroeconomic conditions

Target: y → whether the client subscribed (yes/no)

🔎 Methodology

EDA: 

Distribution of age & campaign contacts

Subscription rate by occupation, education, and channel

Impact of macroeconomic indicators

Feature Engineering:

Age grouping

Capping extreme campaign values

Encoding categorical features

Modeling:

Logistic Regression with class balancing

Train/test split (70/30, stratified)

Evaluation:

Accuracy = 0.7876

ROC AUC = 0.7767

Confusion Matrix & Classification Report

Cost–Benefit Analysis:

Precision (subscribers) = 30% → ~3.3 calls per successful subscription

Break-even: revenue per subscriber R > 3.275 × Ccall

📊 Key Insights

Class imbalance: only ~11.3% subscribe → campaigns must be highly targeted.

Demographics: students & retirees subscribe more; blue-collar & services less.

Education: higher education strongly correlates with subscription.

Contact history: prior successful outcomes predict higher conversion.

Channel: mobile (cellular) outperforms landline.

Campaign fatigue: more calls → lower success.

Macroeconomic factors: subscription likelihood is sensitive to employment and inflation.

💡 Recommendations

Leverage prior successful contacts → retargeting priority.

Segment by age/occupation → personalize for retirees (safety) vs. students (savings).

Optimize calling strategy → max 3 calls per customer.

Prioritize mobile over landline.

#Adjust to economic cycles → align campaigns with favorable conditions.

#🚀 Extended Analysis (Future Work)

Address class imbalance with advanced methods (SMOTE, cost-sensitive learning).

Explore Decision Trees / Ensembles (XGBoost, LightGBM).

Apply Uplift Modeling to capture true causal impact.

Calibrate probabilities to optimize profit thresholds.

🛠 Tech Stack

Python: pandas, numpy

Visualization: matplotlib, seaborn

Modeling: scikit-learn (Logistic Regression, evaluation metrics)

📌 Author

👤 Phan Thi Dinh

📧 Contact: [phandinh0308@gmail.com]
