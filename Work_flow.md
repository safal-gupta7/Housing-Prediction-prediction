1. Clean dataset                 ← do this properly
        ↓
2. Exploratory Data Analysis
        ↓
3. Train/validation split
        ↓
4. Linear Regression             ← you are here
        ↓
5. Evaluate on validation data   ← NEXT
        ↓
6. Understand under/overfitting
        ↓
7. Feature engineering
        ↓
8. Ridge / Lasso
        ↓
9. Decision Tree
        ↓
10. Random Forest
        ↓
11. Gradient Boosting
        ↓
12. Cross-validation
        ↓
13. Hyperparameter tuning
        ↓
14. Select final model
        ↓
15. Train on all training data
        ↓
16. Predict test.csv
        ↓
17. Create submission.csv





1. Dataset structure
       ↓
2. Missing values
       ↓
3. Duplicate values
       ↓
4. Histograms ← YOU ARE HERE
       ↓
5. Outlier analysis
       ↓
6. Feature ↔ target relationships
       ↓
7. Feature ↔ feature correlations
       ↓
8. Decide preprocessing
       ↓
9. Train/test split
       ↓
10. Baseline model
       ↓
11. Evaluate
       ↓
12. Improve/tune


| Column | Meaning | What it contains |
|---|---|---|
| `CRIM` | Crime rate | Per-capita crime rate in the area |
| `ZN` | Residential land | Percentage of land zoned for lots over 25,000 sq. ft. |
| `INDUS` | Industrial land | Percentage of land used for non-retail business/industry |
| `CHAS` | Charles River | Whether the area borders the Charles River: `1` = yes, `0` = no |
| `NOX` | Nitric oxide | Concentration of nitrogen oxides in the area |
| `RM` | Average rooms | Average number of rooms per dwelling |
| `AGE` | Old buildings | Percentage of owner-occupied homes built before 1940 |
| `DIS` | Distance | Weighted distance to major employment centers |
| `RAD` | Highway accessibility | Index of accessibility to radial highways |
| `TAX` | Property tax | Property-tax rate per $10,000 |
| `PTRATIO` | Student-teacher ratio | Pupil-teacher ratio in the area |
| `B` | Demographic transformation | A transformed measure based on the proportion of Black residents |
| `LSTAT` | Lower socioeconomic status | Percentage of the population classified as lower socioeconomic status |
| `MEDV` | House value | Median value of owner-occupied homes, in $1,000s |


**Recommanded workflow for the choosing the best model **

                    YOUR DATA
                        │
                        ▼
               Train / Validation split
                        │
          ┌─────────────┴─────────────┐
          ▼                           ▼
    Training data                Validation data
          │                           │
          ▼                           │
   ┌─────────────────┐                │
   │ Baseline models │                │
   ├─────────────────┤                │
   │Linear Regression│                │
   │Decision Tree    │                │
   │Random Forest    │                │
   │XGBoost          │                │
   └────────┬────────┘                │
            ▼                         │
      Compare validation              │
         performance                  │
            │                         │
            ▼                         │
     Select promising model(s)        │
            │                         │
            ▼                         │
      GridSearchCV / tuning           │
            │                         │
            ▼                         │
       Tuned model                    │
            │                         │
            └──────────────► Validation
                              evaluation