# Summary of 3_Default_Xgboost

[<< Go back](../README.md)


## Extreme Gradient Boosting (Xgboost)
- **n_jobs**: -1
- **objective**: multi:softprob
- **eta**: 0.075
- **max_depth**: 6
- **min_child_weight**: 1
- **subsample**: 1.0
- **colsample_bytree**: 1.0
- **eval_metric**: mlogloss
- **num_class**: 5
- **explain_level**: 2

## Validation
 - **validation_type**: split
 - **train_ratio**: 0.75
 - **shuffle**: True
 - **stratify**: True

## Optimized metric
logloss

## Training time

60.9 seconds

### Metric details
|           |    0 to 17 |   18 to 29 |   30 to 49 |    50 to 69 |   70 or Older |   accuracy |   macro avg |   weighted avg |   logloss |
|:----------|-----------:|-----------:|-----------:|------------:|--------------:|-----------:|------------:|---------------:|----------:|
| precision |   0.890017 |   0.506623 |   0.49328  |    0.517715 |      0.734665 |   0.631389 |    0.62846  |       0.627035 |  0.817724 |
| recall    |   0.799392 |   0.334061 |   0.428238 |    0.582114 |      0.844955 |   0.631389 |    0.597752 |       0.631389 |  0.817724 |
| f1-score  |   0.842274 |   0.402632 |   0.458463 |    0.548029 |      0.78596  |   0.631389 |    0.607472 |       0.624985 |  0.817724 |
| support   | 658        | 458        | 857        | 1230        |   1219        |   0.631389 | 4422        |    4422        |  0.817724 |


## Confusion matrix
|                        |   Predicted as 0 to 17 |   Predicted as 18 to 29 |   Predicted as 30 to 49 |   Predicted as 50 to 69 |   Predicted as 70 or Older |
|:-----------------------|-----------------------:|------------------------:|------------------------:|------------------------:|---------------------------:|
| Labeled as 0 to 17     |                    526 |                      12 |                      50 |                      68 |                          2 |
| Labeled as 18 to 29    |                     20 |                     153 |                     184 |                      96 |                          5 |
| Labeled as 30 to 49    |                     26 |                     115 |                     367 |                     320 |                         29 |
| Labeled as 50 to 69    |                     18 |                      21 |                     139 |                     716 |                        336 |
| Labeled as 70 or Older |                      1 |                       1 |                       4 |                     183 |                       1030 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)
## Confusion Matrix

![Confusion Matrix](confusion_matrix.png)


## Normalized Confusion Matrix

![Normalized Confusion Matrix](confusion_matrix_normalized.png)


## ROC Curve

![ROC Curve](roc_curve.png)


## Precision Recall Curve

![Precision Recall Curve](precision_recall_curve.png)



## SHAP Importance
![SHAP Importance](shap_importance.png)

## SHAP Dependence plots

### Dependence 0 to 17 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_0 to 17.png)
### Dependence 18 to 29 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_18 to 29.png)
### Dependence 30 to 49 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_30 to 49.png)
### Dependence 50 to 69 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_50 to 69.png)
### Dependence 70 or Older (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_70 or Older.png)

## SHAP Decision plots

### Worst decisions for selected sample 1 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_0_worst_decisions.png)
### Worst decisions for selected sample 2 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_1_worst_decisions.png)
### Worst decisions for selected sample 3 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_2_worst_decisions.png)
### Worst decisions for selected sample 4 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_3_worst_decisions.png)
### Best decisions for selected sample 1 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_0_best_decisions.png)
### Best decisions for selected sample 2 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_1_best_decisions.png)
### Best decisions for selected sample 3 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_2_best_decisions.png)
### Best decisions for selected sample 4 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_3_best_decisions.png)

[<< Go back](../README.md)
