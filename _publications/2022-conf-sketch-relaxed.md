---
title: "Conformal Frequency Estimation using Discrete Sketched Data with Coverage for Distinct Queries"
collection: publications
permalink: /publication/2022-conf-sketch-relaxed
excerpt: ''
date: 2023-12-09
venue: 'Journal of Machine Learning Research'
---

**Abstract**

This paper develops conformal inference methods to construct a confidence interval for the frequency of a queried object in a very large discrete data set, based on a sketch with a lower memory footprint. This approach requires no knowledge of the data distribution and can be combined with any sketching algorithm, including but not limited to the renowned count-min sketch, the count-sketch, and variations thereof. After explaining how to achieve marginal coverage for exchangeable random queries, we extend our solution to provide stronger inferences that can account for the discreteness of the data and for heterogeneous query frequencies, increasing also robustness to possible distribution shifts. These results are facilitated by a novel conformal calibration technique that guarantees valid coverage for a large fraction of distinct random queries. Finally, we show our methods have improved empirical performance compared to existing frequentist and Bayesian alternatives in simulations as well as in examples of text and SARS-CoV-2 DNA data. 

[arXiv link](https://arxiv.org/pdf/2211.04612.pdf)
