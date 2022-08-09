---
layout: default
title: Feature selection
nav_order: 3
---

In drug response prediction dataset, row indicates samples and column represents genes. Thus, number of features equals the number of genes. Unfortunately, the number of genes easily exceeds 10,000. This high dimensionality of dataset requires feature selection process to reduce dimensionalty. There are several approaches in dimension reduction. 

Comparing genes from sensitive and resistant group reveals which genes looks more different than others. Then, only highly different genes are selected for further analysis.

These selected genes are called 'differentially expressed(DE) genes'. And they are feed into the machine learning model to train. 

First, apply t-test to get p-values of all features, then use FDR to filter out relatively less different genes. Finally, apply B/W ratio to get final set of genes.

- t-test
- FDR
- B/W

t-test and FDR
![t-test](/drp/assets/images/t-test_fdr.png)

BW
![bw](/drp/assets/images/bw.png)



- Principal component analysis(PCA)

