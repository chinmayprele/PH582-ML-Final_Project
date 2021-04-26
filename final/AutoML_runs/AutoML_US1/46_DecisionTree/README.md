# Summary of 46_DecisionTree

[<< Go back](../README.md)


## Decision Tree
- **n_jobs**: -1
- **criterion**: entropy
- **max_depth**: 2
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

24.4 seconds

## Metric details
|           |    score |    threshold |
|:----------|---------:|-------------:|
| logloss   | 0.344876 | nan          |
| auc       | 0.958293 | nan          |
| f1        | 0.917808 |   0.503311   |
| accuracy  | 0.915094 |   0.503311   |
| precision | 0.970414 |   0.970588   |
| recall    | 1        |   0.00596026 |
| mcc       | 0.832005 |   0.503311   |


## Confusion matrix (at threshold=0.503311)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     187 |                      25 |
| Labeled as positive |                      11 |                     201 |

## Learning curves
![Learning curves](learning_curves.png)

## Decision Tree 

### Tree #1
![Tree 1](learner_fold_0_tree.svg)

### Rules

if (concave points_worst <= 0.109) and (area_mean <= 694.5) then class: 0 (proba: 99.32%) | based on 146 samples

if (concave points_worst > 0.109) and (perimeter_worst > 115.35) then class: 1 (proba: 100.0%) | based on 130 samples

if (concave points_worst > 0.109) and (perimeter_worst <= 115.35) then class: 1 (proba: 61.11%) | based on 54 samples

if (concave points_worst <= 0.109) and (area_mean > 694.5) then class: 1 (proba: 66.67%) | based on 9 samples




### Tree #2
![Tree 2](learner_fold_1_tree.svg)

### Rules

if (area_worst <= 868.2) and (concave points_worst <= 0.132) then class: 0 (proba: 96.95%) | based on 164 samples

if (area_worst > 868.2) and (concavity_se > 0.019) then class: 1 (proba: 100.0%) | based on 135 samples

if (area_worst <= 868.2) and (concave points_worst > 0.132) then class: 1 (proba: 75.0%) | based on 28 samples

if (area_worst > 868.2) and (concavity_se <= 0.019) then class: 1 (proba: 75.0%) | based on 12 samples




### Tree #3
![Tree 3](learner_fold_2_tree.svg)

### Rules

if (concave points_worst <= 0.142) and (area_worst <= 947.6) then class: 0 (proba: 94.83%) | based on 174 samples

if (concave points_worst > 0.142) and (perimeter_worst > 112.8) then class: 1 (proba: 100.0%) | based on 127 samples

if (concave points_worst > 0.142) and (perimeter_worst <= 112.8) then class: 1 (proba: 80.95%) | based on 21 samples

if (concave points_worst <= 0.142) and (area_worst > 947.6) then class: 1 (proba: 94.12%) | based on 17 samples




### Tree #4
![Tree 4](learner_fold_3_tree.svg)

### Rules

if (perimeter_worst <= 102.4) and (concave points_worst <= 0.133) then class: 0 (proba: 99.34%) | based on 151 samples

if (perimeter_worst > 102.4) and (perimeter_worst > 115.45) then class: 1 (proba: 100.0%) | based on 136 samples

if (perimeter_worst > 102.4) and (perimeter_worst <= 115.45) then class: 1 (proba: 59.52%) | based on 42 samples

if (perimeter_worst <= 102.4) and (concave points_worst > 0.133) then class: 1 (proba: 70.0%) | based on 10 samples




### Tree #5
![Tree 5](learner_fold_4_tree.svg)

### Rules

if (concave points_worst <= 0.142) and (area_worst <= 929.8) then class: 0 (proba: 95.38%) | based on 173 samples

if (concave points_worst > 0.142) and (area_worst > 710.2) then class: 1 (proba: 100.0%) | based on 137 samples

if (concave points_worst <= 0.142) and (area_worst > 929.8) then class: 1 (proba: 90.48%) | based on 21 samples

if (concave points_worst > 0.142) and (area_worst <= 710.2) then class: 1 (proba: 66.67%) | based on 9 samples





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
