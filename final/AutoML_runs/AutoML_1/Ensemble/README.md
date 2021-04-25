# Summary of Ensemble

[<< Go back](../README.md)


## Ensemble structure
| Model                        |   Weight |
|:-----------------------------|---------:|
| 26_NeuralNetwork             |        1 |
| 38_NeuralNetwork             |       15 |
| 40_LightGBM_SelectedFeatures |       21 |

## Metric details
|           |     score |     threshold |
|:----------|----------:|--------------:|
| logloss   | 0.0858545 | nan           |
| auc       | 0.995083  | nan           |
| f1        | 0.971831  |   0.392667    |
| accuracy  | 0.971698  |   0.392667    |
| precision | 1         |   0.999153    |
| recall    | 1         |   6.18645e-05 |
| mcc       | 0.943438  |   0.392667    |


## Confusion matrix (at threshold=0.392667)
|                     |   Predicted as negative |   Predicted as positive |
|:--------------------|------------------------:|------------------------:|
| Labeled as negative |                     205 |                       7 |
| Labeled as positive |                       5 |                     207 |

## Learning curves
![Learning curves](learning_curves.png)

[<< Go back](../README.md)
