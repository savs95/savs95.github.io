---
title: "Euclidean k-Means with Center Proximity"
collection: talks
type: "Talk"
permalink: /talks/2019-10-15-inria-kmeans
venue: "INRIA Lille"
date: 2019-10-15
location: "Lille, France"
---
Gave a talk at the INRIA Lille on our work on clustering Euclidean $ k $-Means with Center Proximity [Link to the announcement](https://modal.lille.inria.fr/wikimodal/doku.php?id=seminars).  

**Abstract**: Clustering is an important tool in any data science toolkit. Most popular clustering algorithms partition the given data into disjoint clusters by optimizing a certain global objective such as the k-means. The implicit assumption in doing so is that an optimal solution for this objective would recover the underlying ground truth clustering. However, many such objectives are NP-hard to optimize in the worst case, e.g., k-center, k-median, k-means. Moreover, an optimal solution need not satisfy certain properties desired from the ground truth clustering, e.g., balance, stability. In practice, however, Lloyd’s algorithm, k-means++, and their variants perform well on most real-world data sets. This dichotomy between theoretical intractability and empirically observed efficiency has led to the CDNM thesis: “Clustering is Difficult only when it does Not Matter”! In most real-world data sets, the underlying ground-truth clustering is unambiguous and stable under small perturbations of data. We will highlight these issues with the example of k-means clustering. In this talk, we will explore a notion of stability called center-proximity and give an algorithm and lower bounds for stable instances. This is joint work with Dr Amit Deshpande (Microsoft Research, India) and Dr Anand Louis (Indian Institute of Science, India).

[Find the slides here](/files/inria_ppt.pptx).
