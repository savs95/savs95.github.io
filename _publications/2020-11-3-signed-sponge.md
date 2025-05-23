---
title: "Regularized Spectral Methods for Clustering Signed Networks"
collection: publications
permalink: /publication/2020-11-03
excerpt:
date: 2020-11-03
venue: 'Preprint'
paperurl: 'https://arxiv.org/abs/2011.01737'
citation: 'Mihai Cucuringu, Apoorv Vikram Singh, Déborah Sulem, Hemant Tyagi. Regularized Spectral Methods for Clustering Signed Networks. In Submission.'
---
We study the problem of $k$-way clustering in signed graphs. Considerable attention in recent years has been devoted to analyzing and modeling signed graphs, where the affinity measure between nodes takes either positive or negative values. Recently, Cucuringu et al. [\[CDGT 2019\]](https://arxiv.org/abs/1904.08575) proposed a spectral method, namely SPONGE (Signed Positive over Negative Generalized Eigenproblem), which casts the clustering task as a generalized eigenvalue problem optimizing a suitably defined objective function. This approach is motivated by social balance theory, where the clustering task aims to decompose a given network into disjoint groups, such that individuals within the same group are connected by as many positive edges as possible, while individuals from different groups are mainly connected by negative edges. Through extensive numerical simulations, SPONGE was shown to achieve state-of-the-art empirical performance. On the theoretical front, [CDGT 2019] analyzed SPONGE and the popular Signed Laplacian method under the setting of a Signed Stochastic Block Model (SSBM), for $k=2$ equal-sized clusters, in the regime where the graph is moderately dense.
In this work, we build on the results in [\[CDGT 2019\]](https://arxiv.org/abs/1904.08575) on two fronts for the normalized versions of SPONGE and the Signed Laplacian. Firstly, for both algorithms, we extend the theoretical analysis in [\[CDGT 2019\]](https://arxiv.org/abs/1904.08575) to the general setting of $k \geq 2$ unequal-sized clusters in the moderately dense regime. Secondly, we introduce regularized versions of both methods to handle sparse graphs -- a regime where standard spectral methods underperform -- and provide theoretical guarantees under the same SSBM model. To the best of our knowledge, regularized spectral methods have so far not been considered in the setting of clustering signed graphs. We complement our theoretical results with an extensive set of numerical experiments on synthetic data.
