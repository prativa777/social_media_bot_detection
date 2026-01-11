# 🤖 Account-Level Bot Detection Using Machine Learning

## Overview
This project implements a machine learning model to estimate whether a social media account exhibits **bot-like behavior** based on behavioral activity patterns.  
It uses **synthetic Facebook-like data** to ensure ethical and legal compliance.

---

## Method
- **Problem Type:** Binary Classification (Human vs Bot-like)  
- **Model:** Random Forest Classifier (baseline: Logistic Regression)  
- **Data Representation:** Each row represents **one account**, not individual actions  
- **Features:**
```text
account_age_days
likes_per_day
median_time_between_likes
night_activity_ratio
content_diversity_score
burstiness_index
engagement_entropy

**Why the Results Are Perfect**

Dataset is synthetic with clearly separated behavioral patterns for bots and humans

Train and test data are generated from the same controlled process

Classes are fully separable, allowing the model to achieve perfect performance

This demonstrates correctness of the ML pipeline, not real-world applicability

**Ethics and Limitations**

No real Facebook or user data is used

No scraping or monitoring of real accounts

The model outputs a likelihood score, not a definitive label

Real-world bot detection would involve noise, overlapping behavior, and adversarial tactics

**Future Improvements**

Introduce realistic noise and feature overlap

Apply unsupervised anomaly detection (e.g., Isolation Forest)

Add cross-validation, ROC/Precision-Recall analysis

Incorporate explainability (e.g., SHAP values)
