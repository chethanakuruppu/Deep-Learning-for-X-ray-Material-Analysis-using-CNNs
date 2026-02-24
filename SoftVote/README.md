# Soft Voting (Probability Fusion) Results
**Overall Accuracy: 95.85%**

Soft voting averages the softmax probability outputs from ResNet50, ResNet18, EfficientNetB0, and VGG16 to make the final prediction.

### Classification Performance
| Alloy | Precision | Recall | F1-Score | Support |
| :--- | :---: | :---: | :---: | :---: |
| Al 1050 | 0.92 | 0.97 | 0.94 | 900 |
| Al 2017 | 0.89 | 0.93 | 0.91 | 900 |
| Al 5083 | 0.81 | 0.84 | 0.82 | 900 |
| Al 6082 | 0.83 | 0.86 | 0.84 | 900 |
| Al 7075 | 0.90 | 0.95 | 0.92 | 900 |

> **Note:** Soft voting provided the highest accuracy across the entire study.
