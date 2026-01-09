---
title: "Convolutional neural network-based embarrassing situation detection under camera for social robot in smart homes"
collection: publications
category: manuscripts
permalink: /publication/embarrasing-detection-sensors
excerpt: ''
date: 2018-05-10
venue: 'Sensors'
paperurl: 'https://www.mdpi.com/1424-8220/18/5/1530'
bibtexurl: 'https://feferna.github.io/files/bibtex/embarrasing-detection-sensors.bib'
citation: 'G. Yang, J. Yang, W. Sheng, F. E. Fernandes Junior, and S. Li, “Convolutional Neural Network-Based Embarrassing Situation Detection under Camera for Social Robot in Smart Homes,” Sensors, vol. 18, no. 5, p. 1530, May 2018, doi: 10.3390/s18051530.'
---

Recent research has shown that the ubiquitous use of cameras and voice monitoring equipment in a home environment can raise privacy concerns and affect human mental health. This can be a major obstacle to the deployment of smart home systems for elderly or disabled care. This study uses a social robot to detect embarrassing situations. Firstly, we designed an improved neural network structure based on the You Only Look Once (YOLO) model to obtain feature information. By focusing on reducing area redundancy and computation time, we proposed a bounding-box merging algorithm based on region proposal networks (B-RPN), to merge the areas that have similar features and determine the borders of the bounding box. Thereafter, we designed a feature extraction algorithm based on our improved YOLO and B-RPN, called F-YOLO, for our training datasets, and then proposed a real-time object detection algorithm based on F-YOLO (RODA-FY). We implemented RODA-FY and compared models on our MAT social robot. Secondly, we considered six types of situations in smart homes, and developed training and validation datasets, containing 2580 and 360 images, respectively. Meanwhile, we designed three types of experiments with four types of test datasets composed of 960 sample images. Thirdly, we analyzed how a different number of training iterations affects our prediction estimation, and then we explored the relationship between recognition accuracy and learning rates. Our results show that our proposed privacy detection system can recognize designed situations in the smart home with an acceptable recognition accuracy of 94.48%. Finally, we compared the results among RODA-FY, Inception V3, and YOLO, which indicate that our proposed RODA-FY outperforms the other comparison models in recognition accuracy.
