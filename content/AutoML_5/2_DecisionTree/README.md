# Summary of 2_DecisionTree

[<< Go back](../README.md)


## Decision Tree
- **n_jobs**: -1
- **criterion**: gini
- **max_depth**: 4
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

34.6 seconds

## Metric details
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.712861 |  nan        |
| auc       | 0.913882 |  nan        |
| f1        | 0.922717 |    0.500263 |
| accuracy  | 0.92217  |    0.500263 |
| precision | 0.916279 |    0.500263 |
| recall    | 0.957547 |    0        |
| mcc       | 0.844424 |    0.500263 |


## Confusion matrix (at threshold=0.500263)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     194 |                      18 |
| Labeled as positive |                      15 |                     197 |

## Learning curves
![Learning curves](learning_curves.png)

## Decision Tree 

### Tree #1
![Tree 1](learner_fold_0_tree.svg)

### Rules

if (concave points_mean > 0.256) and (concavity_worst > 0.178) and (area_se > 0.013) and (texture_mean > 0.192) then class: 1 (proba: 99.34%) | based on 152 samples

if (concave points_mean <= 0.256) and (radius_worst <= 0.305) and (area_se <= 0.075) and (texture_worst <= 0.568) then class: 0 (proba: 100.0%) | based on 139 samples

if (concave points_mean > 0.256) and (concavity_worst > 0.178) and (area_se > 0.013) and (texture_mean <= 0.192) then class: 1 (proba: 55.56%) | based on 9 samples

if (concave points_mean <= 0.256) and (radius_worst <= 0.305) and (area_se <= 0.075) and (texture_worst > 0.568) then class: 0 (proba: 88.89%) | based on 9 samples

if (concave points_mean <= 0.256) and (radius_worst > 0.305) and (texture_mean > 0.342) then class: 1 (proba: 100.0%) | based on 8 samples

if (concave points_mean <= 0.256) and (radius_worst > 0.305) and (texture_mean <= 0.342) and (fractal_dimension_mean <= 0.189) then class: 0 (proba: 100.0%) | based on 7 samples

if (concave points_mean > 0.256) and (concavity_worst <= 0.178) and (symmetry_mean > 0.277) then class: 0 (proba: 100.0%) | based on 6 samples

if (concave points_mean > 0.256) and (concavity_worst > 0.178) and (area_se <= 0.013) then class: 0 (proba: 100.0%) | based on 3 samples

if (concave points_mean <= 0.256) and (radius_worst > 0.305) and (texture_mean <= 0.342) and (fractal_dimension_mean > 0.189) then class: 1 (proba: 66.67%) | based on 3 samples

if (concave points_mean <= 0.256) and (radius_worst <= 0.305) and (area_se > 0.075) then class: 1 (proba: 100.0%) | based on 2 samples

if (concave points_mean > 0.256) and (concavity_worst <= 0.178) and (symmetry_mean <= 0.277) then class: 1 (proba: 100.0%) | based on 1 samples




### Tree #2
![Tree 2](learner_fold_1_tree.svg)

### Rules

if (perimeter_worst <= 0.257) and (concave points_worst <= 0.621) and (area_se <= 0.158) and (smoothness_worst <= 0.788) then class: 0 (proba: 98.65%) | based on 148 samples

if (perimeter_worst > 0.257) and (perimeter_worst > 0.334) and (fractal_dimension_se > 0.019) then class: 1 (proba: 100.0%) | based on 135 samples

if (perimeter_worst > 0.257) and (perimeter_worst <= 0.334) and (texture_worst > 0.312) and (symmetry_worst > 0.193) then class: 1 (proba: 92.59%) | based on 27 samples

if (perimeter_worst > 0.257) and (perimeter_worst <= 0.334) and (texture_worst <= 0.312) and (area_mean > 0.197) then class: 0 (proba: 100.0%) | based on 15 samples

if (perimeter_worst > 0.257) and (perimeter_worst <= 0.334) and (texture_worst > 0.312) and (symmetry_worst <= 0.193) then class: 0 (proba: 83.33%) | based on 6 samples

if (perimeter_worst <= 0.257) and (concave points_worst > 0.621) then class: 1 (proba: 100.0%) | based on 4 samples

if (perimeter_worst > 0.257) and (perimeter_worst > 0.334) and (fractal_dimension_se <= 0.019) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst > 0.257) and (perimeter_worst <= 0.334) and (texture_worst <= 0.312) and (area_mean <= 0.197) then class: 1 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 0.257) and (concave points_worst <= 0.621) and (area_se > 0.158) then class: 1 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 0.257) and (concave points_worst <= 0.621) and (area_se <= 0.158) and (smoothness_worst > 0.788) then class: 1 (proba: 100.0%) | based on 1 samples




### Tree #3
![Tree 3](learner_fold_2_tree.svg)

### Rules

if (concave points_mean <= 0.256) and (radius_worst <= 0.305) and (area_se <= 0.075) and (smoothness_worst <= 0.689) then class: 0 (proba: 98.05%) | based on 154 samples

if (concave points_mean > 0.256) and (concavity_worst > 0.172) and (texture_mean > 0.209) and (perimeter_worst > 0.197) then class: 1 (proba: 100.0%) | based on 144 samples

if (concave points_mean <= 0.256) and (radius_worst > 0.305) and (texture_mean > 0.204) and (concave points_se <= 0.192) then class: 1 (proba: 100.0%) | based on 11 samples

if (concave points_mean > 0.256) and (concavity_worst > 0.172) and (texture_mean <= 0.209) and (area_worst > 0.156) then class: 1 (proba: 100.0%) | based on 6 samples

if (concave points_mean > 0.256) and (concavity_worst <= 0.172) and (fractal_dimension_worst > 0.083) then class: 0 (proba: 100.0%) | based on 5 samples

if (concave points_mean <= 0.256) and (radius_worst > 0.305) and (texture_mean <= 0.204) then class: 0 (proba: 100.0%) | based on 5 samples

if (concave points_mean > 0.256) and (concavity_worst > 0.172) and (texture_mean <= 0.209) and (area_worst <= 0.156) then class: 0 (proba: 100.0%) | based on 4 samples

if (concave points_mean <= 0.256) and (radius_worst > 0.305) and (texture_mean > 0.204) and (concave points_se > 0.192) then class: 0 (proba: 100.0%) | based on 3 samples

if (concave points_mean > 0.256) and (concavity_worst > 0.172) and (texture_mean > 0.209) and (perimeter_worst <= 0.197) then class: 0 (proba: 50.0%) | based on 2 samples

if (concave points_mean <= 0.256) and (radius_worst <= 0.305) and (area_se > 0.075) and (smoothness_se > 0.115) then class: 1 (proba: 100.0%) | based on 2 samples

if (concave points_mean > 0.256) and (concavity_worst <= 0.172) and (fractal_dimension_worst <= 0.083) then class: 1 (proba: 100.0%) | based on 1 samples

if (concave points_mean <= 0.256) and (radius_worst <= 0.305) and (area_se > 0.075) and (smoothness_se <= 0.115) then class: 0 (proba: 100.0%) | based on 1 samples

if (concave points_mean <= 0.256) and (radius_worst <= 0.305) and (area_se <= 0.075) and (smoothness_worst > 0.689) then class: 1 (proba: 100.0%) | based on 1 samples




### Tree #4
![Tree 4](learner_fold_3_tree.svg)

### Rules

if (perimeter_worst > 0.257) and (concavity_worst > 0.165) and (texture_mean > 0.192) and (smoothness_worst > 0.159) then class: 1 (proba: 98.11%) | based on 159 samples

if (perimeter_worst <= 0.257) and (concave points_worst <= 0.621) and (texture_worst <= 0.714) and (area_se <= 0.075) then class: 0 (proba: 99.32%) | based on 148 samples

if (perimeter_worst > 0.257) and (concavity_worst <= 0.165) and (texture_mean <= 0.343) then class: 0 (proba: 100.0%) | based on 10 samples

if (perimeter_worst > 0.257) and (concavity_worst > 0.165) and (texture_mean <= 0.192) and (radius_worst <= 0.354) then class: 0 (proba: 100.0%) | based on 5 samples

if (perimeter_worst > 0.257) and (concavity_worst > 0.165) and (texture_mean <= 0.192) and (radius_worst > 0.354) then class: 1 (proba: 100.0%) | based on 4 samples

if (perimeter_worst > 0.257) and (concavity_worst <= 0.165) and (texture_mean > 0.343) and (area_se > 0.057) then class: 1 (proba: 100.0%) | based on 4 samples

if (perimeter_worst <= 0.257) and (concave points_worst <= 0.621) and (texture_worst <= 0.714) and (area_se > 0.075) then class: 0 (proba: 66.67%) | based on 3 samples

if (perimeter_worst <= 0.257) and (concave points_worst > 0.621) then class: 1 (proba: 100.0%) | based on 2 samples

if (perimeter_worst > 0.257) and (concavity_worst > 0.165) and (texture_mean > 0.192) and (smoothness_worst <= 0.159) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst > 0.257) and (concavity_worst <= 0.165) and (texture_mean > 0.343) and (area_se <= 0.057) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 0.257) and (concave points_worst <= 0.621) and (texture_worst > 0.714) and (smoothness_se > 0.17) then class: 1 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 0.257) and (concave points_worst <= 0.621) and (texture_worst > 0.714) and (smoothness_se <= 0.17) then class: 0 (proba: 100.0%) | based on 1 samples




### Tree #5
![Tree 5](learner_fold_4_tree.svg)

### Rules

if (perimeter_worst > 0.272) and (texture_worst > 0.177) and (concave points_mean > 0.153) and (fractal_dimension_se <= 0.415) then class: 1 (proba: 98.7%) | based on 154 samples

if (perimeter_worst <= 0.272) and (concave points_worst <= 0.464) and (area_se <= 0.158) and (area_se <= 0.074) then class: 0 (proba: 99.33%) | based on 150 samples

if (perimeter_worst <= 0.272) and (concave points_worst > 0.464) and (texture_worst > 0.37) then class: 1 (proba: 100.0%) | based on 9 samples

if (perimeter_worst > 0.272) and (texture_worst <= 0.177) and (area_se <= 0.123) then class: 0 (proba: 100.0%) | based on 8 samples

if (perimeter_worst <= 0.272) and (concave points_worst > 0.464) and (texture_worst <= 0.37) and (fractal_dimension_worst <= 0.441) then class: 0 (proba: 100.0%) | based on 5 samples

if (perimeter_worst > 0.272) and (texture_worst > 0.177) and (concave points_mean <= 0.153) and (concave points_se > 0.191) then class: 0 (proba: 100.0%) | based on 3 samples

if (perimeter_worst > 0.272) and (texture_worst <= 0.177) and (area_se > 0.123) then class: 1 (proba: 100.0%) | based on 3 samples

if (perimeter_worst <= 0.272) and (concave points_worst <= 0.464) and (area_se <= 0.158) and (area_se > 0.074) then class: 0 (proba: 66.67%) | based on 3 samples

if (perimeter_worst > 0.272) and (texture_worst > 0.177) and (concave points_mean <= 0.153) and (concave points_se <= 0.191) then class: 1 (proba: 100.0%) | based on 2 samples

if (perimeter_worst > 0.272) and (texture_worst > 0.177) and (concave points_mean > 0.153) and (fractal_dimension_se > 0.415) then class: 0 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 0.272) and (concave points_worst > 0.464) and (texture_worst <= 0.37) and (fractal_dimension_worst > 0.441) then class: 1 (proba: 100.0%) | based on 1 samples

if (perimeter_worst <= 0.272) and (concave points_worst <= 0.464) and (area_se > 0.158) then class: 1 (proba: 100.0%) | based on 1 samples





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
