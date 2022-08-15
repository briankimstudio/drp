---
layout: default
title: Introduction
nav_order: 1
---

## Purpose

To identify effective anti-cancer drugs for patients by examining each patient's unique gene level information using machine learning algorithms.

![Dataset](/drp/assets/images/purpose.png)

## Research methods

The drug response dataset contains gene level information such as gene expression and the result of drug response (sensitive/resistant). For example, drug 1 is effective for patient 1's gene expression, but it is not effective for patient 2's gene expression. 

![Dataset](/drp/assets/images/method.png)

We train a machine learning model with this information from cell lines, animal models, or clinical data. In other words, the machine learning model learns the association between gene level characteristics and a drug's effectiveness. Once the model has finished training, it takes a new patient's gene-level information as input and then predicts whether the given drug would be helpful for the new patient or not.

![Dataset](/drp/assets/images/dataset.png)

As explained above, drug response prediction is a problem of binary classification. Therefore, among various models of machine learning, any binary classifier can be applied for this research.

## Results

After training the machine learning model, it can perform the following tasks.

1. predict drug's effectiveness
2. find biomarkers(relevant genes) related to the effectiveness

## Challenges

There are several challenges in drug response prediction research.

1. Scarcity of clinical data to train and predict precise results
3. High dimensionality of the training and testing dataset
3. Necessity of multi drugs treatments