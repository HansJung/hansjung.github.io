---
layout: post
title: Plan of study - Machine learning and Healthcare
---

Last updated: 16/10/19


## Healthcare related papers (Quick and Dirty review) 

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


__Zachary C. Lipton et al., Learning to diagnose with LSTM Recurrent Neural Networks, ICLR 2016__

* LTSM to recognize patterns in multivariate classification of diagnoses, training a model to classify. 
* _Keyword_ LTSM, Deep learning, ICU data 



## Problems I am interested 

### 1. Personalized medicine by analyzing disease trajectory for better prediciton based on EHR data. 

Personalized medicine is a medical procedure that separates patients into different groups—with medical decisions, practices, interventions and/or products being tailored to the individual patient based on their predicted response or risk of disease. [1](https://en.wikipedia.org/wiki/Personalized_medicine)

More specifically, multiple genes collectively influence the likelihood of developing many common and complex diseases. Personalized medicine can also be used to predict a person's risk for a particular disease. 

With EHR data that is including patients' information and biomarkers (physiological signals), 



## Possible open problem 

1. Classification / Clustering of ECG signal / beat taking account of individuals' information. 
2. Low dimensional projection of multiple longitudinal data corresponding to a specific patient. 
3. Deep learning based anomaly detection scheme in EHR. 
4. Modeling multiple biomarkers in composite GP / GP with kernel learning method. 
5. Poisson matrix factorization in recommendation system. 
6. Readmission rate prediction using Hawkess process 
7. Recurrent GP modeling for ECG. 
 


## Available dataset 

### Breast Cancer Proteomes 

* This data set contains published iTRAQ proteome profiling of 77 breast cancer samples generated by the Clinical Proteomic Tumor Analysis Consortium (NCI/NIH). It contains expression values for ~12.000 proteins for each sample, with missing values present when a given protein could not be quantified in a given sample.
* [https://www.kaggle.com/piotrgrabo/breastcancerproteomes](https://www.kaggle.com/piotrgrabo/breastcancerproteomes)

### Zika Virus Epidemic 

* This dataset shares publicly available data related to the ongoing Zika epidemic. It is being provided as a resource to the scientific community engaged in the public health response. The data provided here is not official and should be considered provisional and non-exhaustive. The data in reports may change over time, reflecting delays in reporting or changes in classifications. And while accurate representation of the reported data is the objective in the machine readable files shared here, that accuracy is not guaranteed. Before using any of these data, it is advisable to review the original reports and sources, which are provided whenever possible along with further information on the CDC Zika epidemic GitHub repo.
* [https://www.kaggle.com/cdc/zika-virus-epidemic](https://www.kaggle.com/cdc/zika-virus-epidemic)


### Hospital Charges for Inpatients

* Variation of hospital charges in the various hospitals in the US for the top 100 diagnoses. The dataset is owned by the US government. This dataset will show you how price for the same diagnosis and the same treatment and in the same city can vary differently across different providers. It might help you or your loved one find a better hospital for your treatment. You can also analyze to detect fraud among providers.
* [https://www.kaggle.com/speedoheck/inpatient-hospital-charges](https://www.kaggle.com/speedoheck/inpatient-hospital-charges)


### Breast cancer dataset 

* Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image. Separating plane described above was obtained using Multisurface Method-Tree (MSM-T) [K. P. Bennett, "Decision Tree Construction Via Linear Programming." Proceedings of the 4th Midwest Artificial Intelligence and Cognitive Science Society, pp. 97-101, 1992], a classification method which uses linear programming to construct a decision tree. Relevant features were selected using an exhaustive search in the space of 1-4 features and 1-3 separating planes. 

* [https://www.kaggle.com/uciml/breast-cancer-wisconsin-data](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data)

### Prescription based prediction 

* The prescription vector for each doctor tells a rich story about that doctor's attributes, including specialty, gender, age, and region. There are 239,930 doctors in the dataset.
* [https://www.kaggle.com/roamresearch/prescriptionbasedprediction](https://www.kaggle.com/roamresearch/prescriptionbasedprediction)
* http://roamanalytics.com/2016/09/13/prescription-based-prediction/

### MIMIC II 

* Physiologic signals and vital signs time series captured from patient monitors, and comprehensive clinical data obtained from hospital medical information systems, for tens of thousands of Intensive Care Unit (ICU) patients*. 


## Theories 

### Deep learning model in analyzing time series data 

* Recurrent Neural Network 
* Restricted Boltzman Machine 


### Gaussian process regression 

### Other process and models 

* Probabilistic graphical model for Bayesian nonparametrics analysis
* Stochastic process 
    * Mondrian process 
    * Hawkess process 



## Community 

### Conference: Theory 

* ICML 
* NIPS
* AISTAT

### Conference: Application 

* UAI 
* KDD
* AAAI
* IJCAI
* Machine learning and healthcare

### Conference: Bioinformatics

* CinC 
* ACM-BCB
* AMIA 
