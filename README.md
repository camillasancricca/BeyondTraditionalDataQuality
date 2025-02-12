# Exploring the Influence of Data Characteristics on Machine Learning Outcomes

This repository contains the experiments conducted to develop and validate a quality model to be used in data-centric AI applications.
Such a model includes all the possible data characteristics that may undermine the execution of a machine-learning pipeline and their related metrics.

<p align="center">
<img src="/static/model.png" width="400" alt="Description">
</p>

**Profile-related** data characteristics describe the profiling characteristics that can be automatically extracted from a dataset through data profiling operations:

- *Dimensionality* refers to the size (i.e., the number of features and instances) of a dataset
- *Data Types* represent the count of numerical, categorical, or boolean variables in a dataset
- *Dependency* is related to the presence of redundant or highly correlated features within a dataset
- *Imbalance* is the deviation of the values distribution of a feature from an ideal Gaussian fit
- *Class Purity* quantifies the presence of label errors or inconsistencies within the targeted class
- *Class Balance* assesses the degree to which the values of the targeted class are equally distributed
- *Class Overlap* measures the similarity of data points with different labels

**Bias-related** data characteristics aim to detect and measure the presence of bias in the training data:

- *Coverage* represents the degree to which a dataset is representative of the real world
- *Disparity* aims to assess whether there is a disparity in the label distribution among different demographic groups
- *Density* is a measure of how densely concentrated certain values are within a feature
- *Diversity* is a measure of the value heterogeneity within a feature

---

## Folders

This repository contains:

1. **Assessment metrics** for computed the proposed data characteristics on the selected datasets.
- Folder: 0_ASSESSMENT
  - *dataset* folder: it contains the datasets for computing the metrics
  - *plot* folder: it contains visualizations of the computed metrics
  - *all.ipynb*: notebook for computing some of the proposed metrics on the example datasets

2. **Experiments** including the code used for implementing a study on the impact of the identified data characteristics on machine learning performance and fairness.
- Folder: 1_IMPACT
  - *dataset* folder: it contains the datasets used for the experiments
  - *plot* folder: it contains visualizations of the computed experiments
  - *metric-name.ipynb*: notebook for executing and analyzing the experiments for a specific data characteristic

3. **Datasets information** contains tables with additional details on the datasets used for the experiments
- Folder: 2_DATASETS
