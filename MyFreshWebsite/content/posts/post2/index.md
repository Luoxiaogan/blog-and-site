---
author: [Gan Luo]
title: "zeroth order optimization"
date: "2024-04-11"
description: "zeroth order optimization"
tags: ["optimization"]
ShowToc: true
math: true
draft: true
weight: 20
---

zeroth order optimization

1. single-point gradient estimator

$G_{f}(x,\delta,z)=\frac{n}{\delta}f(x+\delta z)z$，这个estimator 的期望是某种光滑化（smoothed version）之后的期望$f^{\delta}(x)=\int f(x+\delta y) \, v(dy)$，$\mathbb{E}[G_{f}(x,\delta,z)]=\nabla f^{\delta}(x)$，而且是一个unbiased estimator，对于$\nabla f$是baised

+ $\delta$ : smoothing radies

orthogonally invariant distribution如何去生成，正半轴上的分布（模长分布）和单位球面的均匀分布的卷积

the difference between the $\nabla f(x)$ and $\nabla^{\delta}f(x)$, 可以被连续性控制

缺点：varaince 被$\frac{1}{\delta^2}$阶控制，而$|| \nabla f(x)-\nabla^{\delta}f(x)||$被$\delta$控制，两者不可兼得，如何解决？

2. a way to variance reduction: two-point gradient estimator

这样的话，variance的upper bound 的包含$\delta$的部分是$\delta^2$阶，是好的

直观：当$\delta\to0$，就是随机的方向导数

$$a+b=10\\\\c+d=10$$

1. non-orthogonal-invariant distributions
gradient estimator 不再是某点的光滑化后的梯度了

$$V^*(s)=\max_a d \\\\ d \\\\ s$$
$$a$$

$$\begin{aligned}&s+s=10\\\\ &s+v+10=10\end{aligned}$$