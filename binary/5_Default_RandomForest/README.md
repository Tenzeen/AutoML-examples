# Summary of 5_Default_RandomForest

[<< Go back](../README.md)


## Random Forest
- **n_jobs**: -1
- **criterion**: gini
- **max_features**: 0.9
- **min_samples_split**: 30
- **max_depth**: 4
- **eval_metric_name**: logloss
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

33.7 seconds

### Metric details
|           |    0 to 17 |   18 to 29 |   30 to 49 |    50 to 69 |   70 or Older |   accuracy |   macro avg |   weighted avg |   logloss |
|:----------|-----------:|-----------:|-----------:|------------:|--------------:|-----------:|------------:|---------------:|----------:|
| precision |   1        |   0.547085 |   0.484404 |    0.434917 |      0.690106 |   0.593849 |    0.631302 |       0.610558 |  0.947229 |
| recall    |   0.647416 |   0.266376 |   0.308051 |    0.573171 |      0.909762 |   0.593849 |    0.540955 |       0.593849 |  0.947229 |
| f1-score  |   0.785978 |   0.358297 |   0.376605 |    0.494563 |      0.784855 |   0.593849 |    0.56006  |       0.580976 |  0.947229 |
| support   | 658        | 458        | 857        | 1230        |   1219        |   0.593849 | 4422        |    4422        |  0.947229 |


## Confusion matrix
|                        |   Predicted as 0 to 17 |   Predicted as 18 to 29 |   Predicted as 30 to 49 |   Predicted as 50 to 69 |   Predicted as 70 or Older |
|:-----------------------|-----------------------:|------------------------:|------------------------:|------------------------:|---------------------------:|
| Labeled as 0 to 17     |                    426 |                       4 |                      33 |                     194 |                          1 |
| Labeled as 18 to 29    |                      0 |                     122 |                     151 |                     178 |                          7 |
| Labeled as 30 to 49    |                      0 |                      97 |                     264 |                     439 |                         57 |
| Labeled as 50 to 69    |                      0 |                       0 |                      92 |                     705 |                        433 |
| Labeled as 70 or Older |                      0 |                       0 |                       5 |                     105 |                       1109 |

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
