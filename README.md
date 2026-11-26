
# Identifying Sexual Violence Survivor Narratives in Reddit Posts Using NLP

CMPS 6730 — Natural Language Processing  
Kashif Basaria, MPH | Tulane University

## Project Overview

This project evaluates traditional machine learning and
transformer-based NLP models for identifying first-person
sexual violence survivor narratives in Reddit posts.

The goal is to support the scalable construction of a
narrative-based research corpus for subsequent public
health research.

## Methods

- Source: r/MenGetRapedToo
- Cleaned corpus: 2,960 posts
- Annotated sample: 580 posts
- Models: TF-IDF logistic regression, BERT, RoBERTa
- Evaluation: Five-fold stratified cross-validation
- Model selection: Sensitivity >= 95%, then maximize specificity
- Independent held-out test: 174 posts

## Results

Selected model: RoBERTa

- Sensitivity: 95.4%
- Specificity: 83.7%
- Accuracy: 92.5%
- ROC-AUC: 0.962

## Presentation

[View the project presentation](https://kbasaria.github.io/project-msv_reddit/)
