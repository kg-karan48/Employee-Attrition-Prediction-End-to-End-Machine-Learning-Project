Employee Attrition Prediction End to End Machine Learning Project


Employee attrition is a big problem for companies because when employees leave, it costs money, time, and affects team performance. 
I worked on this project to understand why employees leave and to build a machine learning model that can predict attrition in advance.
The main goal of this project was not just to build a model, but also to understand the real factors that influence employee decisions.


Understanding the Data :
I used an HR dataset that includes employee details like age, education, income, total working years, years at the company, job role, business travel, job satisfaction, and work-life balance.
The target variable was Attrition (Yes/No).
Before doing anything, I checked:
Shape of the dataset
Data types
Missing values
Basic statistics
This helped me understand how the data looks and what needs cleaning.


Exploratory Data Analysis (EDA)
After cleaning basic issues, I explored the data using visualizations.
Some interesting things I noticed:
Employees with lower monthly income were leaving more.
People who travel frequently for business had higher attrition.
Employees who stayed longer in the company were less likely to leave.
Better work-life balance reduced attrition chances.
I used histograms, count plots, boxplots, and correlation heatmaps to understand these patterns clearly.

Data Cleaning :
To prepare the data properly:
I filled missing numerical values using the median.
I filled missing categorical values using the most frequent value.
Removed duplicate rows.
Handled outliers using the IQR method for important numerical features.
This step was important to avoid misleading model results.


Statistical Testing :
I didn’t want to rely only on visual analysis, so I performed statistical tests to confirm my findings.
I used an independent t-test to check if salary actually impacts attrition.
I used a chi-square test to check the relationship between business travel and attrition.
The results showed that both salary and business travel have a statistically significant impact on attrition.
This gave more confidence in my analysis.


Feature Engineering :
Before building models:
I removed unnecessary columns like IDs.
Converted categorical variables using One-Hot Encoding.
Scaled numerical features using StandardScaler.
This made the data ready for machine learning algorithms.


Model Building :
I trained two models:
Logistic Regression (simple and interpretable)
Random Forest (to capture complex patterns)
Logistic Regression helped me understand feature importance clearly, while Random Forest gave better performance in handling non-linear relationships.


Model Evaluation :
I evaluated the models


Accuracy :
Precision, Recall, F1-score
Confusion Matrix
Random Forest performed better overall, but Logistic Regression was easier to interpret.


Model Saving :
Finally, I saved:
The trained model using pickle
The scaler used for preprocessing


Key Insights :
From this project, I learned that:
Lower income employees are more likely to leave.
Frequent business travel increases attrition risk.

Employees with longer tenure and better work-life balance are more stable.

These insights can help HR teams take preventive actions like improving salary structure, travel policies, or employee engagement programs.
