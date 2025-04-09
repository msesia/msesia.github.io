---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
classes: wide custom-font
redirect_from:
  - /research
---

## Research Overview

> **Jump to:**  
> - [Reproducible Variable Selection](#-reproducible-variable-selection)  
> - [Uncertainty Quantification](#-uncertainty-quantification)  
> - [Data Sketching and Frequency Recovery](#-data-sketching-and-frequency-recovery)  
> - [Statistical Genetics](#-statistical-genetics)  
> - [Biomedical Collaborations](#-biomedical-collaborations)  
> - [Uncertainty Estimation for Language Models](#-uncertainty-estimation-for-language-models)

---

My research focuses on developing practical and rigorous statistical methods for analyzing complex, high-dimensional data using modern machine learning algorithms, particularly in settings where traditional modeling assumptions may not hold. These challenges have become increasingly important as data sets grow in scale and complexity, and as rapidly evolving artificial intelligence (AI) and machine learning models are used to drive scientific discoveries and inform decisions across a wide range of high-impact domains.

A central theme in my work is *distribution-free* and *model-agnostic* inference. These methods avoid strong or unrealistic assumptions about how data are generated or how models operate, making them especially well suited for complex, real-world applications. I have developed techniques that work in tandem with modern machine learning models to identify meaningful patterns, ensure reproducibility, and quantify uncertainty.

Because these tools are grounded in fundamental statistical principles rather than tied to any specific model or data distribution, they are broadly applicable and designed to remain relevant as AI technologies continue to evolve. This makes them particularly valuable in settings where results obtained from AI models must be transparent, trustworthy, and scientifically defensible.

#### Key areas of focus:

- **Reproducible Variable Selection.**  Determining which variables in a high-dimensional dataset are truly associated with an outcome—rather than merely correlated due to noise or confounding—is essential for interpretability and scientific validity. My work develops statistical tools that help distinguish meaningful relationships from spurious ones, enabling more robust conclusions from complex models. This is especially important in domains such as genomics, neuroscience, and biomedicine, where identifying potentially causal factors is central to advancing scientific understanding.

- **Uncertainty Quantification.**  Understanding how confident we can be in a model’s predictions is critical for using that model effectively and responsibly. My work provides methods to assess and report uncertainty in complex models, making AI-driven insights more reliable and defensible. This is particularly vital in high-stakes areas such as healthcare, finance, and law, where decisions based on predictions must be backed by clear, well-calibrated measures of risk.

#### Applied Work and Collaboration

Beyond academic research, I serve as a consultant and expert collaborator in both academic and industry settings. I specialize in developing tailored statistical solutions, designing transparent and reproducible analyses, quantifying uncertainty in complex models, and clearly communicating statistical reasoning to diverse audiences. My work is especially relevant in contexts where flexible, data-driven models are deployed—but any errors may carry high costs and rigorous, defensible methodology is therefore essential.



---

## Core Methodology

### 🔍 Reproducible Variable Selection {#reproducible-variable-selection}

Modern data sets can include thousands or even millions of variables potentially related to an outcome of interest. Identifying which variables are truly relevant—rather than spuriously correlated due to noise or confounding—is a major statistical challenge. This task becomes especially difficult in high-dimensional settings, where the number of variables far exceeds the number of observations, and in heterogeneous populations, where relationships between predictors and outcomes may vary across subgroups. Addressing these complexities often requires flexible models capable of capturing diverse and subtle patterns in the data. However, if applied without proper statistical safeguards, such models are particularly prone to overfitting and can yield misleading or non-reproducible findings.


A major focus of my research is on developing *distribution-free* and *model-agnostic* tools for variable selection that can harness the predictive power of modern machine learning algorithms while ensuring reproducibility and interpretability. These methods are designed to uncover meaningful structure in complex data and to ensure that the selected variables reflect robust and practically significant relationships. In particular, I have worked extensively with the [knockoffs framework](https://web.stanford.edu/group/candes/knockoffs/), which enables powerful and flexible feature selection while controlling the false discovery rate. Because it does not rely on specific modeling assumptions, this approach is especially effective when paired with black-box machine learning models, supporting more reliable, interpretable, and scientifically defensible conclusions.


<p align="center">
  <img src="/assets/images/feature_importance.png" width="600"><br><br>
  <em>Feature importance for irrelevant variables (left) and HMM knockoffs (right). From Sesia, Sabatti, and Candès (2019).</em>
</p>


### 🎯 Uncertainty Quantification {#uncertainty-quantification}

Machine learning models often produce predictions without reliable information about how confident we should be in their accuracy. This lack of trustworthy uncertainty estimates can make model outputs misleading and limits their applicability in high-stakes domains where decisions must be supported by defensible statistical reasoning. While traditional statistical methods emphasize uncertainty quantification, they typically rely on rigid or unrealistic assumptions that do not hold in many modern applications—particularly when working with complex, high-dimensional data or modern machine learning models.

A central focus of my research is developing flexible, *distribution-free* and *model-agnostic* tools for predictive uncertainty, such as [conformal inference](http://jmlr.csail.mit.edu/papers/volume9/shafer08a/shafer08a.pdf). These methods can provide statistically rigorous and intuitively interpretable measures of uncertainty for the predictions produced by any machine learning model—regardless of its internal structure—without requiring strong assumptions about the underlying data distribution. This makes them particularly valuable for enhancing transparency, reliability, and accountability in AI systems used for real-world decision-making.


<p align="center">
  <img src="/assets/images/cifar10.png" width="700"><br>
  <em>Conformal prediction sets for test images from CIFAR-10. Left: clean image of a ship. Right: corrupted image of a dog. From Einbinder, Romano, Sesia, and Zhou (2022).</em>
</p>



### 📊 Data Sketching and Frequency Recovery {#data-sketching}

In some very large-scale data analysis settings, storing or processing full datasets is often computationally infeasible. In such cases, data are often compressed or summarized, which poses unique challenges for statistical inference. My work in this area focuses on recovering key signals and estimating uncertainty from compressed or lossily stored data, using sketching techniques combined with ideas from Bayesian modeling and distribution-free inference.

These methods help preserve the integrity of statistical analysis even when working with limited computational resources or streaming data. They reflect my broader goal of developing robust, principled statistical tools that remain reliable under practical constraints, and can scale with the demands of real-world AI systems.

---

## Applied Methodology

### 🧬 Statistical Genetics {#statistical-genetics}

Understanding the genetic basis of complex traits—such as blood pressure, cholesterol levels, or diabetes risk—requires identifying meaningful associations among hundreds of thousands of genetic variants. Statistically, this poses a difficult high-dimensional variable selection problem, further complicated by the strong dependencies characteristic of genomic data, including population structure and linkage disequilibrium.

To address these challenges, I developed a statistical framework that culminated in [KnockoffGWAS](https://msesia.github.io/knockoffgwas/index.html), a powerful *distribution-free* and *model-agnostic* method for genome-wide association studies. This approach provides rigorous false discovery rate control while carefully accounting for complex genetic dependencies. It enables reproducible, interpretable discoveries that are both statistically sound and likely to be biologically meaningful.

This line of work demonstrates how flexible inference techniques can be integrated with machine learning tools to address the scale and complexity of modern genomic data, while maintaining the statistical guarantees necessary for trustworthy scientific conclusions.


<p align="center">
  <img src="/assets/images/digital_twin.png" width="600"><br><br>
  <em>Hidden Markov model of an offspring's genotype conditional on parental DNA. Enables synthetic data generation for inference. From Bates, Sesia, Candès, and Sabatti (2020).</em>
</p>


### 🩺 Biomedical Collaborations {#biomedical-collaborations}

Many biomedical datasets are messy, heterogeneous, and collected under real-world constraints. These conditions challenge conventional statistical methods and call for flexible tools that are both robust and reproducible. I have collaborated on a range of such projects involving complex patient records, clinical measurements, and diagnostic data, applying rigorous statistical inference to extract reliable insights from imperfect data.

These collaborations highlight the importance of integrating domain expertise with methodological innovation. My contributions typically involve designing customized statistical solutions in close partnership with subject-matter experts to ensure that analyses are both scientifically meaningful and statistically defensible.


<p align="center">
  <img src="/assets/images/knockoff_wavelets.png" width="500"><br><br>
  <em>Interpretable classification of bacterial Raman spectra using knockoff-filtered wavelet features. From Chia et al. (2021).</em>
</p>


### 🧠 Uncertainty Estimation for Language Models {#llms}

Large language models (LLMs) have achieved remarkable success in recent years and are now widely used across a range of applications—including many that involve sensitive or high-stakes decisions. However, these models still make errors and often struggle to provide reliable assessments of how confident they are in their outputs. This lack of trustworthy uncertainty estimation can lead to overconfidence in incorrect predictions, making it difficult to use LLMs responsibly in contexts where reliability, transparency, and accountability are essential.

I am beginning to explore how specialized *distribution-free* and *model-agnostic* statistical inference methods can be applied to LLMs to make their outputs more transparent and trustworthy. This line of work builds on my broader research in predictive uncertainty for machine learning models, while addressing new challenges that are unique to language models—such as variable-length outputs, ambiguity in natural language, and the need for meaningful confidence measures across a wide range of tasks.

