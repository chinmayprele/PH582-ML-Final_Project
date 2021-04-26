# Summary of 35_DecisionTree

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

26.3 seconds

## Metric details
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.205083 | nan         |
| auc       | 0.967404 | nan         |
| f1        | 0.944444 |   0.407395  |
| accuracy  | 0.943396 |   0.407395  |
| precision | 0.947619 |   0.509411  |
| recall    | 1        |   0.0116129 |
| mcc       | 0.887425 |   0.407395  |


## Confusion matrix (at threshold=0.407395)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     196 |                      16 |
| Labeled as positive |                       8 |                     204 |

## Learning curves
![Learning curves](learning_curves.png)

## Decision Tree 

### Tree #1
![Tree 1](learner_fold_0_tree.svg)

### Rules

if (perimeter_worst <= 104.95) and (concave points_worst <= 0.135) then class: 0 (proba: 98.71%) | based on 155 samples

if (perimeter_worst > 104.95) and (concave points_worst > 0.151) then class: 1 (proba: 100.0%) | based on 126 samples

if (perimeter_worst > 104.95) and (concave points_worst <= 0.151) then class: 1 (proba: 71.74%) | based on 46 samples

if (perimeter_worst <= 104.95) and (concave points_worst > 0.135) then class: 1 (proba: 66.67%) | based on 12 samples




### Tree #2
![Tree 2](learner_fold_1_tree.svg)

### Rules

if (perimeter_worst <= 104.95) and (concave points_worst <= 0.135) then class: 0 (proba: 98.71%) | based on 155 samples

if (perimeter_worst > 104.95) and (concave points_worst > 0.151) then class: 1 (proba: 100.0%) | based on 121 samples

if (perimeter_worst > 104.95) and (concave points_worst <= 0.151) then class: 1 (proba: 73.47%) | based on 49 samples

if (perimeter_worst <= 104.95) and (concave points_worst > 0.135) then class: 1 (proba: 71.43%) | based on 14 samples




### Tree #3
![Tree 3](learner_fold_2_tree.svg)

### Rules

if (concave points_mean <= 0.051) and (radius_worst <= 16.83) then class: 0 (proba: 97.47%) | based on 158 samples

if (concave points_mean > 0.051) and (concavity_worst > 0.226) then class: 1 (proba: 98.71%) | based on 155 samples

if (concave points_mean <= 0.051) and (radius_worst > 16.83) then class: 1 (proba: 64.71%) | based on 17 samples

if (concave points_mean > 0.051) and (concavity_worst <= 0.226) then class: 0 (proba: 77.78%) | based on 9 samples




### Tree #4
![Tree 4](learner_fold_3_tree.svg)

### Rules

if (concave points_worst <= 0.135) and (radius_worst <= 16.8) then class: 0 (proba: 96.99%) | based on 166 samples

if (concave points_worst > 0.135) and (concave points_worst > 0.151) then class: 1 (proba: 100.0%) | based on 138 samples

if (concave points_worst <= 0.135) and (radius_worst > 16.8) then class: 1 (proba: 78.95%) | based on 19 samples

if (concave points_worst > 0.135) and (concave points_worst <= 0.151) then class: 1 (proba: 75.0%) | based on 16 samples




### Tree #5
![Tree 5](learner_fold_4_tree.svg)

### Rules

if (concave points_mean > 0.051) and (concavity_worst > 0.223) then class: 1 (proba: 99.35%) | based on 154 samples

if (concave points_mean <= 0.051) and (area_worst <= 766.45) then class: 0 (proba: 98.01%) | based on 151 samples

if (concave points_mean <= 0.051) and (area_worst > 766.45) then class: 0 (proba: 53.85%) | based on 26 samples

if (concave points_mean > 0.051) and (concavity_worst <= 0.223) then class: 0 (proba: 77.78%) | based on 9 samples





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
