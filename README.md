# choose-optimal-threshold-for-imbalanced-dataset
# ROC curve for finding the optimal threshold: 
    A receiver operating characteristics or known as ROC curve is a two-dimensional plot that illustrates how well a classifier system works as the discrimination cut-off value is changed over the range of the predictor variable. The X-axis or independent variable is the false positive rate for the predictive test. The Y-axis or dependent variable is the true positive rate for the predictive test. It is relevant to note that the nearer to the upper-left side of ROC space, the better a classifier is.
    
# G-mean:
The geometric mean or known as G-mean is the geometric mean of sensitivity (known as recall) and specificity. This measure tries to maximize the accuracy of each of the classes while keeping these accuracies balanced. So, it will be one of the unbiased evaluation metrics for # imbalanced classification.

# Youden’s J statistic:
Youden’s J index combines sensitivity and specificity into a single measure (Sensitivity + Specificity — 1) and has a value between 0 and 1. Youden’s index is often used in conjunction with ROC analysis. It is also equivalent to the vertical distance above the diagonal line to the ROC curve for a single decision threshold. The statistic is calculated as:

J = Sensitivity + Specificity – 1 Given that we have Sensitivity (TPR) and the complement of the specificity (FPR), we can calculate it as:

J = Sensitivity + (1 – FalsePositiveRate) – 1 Which we can restate as:

J = TruePositiveRate – FalsePositiveRate We can then choose the threshold with the largest J statistic value.

# The precision-Recall curve for finding the optimal threshold:
The precision-recall curve shows the tradeoff between precision and recall for different threshold. A high area under the curve represents both high recall and high precision, where high precision relates to a low false-positive rate, and high recall relates to a low false-negative rate.

# Optimal Threshold Tuning:
Threshold tuning is a common technique to determine an optimal threshold for imbalanced classification. The sequence of the threshold is generated by the researcher need while the previous techniques using the ROC and Precision & Recall to create a sequence of those thresholds. The advantages are the customization of the threshold sequence as the need but it will have a higher cost of computation.
