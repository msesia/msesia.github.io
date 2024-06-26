---
title: "Conformal inference is (almost) free for neural networks trained with early stopping"
collection: publications
permalink: /publication/2023-early-stopping
excerpt: ''
date: 2023-01-30
venue: 'Proceedings of the 40th International Conference on Machine Learning'
---

**Abstract**

Early stopping based on hold-out data is a popular regularization technique designed to mitigate overfitting and increase the predictive accuracy of neural networks. Models trained with early stopping often provide relatively accurate predictions, but they generally still lack precise statistical guarantees unless they are further calibrated using independent hold-out data. This paper addresses the above limitation with conformalized early stopping: a novel method that combines early stopping with conformal calibration while efficiently recycling the same hold-out data. This leads to models that are both accurate and able to provide exact predictive inferences without multiple data splits nor overly conservative adjustments. Practical implementations are developed for different learning tasks -- outlier detection, multi-class classification, regression -- and their competitive performance is demonstrated on real data. 

[arXiv link](https://arxiv.org/pdf/2301.11556.pdf)