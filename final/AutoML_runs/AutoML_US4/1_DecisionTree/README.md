# Summary of 1_DecisionTree

[<< Go back](../README.md)


## Decision Tree
- **n_jobs**: -1
- **criterion**: gini
- **max_depth**: 3
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

61.4 seconds

## Metric details
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.480966 |  nan        |
| auc       | 0.921146 |  nan        |
| f1        | 0.925234 |    0.5      |
| accuracy  | 0.924528 |    0.5      |
| precision | 0.925743 |    0.924513 |
| recall    | 0.985849 |    0        |
| mcc       | 0.849208 |    0.5      |


## Confusion matrix (at threshold=0.5)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     194 |                      18 |
| Labeled as positive |                      14 |                     198 |

## Learning curves
![Learning curves](learning_curves.png)

## Decision Tree 

### Tree #1
![Tree 1](learner_fold_0_tree.svg)

### Rules

if (perimeter_worst <= 106.05) and (concave points_worst <= 0.159) and (smoothness_worst <= 0.178) then class: 0 (proba: 96.84%) | based on 158 samples

if (perimeter_worst > 106.05) and (texture_mean > 15.37) and (smoothness_worst > 0.1) then class: 1 (proba: 97.4%) | based on 154 samples

if (perimeter_worst <= 106.05) and (concave points_worst > 0.159) and (texture_worst > 23.47) then class: 1 (proba: 100.0%) | based on 8 samples

if (perimeter_worst > 106.05) and (texture_mean <= 15.37) and (fractal_dimension_se <= 0.003) then class: 0 (proba: 100.0%) | based on 7 samples

if (perimeter_worst > 106.05) and (texture_mean > 15.37) and (smoothness_worst <= 0.1) then class: 0 (proba: 75.0%) | based on 4 samples

if (perimeter_worst > 106.05) and (texture_mean <= 15.37) and (fractal_dimension_se > 0.003) then class: 1 (proba: 100.0%) | based on 3 samples

if (perimeter_worst <= 106.05) and (concave points_worst <= 0.159) and (smoothness_worst > 0.178) then class: 1 (proba: 66.67%) | based on 3 samples

if (perimeter_worst <= 106.05) and (concave points_worst > 0.159) and (texture_worst <= 23.47) then class: 0 (proba: 100.0%) | based on 2 samples




### Tree #2
![Tree 2](learner_fold_1_tree.svg)

### Rules

if (perimeter_worst <= 105.05) and (smoothness_worst <= 0.178) and (symmetry_worst > 0.157) then class: 0 (proba: 96.3%) | based on 162 samples

if (perimeter_worst > 105.05) and (concave points_mean > 0.049) and (area_se > 14.18) then class: 1 (proba: 98.03%) | based on 152 samples

if (perimeter_worst > 105.05) and (concave points_mean <= 0.049) and (area_worst <= 949.85) then class: 0 (proba: 88.89%) | based on 9 samples

if (perimeter_worst > 105.05) and (concave points_mean <= 0.049) and (area_worst > 949.85) then class: 1 (proba: 87.5%) | based on 8 samples

if (perimeter_worst <= 105.05) and (smoothness_worst > 0.178) and (smoothness_se <= 0.012) then class: 1 (proba: 100.0%) | based on 5 samples

if (perimeter_worst > 105.05) and (concave points_mean > 0.049) and (area_se <= 14.18) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 105.05) and (smoothness_worst > 0.178) and (smoothness_se > 0.012) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 105.05) and (smoothness_worst <= 0.178) and (symmetry_worst <= 0.157) then class: 1 (proba: 100.0%) | based on 1 samples




### Tree #3
![Tree 3](learner_fold_2_tree.svg)

### Rules

if (concave points_worst > 0.116) and (area_worst > 710.2) and (concavity_worst > 0.208) then class: 1 (proba: 98.1%) | based on 158 samples

if (concave points_worst <= 0.116) and (area_mean <= 694.15) and (area_se <= 48.975) then class: 0 (proba: 99.33%) | based on 150 samples

if (concave points_worst > 0.116) and (area_worst <= 710.2) and (fractal_dimension_worst <= 0.122) then class: 0 (proba: 100.0%) | based on 9 samples

if (concave points_worst <= 0.116) and (area_mean > 694.15) and (texture_mean > 19.83) then class: 1 (proba: 100.0%) | based on 8 samples

if (concave points_worst <= 0.116) and (area_mean > 694.15) and (texture_mean <= 19.83) then class: 0 (proba: 83.33%) | based on 6 samples

if (concave points_worst > 0.116) and (area_worst <= 710.2) and (fractal_dimension_worst > 0.122) then class: 1 (proba: 100.0%) | based on 4 samples

if (concave points_worst > 0.116) and (area_worst > 710.2) and (concavity_worst <= 0.208) then class: 0 (proba: 100.0%) | based on 2 samples

if (concave points_worst <= 0.116) and (area_mean <= 694.15) and (area_se > 48.975) then class: 0 (proba: 50.0%) | based on 2 samples




### Tree #4
![Tree 4](learner_fold_3_tree.svg)

### Rules

if (perimeter_worst <= 101.65) and (smoothness_worst <= 0.182) and (symmetry_worst <= 0.5) then class: 0 (proba: 98.66%) | based on 149 samples

if (perimeter_worst > 101.65) and (concave points_mean > 0.05) and (texture_worst > 20.355) then class: 1 (proba: 99.31%) | based on 145 samples

if (perimeter_worst > 101.65) and (concave points_mean <= 0.05) and (texture_worst > 27.65) then class: 1 (proba: 80.0%) | based on 15 samples

if (perimeter_worst > 101.65) and (concave points_mean <= 0.05) and (texture_worst <= 27.65) then class: 0 (proba: 93.33%) | based on 15 samples

if (perimeter_worst > 101.65) and (concave points_mean > 0.05) and (texture_worst <= 20.355) then class: 1 (proba: 60.0%) | based on 10 samples

if (perimeter_worst <= 101.65) and (smoothness_worst > 0.182) then class: 1 (proba: 100.0%) | based on 4 samples

if (perimeter_worst <= 101.65) and (smoothness_worst <= 0.182) and (symmetry_worst > 0.5) then class: 1 (proba: 100.0%) | based on 1 samples




### Tree #5
![Tree 5](learner_fold_4_tree.svg)

### Rules

if (perimeter_worst <= 105.95) and (concave points_worst <= 0.159) and (symmetry_worst > 0.161) then class: 0 (proba: 97.52%) | based on 161 samples

if (perimeter_worst > 105.95) and (texture_worst > 20.875) and (smoothness_worst > 0.088) then class: 1 (proba: 98.7%) | based on 154 samples

if (perimeter_worst > 105.95) and (texture_worst <= 20.875) and (perimeter_worst <= 116.8) then class: 0 (proba: 100.0%) | based on 8 samples

if (perimeter_worst > 105.95) and (texture_worst <= 20.875) and (perimeter_worst > 116.8) then class: 1 (proba: 85.71%) | based on 7 samples

if (perimeter_worst <= 105.95) and (concave points_worst > 0.159) and (smoothness_se <= 0.009) then class: 1 (proba: 100.0%) | based on 7 samples

if (perimeter_worst > 105.95) and (texture_worst > 20.875) and (smoothness_worst <= 0.088) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 105.95) and (concave points_worst > 0.159) and (smoothness_se > 0.009) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 105.95) and (concave points_worst <= 0.159) and (symmetry_worst <= 0.161) then class: 1 (proba: 100.0%) | based on 1 samples





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
