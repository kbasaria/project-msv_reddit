## Models and Evaluation Strategy

**Three model families**

- TF-IDF + logistic regression (unweighted, weighted, tuned)
- BERT (`bert-base-uncased`)
- RoBERTa (`roberta-base`)

**Development workflow**

- Five-fold stratified cross-validation
- Hyperparameter tuning and out-of-fold probability predictions
- Threshold search from **0.05 to 0.95** in increments of 0.01
- Select the threshold maximizing specificity subject to **sensitivity ≥ 0.95**

Evaluate the selected model once on the independent held-out test set.
