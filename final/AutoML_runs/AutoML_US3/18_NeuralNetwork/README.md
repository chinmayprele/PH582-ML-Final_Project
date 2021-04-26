# Summary of 18_NeuralNetwork

[<< Go back](../README.md)


## Neural Network
- **n_jobs**: -1
- **dense_1_size**: 64
- **dense_2_size**: 32
- **learning_rate**: 0.08
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

6.0 seconds

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.143663 | nan           |
| auc       | 0.989565 | nan           |
| f1        | 0.962441 |   0.500002    |
| accuracy  | 0.962264 |   0.500002    |
| precision | 0.994652 |   0.97769     |
| recall    | 1        |   1.41117e-12 |
| mcc       | 0.924569 |   0.500002    |


## Confusion matrix (at threshold=0.500002)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     203 |                       9 |
| Labeled as positive |                       7 |                     205 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
