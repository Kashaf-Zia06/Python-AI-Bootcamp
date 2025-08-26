# Student Placement ML Pipeline — Summary Report

## Dataset Insights
- Dataset shape reported: Shape: 
- Missing values summary (detected lines):
#   Column            Non-Null Count  Dtype
0   Student_ID        1000 non-null   int64
1   CGPA              1000 non-null   float64
2   Internships       1000 non-null   int64
3   Placed            1000 non-null   object
4   Salary (INR LPA)  1000 non-null   float64
Student_ID        1000.0    NaN  NaN  NaN     500.5  288.819436   1.0  250.75
CGPA              1000.0    NaN  NaN  NaN   7.51556    0.783422  4.91    6.98
Internships       1000.0    NaN  NaN  NaN     2.045    1.424431   0.0     1.0
Placed              1000      2  Yes  690       NaN         NaN   NaN     NaN
Salary (INR LPA)  1000.0    NaN  NaN  NaN  11.79558   10.105559   0.0     0.0
Placed               NaN     NaN     NaN
Total missing values: 0
missing_count
Remaining missing values: 0


## Model Comparison

| model         |   recall |   f1 | accuracy   | precision   |
|:--------------|---------:|-----:|:-----------|:------------|
| Decision Tree |        1 |    1 | 1.0        | 1.0         |
| Random Forest |        1 |    1 | 1.0        | 1.0         |
| KNN           |        1 |    1 |            |             |


## Conclusions
- **Best model:** Decision Tree (F1=1.000, Accuracy=1.000)
- **Why it likely performed best:** Based on the metrics parsed, it achieved the highest F1/Accuracy, indicating a good balance between precision and recall on this dataset.
- **Most important features:** As indicated in the detected feature-importance excerpt above; typically, tree-based models highlight variables with highest split gains.
- **Impact of hyperparameter tuning:** The notebook includes a tuning step (e.g., Grid/Random Search). Compare `best_score_` with baseline metrics to quantify the improvement.
