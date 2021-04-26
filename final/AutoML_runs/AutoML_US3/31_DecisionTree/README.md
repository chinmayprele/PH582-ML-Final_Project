# Summary of 31_DecisionTree

[<< Go back](../README.md)


## Decision Tree
- **n_jobs**: -1
- **criterion**: gini
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

26.2 seconds

## Metric details
|           |    score |    threshold |
|:----------|---------:|-------------:|
| logloss   | 0.305727 | nan          |
| auc       | 0.945866 | nan          |
| f1        | 0.930233 |   0.493871   |
| accuracy  | 0.929245 |   0.493871   |
| precision | 0.947368 |   0.996667   |
| recall    | 1        |   0.00584416 |
| mcc       | 0.858835 |   0.493871   |


## Confusion matrix (at threshold=0.493871)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     194 |                      18 |
| Labeled as positive |                      12 |                     200 |

## Learning curves
![Learning curves](learning_curves.png)

## Decision Tree 

### Tree #1
![Tree 1](learner_fold_0_tree.svg)

### Rules

if (perimeter_worst <= 105.95) and (concave points_worst <= 0.142) then class: 0 (proba: 97.53%) | based on 162 samples

if (perimeter_worst > 105.95) and (concave points_mean > 0.047) then class: 1 (proba: 98.67%) | based on 150 samples

if (perimeter_worst > 105.95) and (concave points_mean <= 0.047) then class: 1 (proba: 60.0%) | based on 15 samples

if (perimeter_worst <= 105.95) and (concave points_worst > 0.142) then class: 1 (proba: 75.0%) | based on 12 samples




### Tree #2
![Tree 2](learner_fold_1_tree.svg)

### Rules

if (perimeter_worst <= 107.45) and (concave points_worst <= 0.134) then class: 0 (proba: 98.12%) | based on 160 samples

if (perimeter_worst > 107.45) and (texture_mean > 15.375) then class: 1 (proba: 99.33%) | based on 150 samples

if (perimeter_worst <= 107.45) and (concave points_worst > 0.134) then class: 1 (proba: 71.43%) | based on 21 samples

if (perimeter_worst > 107.45) and (texture_mean <= 15.375) then class: 0 (proba: 62.5%) | based on 8 samples




### Tree #3
![Tree 3](learner_fold_2_tree.svg)

### Rules

if (perimeter_worst <= 106.1) and (concave points_worst <= 0.135) then class: 0 (proba: 99.35%) | based on 154 samples

if (perimeter_worst > 106.1) and (perimeter_worst > 114.45) then class: 1 (proba: 100.0%) | based on 139 samples

if (perimeter_worst > 106.1) and (perimeter_worst <= 114.45) then class: 1 (proba: 60.71%) | based on 28 samples

if (perimeter_worst <= 106.1) and (concave points_worst > 0.135) then class: 1 (proba: 66.67%) | based on 18 samples




### Tree #4
![Tree 4](learner_fold_3_tree.svg)

### Rules

if (concave points_mean > 0.045) and (area_worst > 710.2) then class: 1 (proba: 96.23%) | based on 159 samples

if (concave points_mean <= 0.045) and (area_worst <= 839.85) then class: 0 (proba: 97.45%) | based on 157 samples

if (concave points_mean > 0.045) and (area_worst <= 710.2) then class: 0 (proba: 66.67%) | based on 15 samples

if (concave points_mean <= 0.045) and (area_worst > 839.85) then class: 1 (proba: 87.5%) | based on 8 samples




### Tree #5
![Tree 5](learner_fold_4_tree.svg)

### Rules

if (perimeter_worst <= 106.1) and (symmetry_worst <= 0.362) then class: 0 (proba: 95.83%) | based on 168 samples

if (perimeter_worst > 106.1) and (texture_mean > 15.535) then class: 1 (proba: 98.06%) | based on 155 samples

if (perimeter_worst > 106.1) and (texture_mean <= 15.535) then class: 0 (proba: 50.0%) | based on 12 samples

if (perimeter_worst <= 106.1) and (symmetry_worst > 0.362) then class: 1 (proba: 100.0%) | based on 5 samples





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
