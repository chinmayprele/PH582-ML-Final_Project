# Summary of 19_NeuralNetwork_RandomFeature

[<< Go back](../README.md)


## Neural Network
- **n_jobs**: -1
- **dense_1_size**: 32
- **dense_2_size**: 32
- **learning_rate**: 0.05
- **explain_level**: 1

## Validation
 - **validation_type**: kfold
 - **k_folds**: 5
 - **shuffle**: True
 - **stratify**: True
 - **random_seed**: 1230

## Optimized metric
logloss

## Training time

5.0 seconds

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.221051 | nan           |
| auc       | 0.972455 | nan           |
| f1        | 0.933014 |   0.598907    |
| accuracy  | 0.933962 |   0.598907    |
| precision | 1        |   0.999672    |
| recall    | 1        |   2.34173e-09 |
| mcc       | 0.868272 |   0.598907    |


## Confusion matrix (at threshold=0.598907)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     201 |                      11 |
| Labeled as positive |                      17 |                     195 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
