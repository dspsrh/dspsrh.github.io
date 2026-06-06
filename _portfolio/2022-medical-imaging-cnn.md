---
title: "Deep CNN for Medical Image Classification (IDC)"
excerpt: "Depth-wise separable CNN for invasive ductal carcinoma detection from histopathology."
collection: portfolio
---

**[View code on GitHub](https://github.com/dspsrh/Breastcancer_CNN)** · [Publication](/publication/2022-predicting-invasive-ductal-carcinoma-icaie/)

Undergraduate research (2022) · The Pennsylvania State University

* Investigated whether a parameter-efficient convolutional design could detect invasive ductal carcinoma (IDC) from histopathology while remaining robust to severe class imbalance.
* Designed a depth-wise separable CNN (SeparableConv2D) over 50×50 patches in TensorFlow/Keras—SeparableConv2D–BatchNorm–MaxPooling–Dropout blocks feeding a 256-unit dense softmax classifier trained with Adagrad under binary cross-entropy.
* Built a reproducible re-balancing and preprocessing-to-evaluation pipeline for imbalanced medical-imaging data.
* Demonstrated that the separable-convolution architecture matched standard convolutional baselines at substantially lower parameter count and computational cost.
* First-author publication at ICAIE 2022.
