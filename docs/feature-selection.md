---
layout: default
title: Feature selection
nav_order: 3
---

In drug response prediction dataset, row indicates samples and column represents genes. Thus, number of features equals the number of genes. Unfortunately, the number of genes easily exceeds 10,000. This high dimensionality of dataset requires feature selection process to reduce dimensionalty. There are several approaches in dimension reduction. 

Comparing genes from sensitive and resistant group reveals which genes looks more different than others. Then, only highly different genes are selected for further analysis.

These selected genes are called 'differentially expressed(DE) genes'. And they are feed into the machine learning model to train. 

First, apply t-test to get p-values of all features, then use FDR to filter out relatively less different genes (Reiner et al., 2003). Finally, apply B/W ratio to get final set of genes.

- t-test
- FDR
- B/W

t-test and FDR (Reiner et al., 2003)
![t-test](/drp/assets/images/t-test_fdr.png)

B/W
![bw](/drp/assets/images/bw.png)

Domain adaptation (Mourragui et al., 2019)
![da](/drp/assets/images/da.png)

- Principal component analysis(PCA)

### References

Mourragui, S., Loog, M., van de Wiel, M. A., Reinders, M. J. T., & Wessels, L. F. A. (2019). PRECISE: A domain adaptation approach to transfer predictors of drug response from pre-clinical models to tumors. Bioinformatics, 35(14), i510–i519. https://doi.org/10.1093/bioinformatics/btz372

Reiner, A., Yekutieli, D., & Benjamini, Y. (2003). Identifying differentially expressed genes  using false discovery rate controlling procedures. Bioinformatics, 19(3), 368–375. https://doi.org/10.1093/bioinformatics/btf877
