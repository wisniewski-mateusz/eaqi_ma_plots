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

## 5.3.1 Regression models&ndash;interpretation

### SHAP dependence plots between quarter and g_{pollutant}_avg features

<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/04_shap_dep_pollutants_quarter.png" alt="alt_text" width="1000"/>
</p>

---

### Force plot 1

[Force Plot 1]({{ site.url }}{{ site.baseurl }}/03_force_plots_MpZakopaSien.html)

---

### Force plot 2


---
---

## 5.4.1 Classification model&ndash;interpretation

---
---

## 5.5 Final model&ndash;performance evaluation

### Evaluation of the ensemble model by monitoring station&ndash;interactive

[Evaluation of the ensemble model by monitoring station&ndash;interactive]({{ site.url }}{{ site.baseurl }}/5_14_evaluation_interactive)