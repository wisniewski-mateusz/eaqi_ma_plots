---
layout: single
title: ""
permalink: /
toc: True
toc_label: "Table of contents"
toc_icon: "fas fa-list-ul"
toc_sticky: true
---

<span style="font-size:xx-large;">**Forecasting pollutants concentration and air quality index in Poland with gradient boosted models**</span>

This site is a visualization complement to the *Forecasting pollutants concentration and air quality index in Poland with gradient boosted models* master thesis. Additional figures can be found here. All of them have the *own study* source.

## 5.2 Comparison with the CAMS model

### Dimensionality reduction using SHAP for model with NO2 target

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/02_dim_red_NO2_1.png" alt="alt_text" width="1000"/>
</p>

---

### Dimensionality reduction using SHAP for model with O3 target

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/02_dim_red_O3_1.png" alt="alt_text" width="1000"/>
</p>

---

### Comparison between naive approach and the CAMS model

In the figure's legends next to the model name, RMSEs are added.

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/05_naive_vs_cams.png" alt="alt_text" width="1000"/>
</p>

---
---

## 5.3 Regression models

### 5.3.1 Training

#### Comparison between regression models and the naive approach by all quarters

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/05_naive_vs_model.png" alt="alt_text" width="1000"/>
</p>

---

### 5.3.2 Interpretation

#### SHAP dependence plots between quarter and g_{pollutant}_avg features

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/04_shap_dep_pollutants_quarter.png" alt="alt_text" width="1000"/>
</p>

---

#### Force plot for the MzWarKondrat station on 27.02.2019

[Force plot for the MzWarKondrat station on 27.02.2019]({{ site.url }}{{ site.baseurl }}/04_force_plots_MzWarKondrat_pollutants)

---

#### Force plot for the MzWarWokalna station on 18.11.2018

[Force plot for the MzWarWokalna station on 18.11.2018]({{ site.url }}{{ site.baseurl }}/04_force_plots_MzWarWokalna_pollutants)

---
---

## 5.4 Classification model

### 5.4.1 Training

#### Optuna hyperparamter importances for base model

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/03_optuna_study_gbm_sdm.png" alt="alt_text" width="1000"/>
</p>

---

#### Optuna hyperparamter importances for customized model

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/03_optuna_study_gbm_sdm_c.png" alt="alt_text" width="1000"/>
</p>

---

### 5.4.2 Interpretation

#### SHAP aggregated summary plot for the classification model

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/03_shap_ex_20.png" alt="alt_text" width="1000"/>
</p>

---

#### SHAP summary plots per category

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/03_shap_ex_i.png" alt="alt_text" width="1000"/>
</p>

---

#### SHAP dependence plots between eaqi_0 and g_PM10_avg features

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/03_shap_dep_g_PM10_avg_eaqi_0.png" alt="alt_text" width="1000"/>
</p>

---

#### SHAP dependence plots between n_gust_sfc_1_avg and month features

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/03_shap_dep_month_n_gust_sfc_1_avg.png" alt="alt_text" width="1000"/>
</p>

---

#### SHAP dependence plots between eaqi_0 and n_apcp_sfc_1_max features

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/03_shap_dep_n_apcp_sfc_1_max_eaqi_0.png" alt="alt_text" width="1000"/>
</p>

---

#### Force plot for the MzWarAlNiepo station on 01.06.2019

[Force plot for the MzWarAlNiepo station on 01.06.2019]({{ site.url }}{{ site.baseurl }}/03_force_plots_MzWarAlNiepo)

---

#### Force plot for the MpZakopaSien station on 01.06.2019

[Force plot for the MpZakopaSien station on 01.06.2019]({{ site.url }}{{ site.baseurl }}/03_force_plots_MpZakopaSien)

---
---

## 5.5 Final model

### 5.5.1 The choice

#### Confusion matrices from the regression, classification and ensemble model from the validation set

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/04_cm_comparison_r_c.png" alt="alt_text" width="1000"/>
</p>

---

#### Comparison between all versions of classification models and the naive approach by all quarters

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/05_eaqi_performances.png" alt="alt_text" width="1000"/>
</p>

---

### 5.5.2 Performance evaluation

#### Evaluation of the ensemble model by monitoring station&ndash;interactive

[Evaluation of the ensemble model by monitoring station&ndash;interactive]({{ site.url }}{{ site.baseurl }}/5_14_evaluation_interactive)