# Summary of 20_NearestNeighbors

[<< Go back](../README.md)


## k-Nearest Neighbors (Nearest Neighbors)
- **n_jobs**: -1
- **n_neighbors**: 7
- **weights**: uniform
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

42.9 seconds

## Metric details
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.210939 |  nan        |
| auc       | 0.983079 |  nan        |
| f1        | 0.947115 |    0.428571 |
| accuracy  | 0.948113 |    0.428571 |
| precision | 0.98895  |    0.785714 |
| recall    | 0.990566 |    0        |
| mcc       | 0.896865 |    0.428571 |


## Confusion matrix (at threshold=0.428571)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     205 |                       7 |
| Labeled as positive |                      15 |                     197 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
