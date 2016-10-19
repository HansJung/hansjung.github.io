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

__Markus Heinonen et al., Non-Stationary Gaussian Process Regression with Hamiltonian Monte Carlo, AISTAT 2016__

* Non-stationary GP regression framework with MCMC. 
* _Idea_ This framework can be used in GP modeling of ECG data. It can be furtherly extended to personalized ECG modeling. 

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

__* Andrew Lan et al., Dealbreaker: A Nonlinear Latent Variable Model for Educational Data, ICML 2016__

* Not only modeling with probabilistic model, but also gain some insights about student responses. 
* _Keyword_ Student response model
* _Idea_ We can use this model to healthcare application 

__Dongsheng Li et al., Low-Rank Matrix Approximation with Stability, ICML 2016__

* Low rank matrix approximation for stability 
* _Keyword_ Low rank matrix approximation 
* _Idea_ With personalized medication data, we can use this algorithm for recommendation system 

__Roy J. Adams et al., Hierarchical Span-Based Conditional Random Fields for Labeling and Segmenting Events in Wearable Sensor Data Streams, ICML 2016__

* In mobile health, a hierarchical
span-based conditional random field model
for the key problem of jointly detecting discrete
events in such sensor data streams and segmenting
these events into high-level activity sessions.
* We apply the model to the problems of
smoking and eating detection using four real data
sets.

__Yunseong Hwang et al.,Automatic Construction of Nonparametric Relational Regression Models for Multiple Time Series, ICML 2016__

* Automatic Bayesian Covariance Discovery (ABCD). New Kernel learning methods which can model multiple time-series data sets by finding common, shared causes of changes are proposed.  
* _Keyword_ Kernel learning 
* _Iead_ Anomaly detection? (GP-based) 

__Jie Shen et al., Online Low-rank subspace clustering by Basis Dictionary, ICML 2016__

* Low-Rank Representation is useful in segmentating data that are generated from a union of subspaces. 
* Online implementation of LRR. 
* _Keyword_ LRR / Clustering
* _Idea_ Personalized medicaiton in online manner. 


--- 

# Machine Learning in Healthcare 

__* Joseph Futoma et al., Scalable Modeling of Multivariate Longitudinal Data for Prediction of Chronic Kidney Disease Progression, MLH 2016__ 

*  Probabilistic generative model for multivariate longitudinal data that captures dependencies between multivariate trajectories. Gaussian process based regression model for each individual trajectory, and build off ideas from latent class models to induce dependence between their mean functions. 
*  _Keyword_ EHR data, GP, Random mixture model 

__* Edward Choi et al., Doctor AI: Predicting Clinical Events via Recurrent Neural Networks, MLH 2016__

* Dortor AI is a temporal model using RNN and was developed and applied to longitudinal time stampled EHR data from 260K patients over 8 years. Encounter records were input, and used for predicting the diagnosis and medicatino categories for a subsequent visit. 
*  _Keyword_ Prediction of clinical data, Deep learning, RNN

__* Yanbo Xu et al., A Bayesian Nonparametric Approach for Estimating Individualized Treatment-Response curve, MLH 2016__ 

* Estimating the continuous response over time of interventions from observationaltime series. Motivating by applications where reponse varies by individuals and therefore, estimating reponses at the individual-level are valuable for presonalized decision making. 
* _Keyword_ Bayesian nonparametric, Personalized medication 

__Truyen Tran et al., Preterm Birth Prediction: Deriving Stable and Interpretable rules from High dimensional data, MLH 2016__ 

* 1) Automatically select interpretable features, 2) Accurate classifiers. 
* L1 logistic regression / Elastic net. 

__Konstantinos Georgatzis et al., Input-Output Non-linear Dynamical systems applied to Physiological Condition Monitoring, MLH 2016__ 

* Nonlinear dynamical system for modelling the effect of drug infusion on the vital signs of patients admitted in ICUs. 
* Unscent Kalman Filter is used. Control inputs are drug infusion, and the output is a observable vital signs. Latent variables are state. 
* _Keyword_ Dynamical system. Input output. 

__Zachary C. Lipton et al., Modeling Missing Data in Clinical Time Series with RNNs, MLH 2016__

* Data: ICU, multivariate time series of observations. The measurements are irregularly spaced, leading to missingness patterns in temporally discretized sequences. 
* RNN used to fill the missing data. 

# KDD 

__Kai Fan et al., Hierarchical Graph-Coupled HMMs for Heterogeneous Personalized Health Data, KDD 2015__

* Hierarchical Graph-Coupled Hidden Markov Models (hGCHMMs) to simultaneously track the spread of infection in a small cell phone community and capture person- specific infection parameters by leveraging a link prior that incorporates additional covariates. 
* The results of our model allow us to predict the probability of infection for each persons on each day, and also to infer personal physical vulnerability and the relevant association with covariates.

__Zhengping Che et al., Deep Computational Phenotyping, KDD 2016__

* Using Physionet Challenge 2012 data, consisting of 8000 ICU units, and ICU data.
* Deep feedforward approach. 
* _Keyword_ Physionet, ICU data, Deep learning. 

__* Zitao Liu et al., Learning Adaptive Forecasting Models from Irregularly Sampled Multivariate Clinical Data, KDD 2016__

*  A challenging aspect of constructing the forecasting model is that the model should be flexible and adaptive to reflect well patient-specific temporal behaviors and this also in the case when the available patient-specific data are sparse and short span. 
*  (1) learns the population trend from a collection of time series for past patients; (2) captures individual-specific short-term multivariate variability; and (3) adapts by automatically adjusting its predictions based on new observations. 
*  _Keyword_ Linear dynamical model, Multi-task Gaussian Process 

__Jianefi Zhang et al., Survival Prediction by an Integrated Learning Criterion on Intermittently Varying Healthcare data, KDD 2016__ 

* Survival analysis on intermittently varying data by time-varying coefficients of survival model. 




# AAAI 

__* Yuan Luo et al., Predicting ICU Mortality Risk by Grouping Temporal Trends from a Multivariate Panel of Physiologic Measurements__

* Improve both accuracy and interpretability of prediction models by introducing Subgraph Augmented Non-negative Matrix Factorization (SANMF) on ICU physiologic time series. 
* SANMF converts time series into a graph representation and applies frequent subgraph mining to automatically extract temporal trends. 
* _Keyword_ ICU mortality risk prediction

__* Peter Schulam et al., Clustering Longitudinal Clinical Marker Trajectories from Electronic Health Data: Applications to Phenotyping and Endotype Discovery, AAAI__

* Individual variation makes treating diseases harder. Identifying subgroups based on clustering individual clinical severity markers getting important. Measurement sparsity and irregular sampling patterns pose additional challenges in clustering such data. 

__Marzyeh Ghassemi et al., A Multivariate Timeseries Modeling Approach to Severity of Illness Assessment and Forecasting in ICU with Sparse, Heterogeneous Clinical Data, AAAI 2015__

* Multivariate Time series modeling with the multi-task GP models using Noisy, Incomplete, Sparse, Heterogeneous and unevenly-sampled clinical data. 
* Experiment conducted to ICU. 
* MTGP to learn the correlation between and within time-series. 
* _Keyword_ GP, Multivariate time series learning. 


__Peter Schulam et al., Clustering Longitudinal Clinical Marker Trajectories from Electronic Health Data: Applications to Phenotyping and Endotype Discovery, AAAI 2016__

* Probabilistic Subtyping Model to identify subgroups based on clustering individual clinical severity markers. Measurement sparsity and irregular sampling patterns pose additional challenges in clustering such data.
* _Keyword_ Probabilistical Graphical Model / Trajectory clustering. 


__Thomas A. Lasko, Nonstationary Gaussian Process Regression for Evaluating Clinical Laboratory Test Sampling Strategies, AAAI 2015__

* Estimating the sampling strategy. 

__Kai Fan et al., A Unifying Variational Inference Framework for Hierarchical Graph-Coupled HMM with an Application to Influenza Infection, AAAI 2016__ 

* Hierarchical Graph-Coupled HMM for tracking and predicting the spread of contagious diseases, such as influenza, by leveraging social contact data collected from individual wearable devices. 
* The purpose of this paper is to build a unified learning framework for latent infection state estimation for the hGCHMM. 

# ICLR 

__Bashivan, P. et al., 2015. Learning Representations from EEG with Deep Recurrent-Convolutional Neural Networks. arXiv.org.__

* 3D time series EEG to three 2D images ('movies'), and then applied to Video classification algorithm. 
* _Keyword_ EEG, Deep learning 

__Zachary C. Lipton et al., Learning to diagnose with LSTM Recurrent Neural Networks, ICLR 2016__

* LTSM to recognize patterns in multivariate classification of diagnoses, training a model to classify. 
* _Keyword_ LTSM, Deep learning, ICU data 


# UAI 

