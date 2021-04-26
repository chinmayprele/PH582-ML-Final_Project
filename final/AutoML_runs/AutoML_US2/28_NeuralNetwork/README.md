# Summary of 28_NeuralNetwork

[<< Go back](../README.md)


## Neural Network
- **n_jobs**: -1
- **dense_1_size**: 16
- **dense_2_size**: 32
- **learning_rate**: 0.05
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

5.1 seconds

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.158653 | nan           |
| auc       | 0.986494 | nan           |
| f1        | 0.945882 |   0.47807     |
| accuracy  | 0.945755 |   0.47807     |
| precision | 1        |   0.999996    |
| recall    | 1        |   1.82897e-08 |
| mcc       | 0.891519 |   0.47807     |


## Confusion matrix (at threshold=0.47807)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     200 |                      12 |
| Labeled as positive |                      11 |                     201 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
