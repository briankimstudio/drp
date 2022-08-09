---
layout: default
title: Feature selection
nav_order: 3
---

In drug response prediction dataset, row indicates samples and column represents genes. Thus, number of features equals the number of genes. Unfortunately, the number of genes easily exceeds 10,000. This high dimensionality of dataset requires feature selection process to reduce dimensionalty. There are several approaches in dimension reduction. 

Comparing genes from sensitive and resistant group reveals which genes looks more different than others. Then, only highly different genes are selected for further analysis.

These selected genes are called 'differentially expressed(DE) genes'. And they are feed into the machine learning model to train. 

- t-test
- FDR
- Principal component analysis(PCA)

