# Summary of 28_NeuralNetwork

[<< Go back](../README.md)


## Neural Network
- **n_jobs**: -1
- **dense_1_size**: 64
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

5.6 seconds

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.132935 | nan           |
| auc       | 0.991968 | nan           |
| f1        | 0.959036 |   0.923855    |
| accuracy  | 0.959906 |   0.923855    |
| precision | 1        |   0.999216    |
| recall    | 1        |   1.48792e-09 |
| mcc       | 0.920641 |   0.923855    |


## Confusion matrix (at threshold=0.923855)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     208 |                       4 |
| Labeled as positive |                      13 |                     199 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
