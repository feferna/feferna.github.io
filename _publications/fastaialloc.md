---
title: "FastAiAlloc: A real-time multi-resources allocation framework proposal based on predictive model and multiple optimization strategies"
collection: publications
category: manuscripts
permalink: /publication/fastaialloc
excerpt: ''
date: 2023-12-01
venue: 'Future Generation Computer Systems'
paperurl: 'https://www.sciencedirect.com/science/article/abs/pii/S0167739X23003126'
bibtexurl: 'https://feferna.github.io/files/bibtex/fastaialloc.bib'
citation: 'M. De S. Oliveira, F. E. Fernandes Junior, et al., “FastAiAlloc: A real-time multi-resources allocation framework proposal based on predictive model and multiple optimization strategies,” Future Generation Computer Systems, vol. 149, pp. 622–636, Dec. 2023, doi: 10.1016/j.future.2023.08.014.'
---

In cloud platforms, a common task is to allocate computational resources, e.g., memory and CPU, requested by applications and users. The allocation of these resources, which is an optimal load-balancing task, is considered an NP-Hard problem, being a challenging research area. There are many works proposed in the literature to address this problem. They use several strategies to deal with this optimization problem such as evolutionary algorithms, exact programming and also heuristics. However, some steps of the allocation process are not considered by these works, which are sometimes treated separately and not in an integrated manner. These steps include the applications and users resource consumption request profile as part of the optimization process and defining adequate metrics to check the optimized allocation. To integrate these steps, this work proposes a framework based on the following strategies, widely used in the literature: Genetic Algorithms (GA), Particle Swarm Optimization (PSO) and Linear Programming, besides our Heuristic approach. Furthermore, we restricted the resource allocation optimization to a real-time scenario, facilitating its use in an industrial process. In addition, Key Performance Indicators (KPIs) are proposed to carry out a comparative study in a public dataset. Our experiments showed that our proposed framework achieved better results than the baseline one, e.g., using a random allocation. In some cases, we observed an increase of almost 60% in performance compared with the baseline. In addition, when trying to balance memory and CPU consumption in the cluster, the linear approach performed the best, while the GA achieved the best result in allocating different user profiles across the cluster.

[Github Repository](https://github.com/marcosd3souza/fast-ai-alloc)
