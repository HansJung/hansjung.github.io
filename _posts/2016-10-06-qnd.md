---
layout: post
title: QnD to Machine Learning field
---

Last updated: 16/10/06


# Review strategy 

* Within 3 years 
* At least understandable Title. (If I don't even understand the title, then skip it) 

# AISTAT

__* Alan D. Saul et al., Chained Gaussian Process, AISTAT 2016__ 

* To overcome drawbacks in link function (used in modeling non-Gaussian data which requires invertibility and linear combinated parameters of interest), Chained GP is proposed for not requiring invertible and linearization only possible for multiple links (i,e,. chain).
* Survival data / Twitter data / Spatio-temporal data... 
* _keyword_ Gaussian Process 

__Zi Wang et al., Optimization as Estimation with Gaussian Processes in Bandit Settings, AISTAT 2016__

* Connection b/w GP-UCB and GP-PI by automatically and adaptively trading off exploration and exploitation. 
* _keyword_  Gaussian Process / Bandit 

__Raphael Feraud, Random Forest for the Contextual Bandit Problem, AISTAT 2016__  

* Bandit Forest with promising performance, low computational cost, and non-linear dependence. 
* _keyword_  Bandit Forest, Random Forest, Bandit 

# ICML 

__* Shuangfei Zhai, Deep Structured Energy Based models for anomaly detection, ICML 2016__ 

* Deep Structured Energy based Model (DSEBM) for anomaly detection on static, sequential, spatial data. 
* Proposed method is a training deep structured energy based models for the anomaly detection problem and extended EBMs to deep architectures with three types of structures: fully connected, recurrent and convolutional.
* _keyword_  Deep learning, Energy based model, Anomaly detection 

__Nihar B. Shah et al., No Oops, You Won’t Do It Again: Mechanisms for Self-correction in Crowdsourcing, ICML 2016__ 

* To mitigate the large errors in crowdsourcing labeled data, two-stage setting for self-correction algorithm is developed (Crowdsource is that the label is made by crowds). 
* _keyword_  Crowdsourced data 

__Chelsea Finn et al (Pieter Abbeel), Guided Cost Learning: Deep Inverse Optimal Control via Policy Optimization, ICML 2016__ 

* To define a cost function in reinforce learning, Inverse Optimal Control algorithm can be used to learn behaviors from demonstrations. 
* An inverse optimal control algorithm that can learn complex, nonlinear cost representations, such as neural networks, and can be applied to high-dimensional systems with unknown dynamics.
* _keyword_  Reinforce learning, Inverse Optimal Control, Bayesian optimization 
* _(To read)_ Levine, S., Popovic, Z., and Koltun, V. Nonlinear inverse reinforcement learning with gaussian processes. In Advances in Neural Information Processing Systems (NIPS), 2011.

__Uri Shaham et al., A Deep Learning Approach to Unsupervised Ensemble Learning, ICML 2016__

* Deep learning to crowdsourcing and unsupervised ensemble learning 
* Ensemble model == RBM --> Deep RBM 
* _keyword_  RBM, Deep learning 

__Pengtao Xie., Diversity-Promoting Bayesian Learning of Latent Variable Models, ICML 2016__

* Full Bayesian setting on Latent Variable Model (LVM) for capturing infrequent patterns on dataset.  
* _keyword_ Latent Variable Model, Diversity

__* Kirthevasan Kandasamy et al., Additive Approximations in High Dimensional
Nonparametric Regression via the SALSA, ICML 2016__
 
* General Additive Model approach for approximating High dimensional nonparametric regression. (Kernel ridge regression with an additive Kernel)
* _Keywords_ Kernel Ridge regression with additive Kernel 

__* Jan Hendrick Metzen, Minimum Regret Search for Single- and Multi-Task Optimization, ICML 2016__

* Novel acquisition function (based on minimum regret searching) for Bayesian Optimization 
* _Keyword_ Bayesian optimization

__The Variational Nystrom Method for Large-Scale Spectral Problems ¨__

--- 
# Machine Learning in Healthcare 

__Joseph Futoma et al., Scalable Modeling of Multivariate Longitudinal Data for Prediction of Chronic Kidney Disease Progression, MLH 2016__ 

*  Probabilistic generative model for multivariate longitudinal data that captures dependencies between multivariate trajectories. Gaussian process based regression model for each individual trajectory, and build off ideas from latent class models to induce dependence between their mean functions. 
*  _Keyword_ EHR data, GP, 