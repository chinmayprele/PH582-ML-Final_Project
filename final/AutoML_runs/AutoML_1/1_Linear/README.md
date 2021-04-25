# Summary of 1_Linear

[<< Go back](../README.md)


## Logistic Regression (Linear)
- **n_jobs**: -1
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

25.5 seconds

## Metric details
|           |    score |    threshold |
|:----------|---------:|-------------:|
| logloss   | 0.161814 | nan          |
| auc       | 0.99159  | nan          |
| f1        | 0.95962  |   0.477147   |
| accuracy  | 0.959906 |   0.477147   |
| precision | 1        |   0.975623   |
| recall    | 1        |   0.00251704 |
| mcc       | 0.919903 |   0.477147   |


## Confusion matrix (at threshold=0.477147)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     205 |                       7 |
| Labeled as positive |                      10 |                     202 |

## Learning curves
![Learning curves](learning_curves.png)

## Coefficients
| feature                 |   Learner_1 |   Learner_2 |   Learner_3 |   Learner_4 |    Learner_5 |
|:------------------------|------------:|------------:|------------:|------------:|-------------:|
| concave points_worst    |   2.33225   |    2.40782  |   2.49428   |   2.492     |  2.36282     |
| texture_worst           |   2.09685   |    2.28118  |   1.93942   |   2.24153   |  2.00512     |
| radius_worst            |   1.98623   |    2.03591  |   1.92581   |   2.1128    |  2.08513     |
| perimeter_worst         |   1.84014   |    1.91961  |   1.77968   |   1.91503   |  1.91229     |
| concave points_mean     |   1.93103   |    1.81558  |   1.84623   |   1.79046   |  1.9264      |
| radius_mean             |   1.618     |    1.60863  |   1.52146   |   1.62918   |  1.68221     |
| perimeter_mean          |   1.59242   |    1.57828  |   1.5081    |   1.59712   |  1.66127     |
| texture_mean            |   1.62492   |    1.63392  |   1.4395    |   1.53571   |  1.47966     |
| area_worst              |   1.44353   |    1.46916  |   1.39208   |   1.52974   |  1.48331     |
| area_mean               |   1.36496   |    1.36092  |   1.27889   |   1.35901   |  1.4013      |
| smoothness_worst        |   1.30848   |    1.1404   |   1.17299   |   1.309     |  1.28946     |
| concavity_mean          |   1.0891    |    1.18634  |   1.49062   |   1.19589   |  1.15162     |
| concavity_worst         |   0.970413  |    1.24248  |   1.42758   |   1.1287    |  1.0733      |
| radius_se               |   1.07167   |    1.01191  |   1.02763   |   0.90224   |  1.07062     |
| symmetry_worst          |   0.935178  |    1.09298  |   0.778489  |   1.0332    |  1.01988     |
| perimeter_se            |   0.846166  |    0.834868 |   0.828288  |   0.662938  |  0.832358    |
| compactness_worst       |   0.742475  |    0.717461 |   0.638067  |   0.690504  |  0.714642    |
| area_se                 |   0.712747  |    0.689322 |   0.670707  |   0.645404  |  0.702164    |
| smoothness_mean         |   0.760495  |    0.387533 |   0.491431  |   0.564538  |  0.736322    |
| symmetry_mean           |   0.508808  |    0.578272 |   0.284262  |   0.340625  |  0.488744    |
| concave points_se       |   0.458336  |    0.253967 |   0.657457  |   0.272333  |  0.379264    |
| compactness_mean        |   0.503475  |    0.243122 |   0.387302  |   0.322949  |  0.43561     |
| fractal_dimension_worst |   0.328736  |    0.224863 |   0.295428  |   0.246007  |  0.253858    |
| texture_se              |   0.262045  |    0.177801 |   0.164073  |   0.149986  |  0.188129    |
| smoothness_se           |   0.0816303 |   -0.167868 |   0.0230513 |   0.0622327 | -0.000602253 |
| concavity_se            |  -0.272074  |   -0.219598 |   0.121797  |  -0.224357  | -0.25758     |
| symmetry_se             |  -0.313218  |   -0.157951 |  -0.366255  |  -0.165801  | -0.204674    |
| fractal_dimension_se    |  -0.45837   |   -0.546942 |  -0.210896  |  -0.516321  | -0.513039    |
| compactness_se          |  -0.547377  |   -0.540823 |  -0.324215  |  -0.619445  | -0.607757    |
| fractal_dimension_mean  |  -0.741812  |   -1.13441  |  -0.751171  |  -0.922959  | -0.875714    |
| intercept               |  -7.8525    |   -7.57531  |  -7.47969   |  -7.67569   | -7.64514     |


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
