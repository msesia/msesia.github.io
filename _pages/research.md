---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
redirect_from:
  - /research
---

{% include base_path %}


## Methodology and theory

### High-dimensional variable selection

Modern data sets often measure thousands of possible explanatory variables, which one would want to leverage to explain a particular phenomenon of interest, although only a small subset of them may be relevant. The challenge for statisticians is to identify which of these variables are truly important by analyzing the data, even though the number of observations may be smaller than the number of variables, and to do so with confidence.
I am broadly interested in developing methods that can perform statistically principled variable selection for high-dimensional data, without relying on unrealistic assumptions. If you would like to learn more about this line of research, a good starting point would be to read about [knockoffs](https://web.stanford.edu/group/candes/knockoffs/).

<p align="center">
  <img src="/images/feature_importance.png" width="600"><br><br>
  <em>Feature importance measures for unimportant explanatory variables (left) and hidden Markov model knockoffs (right). Knockoffs allow one to single out truly important variables while controlling the false discovery rate. Image from Sesia, Sabatti, and Candès. 2019.</em>
</p>

Relevant papers: [transfer learning with knockoffs](/publication/2021-transfer), [multi-environment knockoff filter](/publication/2021-mekf), [deep knockoffs](/publication/2019-deep-knockoffs), [HMM knockoffs](/publication/2019-hmm-knockoffs).

### Model-free predictive inference

An important objective of statistics is to predict future outcomes of a certain phenomenon given relevant past observations. 
Most existing approaches to this problem are either limited by relatively simple parametric models (whose validity may often be hard to justify in practice), or are based on complex algorithms that offer no statistical guarantees (and tend to be overconfident about the accuracy of their predictions).
I am interested in developing methods for model-free predictive inference that are both generally applicable and as efficient as possible. I seek this goal by combining statistical exchangeability ideas (e.g., [conformal inference](http://jmlr.csail.mit.edu/papers/volume9/shafer08a/shafer08a.pdf)) with machine learning.

<p align="center">
  <img src="/images/cqr.png" width="450"><br>
  <em>Prediction bands with guaranteed 90% coverage in a one-dimensional model-free regression problem, using conformal quantile regression. Image inspired by Romano, Patterson, and Candès. 2019.</em>
</p>

Relevant papers: [conformal prediction using conditional histograms](/publication/2021-chr), [testing for outliers with conformal p-values](/publication/2021-mot), [valid and adaptive classification](/publication/2020-classification), [a comparison of conformal quantile regression methods](/publication/2020-comparison-conformal).

## Methodology and applications

### Statistical genetics

Genome-wide association studies measure, from large numbers of people, hundreds of thousands of simple genetic mutations across the entire genome and compare them to interesting phenotypes (e.g., blood pressure, cholesterol levels, diabetes, and many other diseases), with the goal of better understanding the underlying biology and heritability.
From a statistician's perspective, this problem can at first be seen as a special instance of high-dimensional variable selection, although genetic data are extremely high-dimensional and display a particular structure (hidden Markov models) that raises unique challenges as well as opportunities.

<p align="center">
  <img src="/images/digital_twin.png" width="600"><br><br>
  <em>Visualization of a hidden Markov model for the genetic variables of an offspring conditional on the DNA of the parents. This model can be used to generate synthetic data for rigorous model-free inference. Image from Bates, Sesia, Candès, and Sabatti. 2020.</em>
</p>

Relevant papers: [transfer learning with knockoffs](/publication/2021-transfer), [multi-environment knockoff filter](/publication/2021-mekf), [KnockoffGWAS](/publication/2020-knockoffgwas), [KnockoffZoom](/publication/2020-knockoffzoom), [HMM knockoffs](/publication/2019-hmm-knockoffs), [causal inference from trio data](/publication/2020-trio-studies), [HMM knockoffs](/publication/2019-hmm-knockoffs).

### Collaborations

I enjoy collaborating on applied problems that involve statistics. 
I was also very involved with the [statistics consulting workshop at Stanford](https://statistics.stanford.edu/resources/consulting) and I look forward to building new collaborations at USC.

<p align="center">
  <img src="/images/knockoff_wavelets.png" width="500"><br><br>
  <em>Interpretable classification of bacterial Raman spectra using knockoff-filtered wavelet features. Image from Chia et al. 2021.</em>
</p>


Relevant papers: [bacterial classification from Raman spectra](/publication/2021-raman).
