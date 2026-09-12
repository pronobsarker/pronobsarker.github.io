---
title: "Fine-Grained Apple Image Classification"
date: '2025-05-01'
summary: "Comparative study of classical ML and deep learning for fine-grained apple variety classification (Fruit-360): ResNet-50 reached macro-F1 0.99, with analysis of misclassification patterns and deployment trade-offs."
tags:
  - Computer Vision
  - Model Evaluation
  - Robustness
featured: true
---

## Overview

**Research Assistant, Gettysburg College & Rice Fruit Company · Spring 2025 · Advisors: Dr. Kim Spayd, Dr. Eatai Roth**

A comparative study of machine-learning approaches for **fine-grained apple image classification** on the Fruit-360 dataset — a setting where classes are visually similar and mistakes have practical consequences for a real industry partner.

## Research Question

Which modeling approach best distinguishes fine-grained apple varieties, and what are the accuracy, generalization, and deployment trade-offs between classical methods and deep learning?

## Approach

- Implemented and compared **KNN, SVM, Random Forest, and ResNet-50** on the same classification task.
- Evaluated with **accuracy, precision, recall, macro-F1, and confusion matrices** — not accuracy alone.
- Analyzed **misclassification patterns** among visually similar apple classes to understand *where* and *why* models fail.
- Investigated **model generalization and practical deployment trade-offs** (performance vs. complexity) with the industry partner's constraints in mind.

## My Contribution

I ran the full comparative study: model implementation, the evaluation protocol across five metrics, the misclassification analysis, and the synthesis of findings into deployment-relevant trade-offs.

## Results

**ResNet-50 achieved a macro-F1 score of 0.99**, substantially outperforming the classical baselines — but the more valuable output was the failure analysis: characterizing exactly which visually similar classes confused which models, and what that implies for deploying vision systems in agricultural settings.

## What This Motivated

This project shaped my interest in **robustness and evaluation**: high aggregate metrics can hide systematic failures, and understanding a model's mistakes matters as much as its score. It is the empirical complement to my theoretical work — asking not just "does it work?" but "where does it break?"

## Technologies

Python · PyTorch · scikit-learn · ResNet-50
