---
title: "Random measure priors in Bayesian frequency recovery from sketches"
collection: publications
permalink: /publication/2024-random-measure-priors
excerpt: ''
date: 2024-06-24
venue: 'Journal of Machine Learning Research (2024)'
---

**Abstract**

This paper introduces a Bayesian nonparametric approach to frequency recovery from lossy-compressed discrete data, leveraging all information contained in a sketch obtained through random hashing. By modeling the data points as random samples from an unknown discrete distribution endowed with a Poisson-Kingman prior, we derive the posterior distribution of a symbol's empirical frequency given the sketch. This leads to principled frequency estimates through mean functionals, e.g., the posterior mean, median and mode. We highlight applications of this general result to Dirichlet process and Pitman-Yor process priors. Notably, we prove that the former prior uniquely satisfies a sufficiency property that simplifies the posterior distribution, while the latter enables a convenient large-sample asymptotic approximation. Additionally, we extend our approach to the problem of cardinality recovery, estimating the number of distinct symbols in the sketched dataset. Our approach to frequency recovery also adapts to a more general ``traits'' setting, where each data point has integer levels of association with multiple symbols, typically referred to as ``traits''. By employing a generalized Indian buffet process, we compute the posterior distribution of a trait's frequency using both the Poisson and Bernoulli distributions for the trait association levels, respectively yielding exact and approximate posterior frequency distributions. 


[Download paper here](https://arxiv.org/pdf/2303.15029.pdf)
