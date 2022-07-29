---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

![FamilyAtWapatki](\files\Pics\FamilyAtWapatki.jpg)

Currently, I am a Ph.D. candidate at the University of Arizona in the Applied Math Graduate Interdisciplinary Program (GIDP). I received a master's degree in math from Brigham Young University (BYU) in 2016. I have a wife and three children.

## Research

Broadly I am interested in stochastic modeling. Currently I am studying data-driven models and model reduction. For my [master's thesis](https://scholarsarchive.byu.edu/etd/6023/). I studied the steady state configuration of a small group of cells connected by cadherin sites.

### Current Research Project

From power grids to epidemics, scientists and engineers use mathematical models to simulate,
predict, and control complex systems. Traditionally, such models are often derived from first
principles. For example, to model the weather, one might start with the relevant physical laws
and derive a mathematical model (in the form of large systems of differential equations). Such
models are built on clear conceptual foundations and can achieve great accuracy when all the
relevant physical principles are known. But they often require resolving small-scale details in
order to make accurate predictions. Again using weather as an example, for regional weather
forecasting, it may be necessary to resolve variations in temperature, pressure, etc., down to a
scale of kilometers, even when the modeler is only interested in large-scale weather patterns.
This makes first-principles models sometimes very expensive to use. Moreover, they may require
variables that are hard to measure, and very often not all relevant physics are completely
understood. As a complementary approach, many modelers have turned to machine learning
(ML), which uses general mathematical models with many tunable parameters, which are
adjusted to optimally fit available data. The fitting, or training, of the model can be
computationally expensive, but need only be done once; the resulting, more efficient model can
be used repeatedly. However, machine-learned models can be opaque and hard to interpret.

To retain the interpretability of first-principles models and the efficiency of ML, there is currently
much effort in the computational science and engineering community in a combined approach:
start with a “rough” first-principles model of only the features of interest, then leverage the power
of ML to incorporate the dynamical effects of fine-scale features. Such a combined approach
has been shown to be effective in a variety of test problems. However, to make these methods
practical, there are numerous challenges to overcome. One is that these ML-assisted models
may not be robust or stable: they can give unrealistic outputs when inputs are only varied
slightly. Another issue is that the training process may be computationally costly.

I am using a novel combination of ideas from signal processing, modern numerical linear
algebra, and statistical mechanics to address these challenges. Specifically, I am designing
methods to pre-process data so as to accelerate model training. Since this issue arises in many
applications of ML to so-called time series data, this work can be expected to impact many
applications. Robustness and stability, too, are general issues for many ML problems, and I
expect my work to improve the practical utility of these methods and, at the same time, lead to a
deeper mathematical understanding of these issues.
