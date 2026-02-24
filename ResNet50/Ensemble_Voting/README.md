# Ensemble Methods: Multi-Task Material Analysis
This section covers the aggregation of ResNet, VGG, and EfficientNet architectures.

### Implementation
* **Hard Voting:** Classification based on the majority label predicted across all models.
* **Soft Voting:** Classification based on the average of softmax probability distributions for the five alloy classes (Al 1050, 2017, 5083, 6082, 7075).
