---
title: "Automatic Searching and Pruning of Deep Neural Networks for Medical Imaging Diagnostic"
collection: publications
category: manuscripts
permalink: /publication/automatic-searching-pruning-med
excerpt: ''
date: 2020-10-03
venue: 'IEEE Transactions on Neural Networks and Learning Systems'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/9222548'
bibtexurl: 'https://feferna.github.io/files/bibtex/automatic-searching-pruning-med.bib'
citation: 'F. E. Fernandes Junior and G. G. Yen, “Automatic Searching and Pruning of Deep Neural Networks for Medical Imaging Diagnostic,” IEEE Trans. Neural Netw. Learning Syst., pp. 1–11, 2020, doi: 10.1109/TNNLS.2020.3027308.'
---

The field of medical imaging diagnostic makes use of a modality of imaging tests, e.g., X-rays, ultrasounds, computed tomographies, and magnetic resonance imaging, to assist physicians with the diagnostic of patients’ illnesses. Due to their state-of-the-art results in many challenging image classification tasks, deep neural networks (DNNs) are suitable tools for use by physicians to provide diagnostic support when dealing with medical images. To further advance the field, the present work proposes a two-phase algorithm capable of automatically generating compact DNN architectures given a database, called here DNNDeepeningPruning. In the first phase, also called the deepening phase, the algorithm grows a DNN by adding blocks of residual layers one after another until the model overfits the given data. In the second phase, called the pruning phase, the algorithm prunes the created DNN model from the first phase to produce a DNN with a small amount of floating-point operations guided by some preference given by the user. The proposed algorithm unifies the two separate fields of DNN architecture searching and pruning under a single framework, and it is tested in two medical imaging data sets with satisfactory results.
