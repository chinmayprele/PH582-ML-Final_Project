# Summary of 19_NeuralNetwork_GoldenFeatures

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

9.5 seconds

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.158605 | nan           |
| auc       | 0.986606 | nan           |
| f1        | 0.954436 |   0.544482    |
| accuracy  | 0.955189 |   0.544482    |
| precision | 1        |   0.999958    |
| recall    | 1        |   8.83454e-21 |
| mcc       | 0.911199 |   0.573343    |


## Confusion matrix (at threshold=0.544482)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     206 |                       6 |
| Labeled as positive |                      13 |                     199 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)

[<< Go back](../README.md)
