---
title: 'Blog Post number 1'
date: 2021-11-1
permalink: /posts/2021/11/tech_spec_SoftTree/
tags:
  - BART
  - Tree
  - Algorithm
  - Soft Decision
---

This is one of the work in Bayesian Additive Regression Tree (BART) technical specification series. In this post, I will focus on the details of soft decision trees and show how it improves the model. To understand the content, some knowledge in decision tree is required.

Soft Decision Tree 
======
The Soft-BART was proposed by AL (2018) by adopting the idea in Irsoy’s paper in 2012. The key idea is:

at the internal nodes we choose both children with probabilities
given by a sigmoid gating function. In the canonical hard binary decision tree, each node applies a *hard
decision* and choose one of the children accordingly. In the soft decision tree, all children are selected
with certain probability. That is, we follow all the paths to all the leaves and all the leaves contribute
to the final decision but with different probabilities. One instance will be redirects to all the children
leaves with probabilities calculated by a *gating function*.

$$
  \int_0^\infty \frac{x^3}{e^x-1}\,dx = \frac{\pi^4}{15}
$$

Aren't headings cool?
------
