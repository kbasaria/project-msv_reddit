---
layout: slide
title: ""
---
## CROSS-VALIDATION MODEL COMPARISON

| Model (5-fold CV) | Accuracy | Sensitivity | Specificity | ROC-AUC |
|:--|--:|--:|--:|--:|
| Baseline logistic regression | .793 | .997 | .170 | .933 |
| Weighted logistic regression | .882 | .905 | .810 | .934 |
| **Tuned BERT** | **.916** | .948 | .820 | .953 |
| **Tuned RoBERTa** | .914 | .944 | .820 | **.963** |

*Values are five-fold means; selected configurations shown.*

**Takeaway:** BERT had slightly higher cross-validation accuracy. RoBERTa had the highest ROC-AUC and the strongest specificity after sensitivity-constrained threshold selection.
