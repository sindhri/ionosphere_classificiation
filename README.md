# Ionosphere classification

Use radar returns (34 attributes) to classify whether it is an electron (g) or not (b).  
Credit: Deep Learning with Python by Jason Brownlee  
Data source: UCI Machine learning repository
https://archive.ics.uci.edu/ml/datasets/Ionosphere

Dataset has 351 rows, and 34 attributes/features
## 1. Using the default: not specify learning rate decay and momentum
Accuracy 98.28%

## 2. Time-Based Learning Rate Schedule

Epoch Learning Rate  
1   0.1  
2   0.0999000999  
3   0.0997006985  
4   0.09940249103  
5   0.09900646517  

Accuracy 99.14%, slight improvement

## 3. Drop-based learning rate schedule

The initial learning rate of 0.1 drops by a factor of 0.5 every 10 epochs.
Accuracy 97.41%, not better

# Conclusion: time based learning rate scheduler has the best performance with an accuracy of 99.14%
