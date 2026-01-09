---
title: "Pruning of Generative Adversarial Neural Networks for Medical Imaging Diagnostics with Evolution Strategy"
collection: publications
category: manuscripts
permalink: /publication/pruning-of-gans-for-med
excerpt: ''
date: 2021-01-26
venue: 'Information Sciences'
paperurl: 'https://www.sciencedirect.com/science/article/abs/pii/S0020025521000189'
bibtexurl: 'https://feferna.github.io/files/bibtex/pruning-of-gans-for-med.bib'
citation: 'F. E. Fernandes Junior and G. G. Yen, “Pruning of generative adversarial neural networks for medical imaging diagnostics with evolution strategy,” Information Sciences, vol. 558, pp. 91–102, May 2021, doi: 10.1016/j.ins.2020.12.086.'
---

Deep Convolutional Neural Networks (DCNNs) have the potential to revolutionize the field of Medical Imaging Diagnostics due to their capabilities of learning by using only raw data. However, DCNNs can only learn when trained using thousands of data points, which is not always available when dealing with medical data. Moreover, due to patient privacy concerns and the small prevalence of certain diseases in the population, medical data often presents unbalanced classes and fewer data points than other data types. Researchers often rely on Generative Adversarial Networks (GANs) to synthesize more data from a given distribution to solve this problem. Nevertheless, GANs are computationally intensive models requiring the use of powerful hardware to run. In the present work, an algorithm for pruning GANs based on Evolution Strategy (ES) and Multi-Criteria Decision Making (MCDM) is proposed in which a model with the best trade-off between computational complexity and synthesis performance can be found without the use of any trade-off parameter. In the proposed algorithm, the model with the best trade-off is defined geometrically as the candidate solution with the minimum Manhattan distance (MMD) in a two-dimensional objective space established by the number of Floating-Point Operations (FLOPs) and the Wasserstein distance of all candidate solutions, also known as the knee solution. The results show that the pruned GAN model achieves similar performance compared with the original model with up to 70% fewer Floating-Point Operations.
