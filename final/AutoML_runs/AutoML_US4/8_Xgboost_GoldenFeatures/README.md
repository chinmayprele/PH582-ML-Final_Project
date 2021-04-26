# Summary of 8_Xgboost_GoldenFeatures

[<< Go back](../README.md)


## Extreme Gradient Boosting (Xgboost)
- **n_jobs**: -1
- **objective**: binary:logistic
- **eta**: 0.075
- **max_depth**: 8
- **min_child_weight**: 5
- **subsample**: 1.0
- **colsample_bytree**: 1.0
- **eval_metric**: logloss
- **explain_level**: 2

## Validation
 - **validation_type**: kfold
 - **k_folds**: 5
 - **shuffle**: True
 - **stratify**: True
 - **random_seed**: 1230

## Optimized metric
logloss

## Training time

35.9 seconds

## Metric details
|           |    score |    threshold |
|:----------|---------:|-------------:|
| logloss   | 0.116867 | nan          |
| auc       | 0.990054 | nan          |
| f1        | 0.964371 |   0.578798   |
| accuracy  | 0.964623 |   0.578798   |
| precision | 1        |   0.975077   |
| recall    | 1        |   0.00156717 |
| mcc       | 0.929338 |   0.578798   |


## Confusion matrix (at threshold=0.578798)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     206 |                       6 |
| Labeled as positive |                       9 |                     203 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

## SHAP Importance
![SHAP Importance](shap_importance.png)

## SHAP Dependence plots

### Dependence (Fold 1)
![SHAP Dependence from Fold 1](learner_fold_0_shap_dependence.png)
### Dependence (Fold 2)
![SHAP Dependence from Fold 2](learner_fold_1_shap_dependence.png)
### Dependence (Fold 3)
![SHAP Dependence from Fold 3](learner_fold_2_shap_dependence.png)
### Dependence (Fold 4)
![SHAP Dependence from Fold 4](learner_fold_3_shap_dependence.png)
### Dependence (Fold 5)
![SHAP Dependence from Fold 5](learner_fold_4_shap_dependence.png)

## SHAP Decision plots

### Top-10 Worst decisions for class 0 (Fold 1)
![SHAP worst decisions class 0 from Fold 1](learner_fold_0_shap_class_0_worst_decisions.png)
### Top-10 Worst decisions for class 0 (Fold 2)
![SHAP worst decisions class 0 from Fold 2](learner_fold_1_shap_class_0_worst_decisions.png)
### Top-10 Worst decisions for class 0 (Fold 3)
![SHAP worst decisions class 0 from Fold 3](learner_fold_2_shap_class_0_worst_decisions.png)
### Top-10 Worst decisions for class 0 (Fold 4)
![SHAP worst decisions class 0 from Fold 4](learner_fold_3_shap_class_0_worst_decisions.png)
### Top-10 Worst decisions for class 0 (Fold 5)
![SHAP worst decisions class 0 from Fold 5](learner_fold_4_shap_class_0_worst_decisions.png)
### Top-10 Best decisions for class 0 (Fold 1)
![SHAP best decisions class 0 from Fold 1](learner_fold_0_shap_class_0_best_decisions.png)
### Top-10 Best decisions for class 0 (Fold 2)
![SHAP best decisions class 0 from Fold 2](learner_fold_1_shap_class_0_best_decisions.png)
### Top-10 Best decisions for class 0 (Fold 3)
![SHAP best decisions class 0 from Fold 3](learner_fold_2_shap_class_0_best_decisions.png)
### Top-10 Best decisions for class 0 (Fold 4)
![SHAP best decisions class 0 from Fold 4](learner_fold_3_shap_class_0_best_decisions.png)
### Top-10 Best decisions for class 0 (Fold 5)
![SHAP best decisions class 0 from Fold 5](learner_fold_4_shap_class_0_best_decisions.png)
### Top-10 Worst decisions for class 1 (Fold 1)
![SHAP worst decisions class 1 from Fold 1](learner_fold_0_shap_class_1_worst_decisions.png)
### Top-10 Worst decisions for class 1 (Fold 2)
![SHAP worst decisions class 1 from Fold 2](learner_fold_1_shap_class_1_worst_decisions.png)
### Top-10 Worst decisions for class 1 (Fold 3)
![SHAP worst decisions class 1 from Fold 3](learner_fold_2_shap_class_1_worst_decisions.png)
### Top-10 Worst decisions for class 1 (Fold 4)
![SHAP worst decisions class 1 from Fold 4](learner_fold_3_shap_class_1_worst_decisions.png)
### Top-10 Worst decisions for class 1 (Fold 5)
![SHAP worst decisions class 1 from Fold 5](learner_fold_4_shap_class_1_worst_decisions.png)
### Top-10 Best decisions for class 1 (Fold 1)
![SHAP best decisions class 1 from Fold 1](learner_fold_0_shap_class_1_best_decisions.png)
### Top-10 Best decisions for class 1 (Fold 2)
![SHAP best decisions class 1 from Fold 2](learner_fold_1_shap_class_1_best_decisions.png)
### Top-10 Best decisions for class 1 (Fold 3)
![SHAP best decisions class 1 from Fold 3](learner_fold_2_shap_class_1_best_decisions.png)
### Top-10 Best decisions for class 1 (Fold 4)
![SHAP best decisions class 1 from Fold 4](learner_fold_3_shap_class_1_best_decisions.png)
### Top-10 Best decisions for class 1 (Fold 5)
![SHAP best decisions class 1 from Fold 5](learner_fold_4_shap_class_1_best_decisions.png)

[<< Go back](../README.md)
