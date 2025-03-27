---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
classes: wide custom-font
redirect_from:
  - /research
---

My research lies at the intersection of statistics and machine learning, with a focus on developing practical, reliable methods for analyzing complex, high-dimensional data. I aim to create tools that are not only statistically rigorous but also effective and broadly applicable in real-world settings—where data are often imperfect, and modeling assumptions rarely hold.

A unifying theme across my work is the development of distribution-free inference techniques that enable uncertainty quantification, robust variable selection, and structured prediction—especially in areas such as biomedical research, genetics, and machine learning systems.

## Core Methodology

### 🎯 Distribution-Free Predictive Inference

Accurately measuring the uncertainty of predictions is essential for the safe and reliable use of machine learning and AI systems—particularly in high-stakes applications. Yet many machine learning models produce predictions without indicating how confident they are, and when they do, that confidence is often misplaced. In contrast, traditional statistical methods place greater emphasis on uncertainty estimation, but they typically rely on unrealistic parametric assumptions about the data and impose rigid constraints on how predictions are computed—making them poorly suited to the complexity of modern machine learning.

A central focus of my research is to address this challenge by developing more flexible statistical tools for model-free predictive inference, also known as [conformal inference](http://jmlr.csail.mit.edu/papers/volume9/shafer08a/shafer08a.pdf). These methods provide statistically valid measures of uncertainty for the predictions of any machine learning model—without relying on strong assumptions about the structure of the data or the way predictions are generated.

<p align="center">
  <img src="/assets/images/cifar10.png" width="700"><br>
  <em>Conformal prediction sets for test images from CIFAR-10. Left: clean image of a ship. Right: corrupted image of a dog. From Einbinder, Romano, Sesia, and Zhou (2022).</em>
</p>

---

### 🔍 High-Dimensional Variable Selection

Modern data sets are often very large and complex, containing thousands—or in some cases even millions—of explanatory variables that might be related to a particular outcome of interest. While it's increasingly easy to collect and store large volumes of data, identifying which variables are truly relevant remains extremely challenging. In many cases, we are trying to understand intricate, high-dimensional phenomena, and finding the key signals is like searching for a few needles in a very large haystack. This setting calls for statistical tools that can effectively sift through noisy, high-dimensional data to discover meaningful relationships powerfully but without being misled by spurious patterns.

A major focus of my research is on developing statistically rigorous methods for variable selection that remain reliable even in these complex environments. In particular, I have worked extensively with a framework known as [knockoffs](https://web.stanford.edu/group/candes/knockoffs/), which enables powerful and flexible feature selection while controlling the false discovery rate. These tools help ensure that the discoveries we make from high-dimensional data are not only interesting but also scientifically trustworthy.

<p align="center">
  <img src="/assets/images/feature_importance.png" width="600"><br><br>
  <em>Feature importance for irrelevant variables (left) and HMM knockoffs (right). From Sesia, Sabatti, and Candès (2019).</em>
</p>

---

### 📊 Data Sketching and Frequency Recovery

In the era of big data, extracting reliable insights from massive, high-dimensional data sets often requires operating under significant computational or storage constraints. In such settings, raw data sometimes need to be compressed or summarized in ways that inevitably lose some information. I have developed methods for recovering key insights from lossily compressed, discrete data using sketched data structures. This work draws on ideas from Bayesian modeling and conformal inference to enable meaningful uncertainty quantification, and reflects a broader aim of my research: bridging concepts across different areas of statistics and computer science to create practical, robust tools for modern data science.

---

## Application-Driven Methodology

### 🧬 Statistical Genetics

Many important human traits and diseases—such as height, cholesterol levels, or diabetes risk—are heritable yet poorly understood, as they are influenced by the subtle interplay of thousands of genetic variants. These are known as *complex traits*, and uncovering their genetic basis is one of the central goals of genome-wide association studies (GWAS). Statistically, this presents a high-dimensional variable selection problem: we aim to identify a small number of relevant genetic markers from among hundreds of thousands of possibilities, all while accounting for intricate correlations between them due to linkage disequilibrium and confounding from population structure.

A major contribution of my work in this area is [KnockoffGWAS](https://msesia.github.io/knockoffgwas/index.html), a method for genome-wide variable selection that enables statistically rigorous discoveries under false discovery rate control, even in the presence of complex genetic structure. 
 This method is carefully designed to ensure that findings are not only statistically valid, but also likely to be biologically meaningful.
This research is closely connected to my broader interest in developing tools for powerful and reliable distribution-free statistical inference with very high-dimensional data.


<p align="center">
  <img src="/assets/images/digital_twin.png" width="600"><br><br>
  <em>Hidden Markov model of an offspring's genotype conditional on parental DNA. Enables synthetic data generation for inference. From Bates, Sesia, Candès, and Sabatti (2020).</em>
</p>

---

### 🩺 Biomedical Collaborations

I have collaborated on a range of applied research projects in biomedicine and clinical science, where data are often messy, high-dimensional, and collected under real-world constraints. In several of these studies, I worked directly with complex patient records and biomedical measurements—developing and applying statistical methods to extract reliable insights from noisy and heterogeneous data.

These projects have reinforced the importance of practical data skills—such as data cleaning, model selection, and close collaboration with domain experts—in addition to statistical innovation. They exemplify my broader goal of creating and using methods that are not only theoretically sound but also effective in the kinds of challenging, high-stakes environments where decisions matter.

<p align="center">
  <img src="/assets/images/knockoff_wavelets.png" width="500"><br><br>
  <em>Interpretable classification of bacterial Raman spectra using knockoff-filtered wavelet features. From Chia et al. (2021).</em>
</p>

---

### 🧠 Language Models

I am beginning to explore **uncertainty estimation in large language models (LLMs)** — a fast-growing area that connects naturally with conformal prediction and calibration techniques.
