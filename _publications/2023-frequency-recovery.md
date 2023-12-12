---
title: "Frequency and cardinality recovery from sketched data: a novel approach bridging Bayesian and frequentist views"
collection: publications
permalink: /publication/2023-frequency-recovery
excerpt: ''
date: 2023-09-27
venue: 'pre-print'
---

**Abstract**

We study how to recover the frequency of a symbol in a large discrete data set, using only a compressed representation, or sketch, of those data obtained via random hashing. This is a classical problem in computer science, with various algorithms available, such as the count-min sketch. However, these algorithms often assume that the data are fixed, leading to overly conservative and potentially inaccurate estimates when dealing with randomly sampled data. In this paper, we consider the sketched data as a random sample from an unknown distribution, and then we introduce novel estimators that improve upon existing approaches. Our method combines Bayesian nonparametric and classical (frequentist) perspectives, addressing their unique limitations to provide a principled and practical solution. Additionally, we extend our method to address the related but distinct problem of cardinality recovery, which consists of estimating the total number of distinct objects in the data set. We validate our method on synthetic and real data, comparing its performance to state-of-the-art alternatives. 


[Download paper here](https://arxiv.org/pdf/2309.15408.pdf)