![Python](https://img.shields.io/badge/python-v3.7-blue)
![Tensor](https://img.shields.io/badge/TensorFlow-V2.9.1-orange)
![Keras](https://img.shields.io/badge/Keras-V2.7-brightgreen)
![pandas](https://img.shields.io/badge/Pandas-V1.4.2-ff69b4)
![numpy](https://img.shields.io/badge/%E2%80%8ENumpy-V1.20.2-success)
![releasedate](https://img.shields.io/badge/release%20date-June%222023-red)
![Opensource](https://img.shields.io/badge/OpenSource-Yes!-6f42c1)

# Hybrid machine learning models

# [Predicting traffic crash severity using hybrid of balanced bagging classification and light gradient boosting machine](https://www.researchgate.net/profile/Jovial-Niyogisubizo/publication/367664188_Predicting_traffic_crash_severity_using_hybrid_of_balanced_bagging_classification_and_light_gradient_boosting_machine/links/63ddc049c97bd76a8263dc78/Predicting-traffic-crash-severity-using-hybrid-of-balanced-bagging-classification-and-light-gradient-boosting-machine.pdf)


This is the official repository of **Predicting traffic crash severity using hybrid of balanced bagging classification and light gradient boosting machine** 


**Hybrid machine learning models for traffic crash severity prediction** <br />



**For details, please refer to:**

**[[Paper](https://www.researchgate.net/profile/Jovial-Niyogisubizo/publication/367664188_Predicting_traffic_crash_severity_using_hybrid_of_balanced_bagging_classification_and_light_gradient_boosting_machine/links/63ddc049c97bd76a8263dc78/Predicting-traffic-crash-severity-using-hybrid-of-balanced-bagging-classification-and-light-gradient-boosting-machine.pdf)]** 



## Abstract

Accident severity prediction is a hot topic of research aimed at ensuring road safety as well as taking precautionary measures for anticipated future road crashes. In the past decades, both classical statistical methods and machine learning algorithms have been used to predict traffic crash severity. However, most of these models suffer from several drawbacks including low accuracy, and lack of interpretability for people. To address these issues, this paper proposed a hybrid of Balanced Bagging Classification (BBC) and Light Gradient Boosting Machine (LGBM) to improve the accuracy of crash severity prediction and eliminate the issues of bias and variance. To the best of the author’s knowledge, this is one of the pioneer studies which explores the application of BBC-LGBM to predict traffic crash severity. On the accident dataset of Great Britain (UK) from 2013 to 2019, the proposed model has demonstrated better performance when compared with other models such as Gaussian Naïve Bayes (GNB), Support vector machines (SVM), and Random Forest (RF). More specifically, the proposed model managed to achieve better performance among all metrics for the testing dataset (accuracy = 77.7%, precision = 75%, recall = 73%, F1-Score = 68%). Moreover, permutation importance is used to interpret the results and analyze the importance of each factor influencing crash severity. The accuracy-enhanced model is significant to several stakeholders including drivers for early alarm and government departments, insurance companies, and even hospitals for the services concerned about human lives and property damage in road crashes.

## Methodology


We proposed the ensemble-based hybrid BBC-LGBM which is often much more accurate than a single method due to its ability to handle bias, variance, and error reduction to enhance accuracy and help to achieve better approximation.

<br/>

![](/figures/method.png)

<br/>


## Correlation matrix dependence heat map


Before proceeding to model development and avoiding the issues of multicollinearity, we first check the multicollinearity between variables using Spearman’s correlation matrix. The Spearman correlation coefficient between many features and accident severity is at a high level [0.6, 1]. Since the correlation coefficient only states the linear relationships which would also make explaining feature importance very tricky due to the scarce independence of features, the R^2 prediction error was taken into consideration while computing Spearman’s correlation to make sure it is simple to predict any variable.

<br/>

![](/figures/heat_map.png)

<br/>

## Permutation importance

Permutation importance plays a significant role in removing an impurity-based feature that would lead to high importance even when the feature has no predictive ability on the experimental variable. Permutation importance has a strong ability to evaluate the impact of discriminatory information on every feature production.

<br/>

![](/figures/Permutation_importance.png)

<br/>

## Dataset

**The Data-Set is Available in below links:**

[To download Dataset you can use this link:] [Click Here](https://www.data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data). Unzip the data sets into the folder *data*.	


## Getting Started

**To run the script please use this file on Google Colab or Jupyter Notebook:**


```notebooks``` folder contains all scripts used to train and test models. More details on how to train and test the code is mentioned inside ```notebooks``` folder.

<br/>

## Evaluation and metrics

**We use the following evaluation Metrics for experimental results:**

 Accuracy,Precision, Recall,F1-Score


**Created by:** : Jovial Niyogisubizo 

jovialniyo93@gmail.com


**Citation Request:** 

If you find our work useful in your research, please consider citing:

Jovial, N.; Lyuchao L.; Fumin Z.; Guangjie H.; Eric N.; Ben L.; Yuyuan L. Predicting traffic crash severity using hybrid of balanced bagging classification and light gradient boosting machine. Intell. Data Anal. 2023, 27(1), 79-101. https://doi.org/10.3233/IDA-216398.


>[Online Published Paper](https://www.researchgate.net/profile/Jovial-Niyogisubizo/publication/367664188_Predicting_traffic_crash_severity_using_hybrid_of_balanced_bagging_classification_and_light_gradient_boosting_machine/links/63ddc049c97bd76a8263dc78/Predicting-traffic-crash-severity-using-hybrid-of-balanced-bagging-classification-and-light-gradient-boosting-machine.pdf)




## License ##
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.



  
