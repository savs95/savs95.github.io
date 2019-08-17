---
title: "Approximation Algorithms for Cost-Balanced Clustering"
collection: publications
permalink: /publication/2009-10-01-cost-balanced
excerpt:
date: 2019-07-17
venue: 'Preprint'
#paperurl:
citation: 'Amit Deshpande, Anand Louis, Deval Patel, Apoorv Singh'
---
Clustering points in the Euclidean space is a fundamental problem in the theory of algorithms
and in unsupervised learning.
Various clustering objectives to quantify the quality of clustering have been proposed and studied;
the $k$-means and $k$-median clustering objective are the most popular ones.
In some cases, the $k$-means or the $k$-median objective may result in a few clusters of very large cost and many clusters of extremely small cost. Even when the optimal clusters are balanced in size, some of them may have a huge variance. This is undesirable for quantization or when we have a budget constraint on the cost of each cluster.
Motivated by this, we study the cost-balanced $k$-means and the cost-balanced $k$-median problem.
For a $k$-clustering $O_1, \ldots, O_k$ of a given set of $n$ points $X \subset \mathbb R^d$,
we define its cost-balanced $k$-means cost as:    
<center> $ \boxed{\mathcal K ({O_1, \ldots, O_k}) \stackrel{def}{=} \max_{l \in [k]} \sum_{x \in O_l} \left\lVert{x - \mu_l}\right\rVert^2,
\qquad \textrm{where } \mu_l = \frac{1}{\left\lvert{O_l}\right\rvert} \sum_{x \in O_l} x ~} $ </center>
In other words, we want to minimize the cost of the heaviest cluster or balance the cost of each cluster.
For any $\varepsilon > 0$, we give a randomized algorithm with running time $\mathcal O\big({2^{poly \big({k/\varepsilon}\big)} n d }\big)$ that gives a $(1+\varepsilon)$-approximation to the optimal cost-balanced $k$-means and the similarly defined optimal cost-balanced $k$-median clustering, using $k$ clusters, with a constant probability. We define a more general version of the $k$-median clustering and the cost-balanced $k$-median clustering, and we name them $\ell_p$ cost $k$-clustering and $\ell_p$ cost-balanced $k$-clustering, respectively.
Given a black-box algorithm which gives a constant factor approximation to the $\ell_p$ cost $k$-clustering, we show a procedure that runs in time $poly(n,k,p)$ which gives a bi-criteria $\mathcal O\big({1/\varepsilon^{1/p}}\big)$-approximation to the optimal $\ell_p$ cost-balanced $k$-clustering, using $(1+\varepsilon)k$ clusters.
