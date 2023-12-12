---
title: "Derandomized novelty detection with FDR control via conformal e-values"
collection: publications
permalink: /publication/2023-c-fdr-evals
excerpt: ''
date: 2023-02-16
venue: 'Advances in Neural Information Processing Systems 36 (NeurIPS), 2023'
---

**Abstract**

Conformal inference provides a general distribution-free method to rigorously calibrate the output of any machine learning algorithm for novelty detection. While this approach has many strengths, it has the limitation of being randomized, in the sense that it may lead to different results when analyzing twice the same data, and this can hinder the interpretation of any findings. We propose to make conformal inferences more stable by leveraging suitable conformal e-values instead of p-values to quantify statistical significance. This solution allows the evidence gathered from multiple analyses of the same data to be aggregated effectively while provably controlling the false discovery rate. Further, we show that the proposed method can reduce randomness without much loss of power compared to standard conformal inference, partly thanks to an innovative way of weighting conformal e-values based on additional side information carefully extracted from the same data. Simulations with synthetic and real data confirm this solution can be effective at eliminating random noise in the inferences obtained with state-of-the-art alternative techniques, sometimes also leading to higher power. 

[arXiv link](https://arxiv.org/pdf/2302.07294.pdf)