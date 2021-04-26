# Summary of 33_RandomForest

[<< Go back](../README.md)


## Random Forest
- **n_jobs**: -1
- **criterion**: entropy
- **max_features**: 0.7
- **min_samples_split**: 30
- **max_depth**: 6
- **eval_metric_name**: logloss
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

69.5 seconds

## Metric details
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.181781 |  nan        |
| auc       | 0.985237 |  nan        |
| f1        | 0.956322 |    0.396296 |
| accuracy  | 0.955189 |    0.396296 |
| precision | 1        |    0.997764 |
| recall    | 0.990566 |    0        |
| mcc       | 0.911605 |    0.396296 |


## Confusion matrix (at threshold=0.396296)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     197 |                      15 |
| Labeled as positive |                       4 |                     208 |

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
