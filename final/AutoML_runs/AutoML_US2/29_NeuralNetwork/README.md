# Summary of 29_NeuralNetwork

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

5.9 seconds

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.168869 | nan           |
| auc       | 0.984603 | nan           |
| f1        | 0.955294 |   0.670374    |
| accuracy  | 0.955189 |   0.862471    |
| precision | 1        |   1           |
| recall    | 1        |   2.37241e-08 |
| mcc       | 0.911199 |   0.862471    |


## Confusion matrix (at threshold=0.862471)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     207 |                       5 |
| Labeled as positive |                      14 |                     198 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
