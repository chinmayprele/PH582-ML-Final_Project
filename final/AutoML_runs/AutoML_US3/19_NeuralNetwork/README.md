# Summary of 19_NeuralNetwork

[<< Go back](../README.md)


## Neural Network
- **n_jobs**: -1
- **dense_1_size**: 32
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

5.2 seconds

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.14853  | nan           |
| auc       | 0.990143 | nan           |
| f1        | 0.951945 |   0.447944    |
| accuracy  | 0.950472 |   0.447944    |
| precision | 1        |   0.996264    |
| recall    | 1        |   2.60221e-06 |
| mcc       | 0.902642 |   0.447944    |


## Confusion matrix (at threshold=0.447944)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     195 |                      17 |
| Labeled as positive |                       4 |                     208 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
