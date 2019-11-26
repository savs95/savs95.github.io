---
title: 'A Note About Sparse Optimization'
date: 2019-11-26
permalink: /posts/2019/11/sparse-optz/
tags:
  - sparse optimization
  - regularization
---

For an under-determined system of linear equations, there exists infinitely many solutions. However, with more information, for example, if we know the the optimal solution is sparse, we can recover the desired solution.

There are also cases where we are interested in the sparse solution. For such problems we generally introduce a regularizer, to force the solution to be sparse:  
<center> $ \min_{\theta} ~ $ loss$ (\theta, $ data) $ + ~ \lambda $ regularizer $ (\theta) .$ </center>   


One of the most popular choice for a regularizer is the $ \ell_1 $ norm regularization (when $ \theta $ is a vector) or nuclear norm regularization (when $ \theta $ is a matrix). I used to think that $ \ell_1 $ regularization makes sense because it is the tightest convex-relaxation to the corresponding  objective function with $ \ell_0 $ function regularization (which makes the problem non-convex).
However, in a talk by [Venkat Chandrasekaran](http://users.cms.caltech.edu/~venkatc/), I came to know that I was essentially wrong.
The tightest convex relaxation of objective with the $ \ell_0 $ function regularization need not be the $ \ell_1 $ regularization. Suppose the problem at hand was:

<center> $ \min_{\theta} ~ $ loss$ (\theta, $ data) $ + ~ \lambda \ell_0 (\theta) .$ </center>

Let the optimum value of this (non-convex) optimization problem be $ OPT $. Suppose the tightest convex relaxation of this problem is:  

<center> $ \min_{\theta} ~ $ loss$ (\theta, $ data) $ + ~ \lambda \ell_c (\theta) .$ </center>

Let the optimum value of this optimization problem be $ OPT_c $. The solution returned by this convex optimization need not be the sparsest. In fact, it could be the case that the sparsest solution is returned by this optimization problem:

<center> $ \min_{\theta} ~ $ loss$ (\theta, $ data) $ + ~ \lambda \ell_1 (\theta) .$ </center>

Let the optimum value of this objective function be $ OPT_1 $.

The above scenario could be be true because convex relaxation guarantees nothing about sparsity of the solution. It only tells that $ OPT $ is closer to $ OPT_c $ than $ OPT_1 $. Turns out, in many cases, $ \ell_1 $-regularization forces the solution to be on the "low-dimensional" face of the polytope formed by the "atoms" (see [Convex Geometry of Linear Inverse Problems](https://arxiv.org/pdf/1012.0621.pdf)).  

I also attended a [talk](http://seminaire.univ-lille1.fr/node/414) by [Dr Arthur Mensch](https://www.amensch.fr/), where he showed [an example](https://arxiv.org/pdf/1802.03676.pdf) (in the section on Smoothed max operators) where $ \ell_2^2 $ regularization lead to the sparsest solution! 
