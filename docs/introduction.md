---
layout: default
title: Introduction
nav_order: 1
---

Drug response prediction is a research area where gene level information is examined to predict the effectiveness of a given anti-cancer drug.

## Purpose

To identify effective anti-cancer drugs for patients by examining each patient's unique gene level information using machine learning algorithm.

## Research methods

Drug response dataset contains gene level information such as gene expression and the results of drug response (sensitive/registant). For example, the drug 1 is effective for the patient 1's gene expression, but, not effective for patient 2's gene expression. 

![Dataset](/assets/images/dataset.png)

We train machine learning model with this information. In other words, machine learning model learns the association between gene level information and drug's effectiveness. Once the model finished traning, it compare news patient's gene level information with the dataset to predict whether the given drug would helpful for the new patient or not.

As explained above, drug response prediction is a problem of binary classification. Therefore, among machine learning models, any binary classifier can be applied for this research.

## Results

After training machine learning model, it takes patient's gene information as an input, then, predict whether the drug is effective or not for this patient.

## Discussion

There are several challneges in drug response prediction research. 