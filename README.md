
## Detailed Classification Results
The following table summarizes the **Precision (AP)**, **Recall (AUC)**, and **F1-score** across all five aluminum alloys for each model architecture.

| Metric | Alloy | ResNet18 | ResNet50 | EfficientNetB0 | VGG16 | Support |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: |
| **Precision (AP)** | Al 1050 | 0.76 | 0.88 | 0.75 | 0.68 | 900 |
| | Al 2017 | 0.83 | 0.92 | 0.70 | 0.63 | 900 |
| | Al 5083 | 0.66 | 0.70 | 0.68 | 0.60 | 900 |
| | Al 6082 | 0.64 | 0.70 | 0.69 | 0.61 | 900 |
| | Al 7075 | 0.75 | 0.81 | 0.72 | 0.65 | 900 |
| **Recall (AUC)** | Al 1050 | 0.92 | 0.96 | 0.90 | 0.86 | 900 |
| | Al 2017 | 0.95 | 0.97 | 0.88 | 0.83 | 0.90 |
| | Al 5083 | 0.88 | 0.89 | 0.78 | 0.72 | 900 |
| | Al 6082 | 0.88 | 0.90 | 0.80 | 0.75 | 900 |
| | Al 7075 | 0.93 | 0.95 | 0.87 | 0.82 | 900 |
| **F1-score** | Al 1050 | 0.83 | 0.92 | 0.80 | 0.74 | 900 |
| | Al 2017 | 0.89 | 0.94 | 0.76 | 0.70 | 900 |
| | Al 5083 | 0.75 | 0.78 | 0.61 | 0.55 | 900 |
| | Al 6082 | 0.74 | 0.78 | 0.64 | 0.58 | 900 |
| | Al 7075 | 0.83 | 0.88 | 0.73 | 0.68 | 900 |

> **Key Takeaway:** ResNet50 consistently outperformed other models across all metrics, reaching a peak F1-score of 0.94 for Al 2017.
