
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

## Ensemble Learning Results

The ensemble methods combine the strengths of **ResNet50**, **ResNet18**, **EfficientNetB0**, and **VGG16** to achieve higher classification accuracy for the five aluminum alloys.

### 1. Soft Voting Results (Fusion)
Soft voting achieved the highest overall performance by averaging the probability distributions from the base models.

| Alloy | Precision | Recall | F1-Score | Support |
| :--- | :---: | :---: | :---: | :---: |
| Al 1050 | 0.92 | 0.97 | 0.94 | 900 |
| Al 2017 | 0.89 | 0.93 | 0.91 | 900 |
| Al 5083 | 0.81 | 0.84 | 0.82 | 900 |
| Al 6082 | 0.83 | 0.86 | 0.84 | 900 |
| Al 7075 | 0.90 | 0.95 | 0.92 | 900 |
| **Accuracy** | | | **0.9585** | **4500** |

### 2. Hard Voting Results (Majority Rule)
Hard voting selects the final class based on the majority label predicted by the individual models.

| Alloy | Precision | Recall | F1-Score | Support |
| :--- | :---: | :---: | :---: | :---: |
| Al 1050 | 0.90 | 0.96 | 0.93 | 900 |
| Al 2017 | 0.87 | 0.91 | 0.89 | 900 |
| Al 5083 | 0.78 | 0.81 | 0.79 | 900 |
| Al 6082 | 0.80 | 0.83 | 0.81 | 900 |
| Al 7075 | 0.89 | 0.93 | 0.91 | 900 |
| **Accuracy** | | | **0.9401** | **4500** |

---

### Final Comparison
* **Soft Voting Accuracy**: 95.85%
* **Hard Voting Accuracy**: 94.01%
* **Best Individual Model (ResNet50)**: 93.7%

The results confirm that the **Soft Voting Ensemble** provides the most robust identification for X-ray-based material analysis.
