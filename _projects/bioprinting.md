---
layout: page
title: Auditing Predictive Models in General Internal Medicine for Diverse and Evolving Populations
description: Supervised by Prof. Rahul Krishnan, supported by the NSERC Undergraduate Student Research Awards.
img: assets/img/gemini_logo.png
importance: 1
category: work

---
Paper coming soon!

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/healthcare.png" title="timeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


In this project, we address the pivotal issue of distribution shifts that can lead to the deterioration of model performance in the context of healthcare. These shifts, which can be attributed to changes in patient demographics, disease patterns, or healthcare practices, pose a significant challenge to the accuracy and reliability of models used in clinical decision-making. Our focus is twofold: (i) understanding the impact of various distribution shifts on model performance in the constantly evolving landscape of healthcare data, and (ii) demonstrating the capability of existing methodologies to evaluate model performance using solely unlabeled data. This is particularly beneficial in environments where labeled data is scarce or unavailable.

The study is conducted using the GEMINI database, which contains administrative and clinical data from over 30 Canadian hospitals, encompassing more than 640,000 unique patients and 2.2 billion data points. To assess the impact of distribution shifts, we developed statistical models using the XGBoost algorithm to predict four different mortality risk and length of stay tasks. The distribution shifts we studied include temporal, institutional (hospital-to-hospital), and demographic shifts. Our approach has led to the establishment of a systematic framework for the ongoing monitoring and auditing of model performance in hospital settings. This framework is designed to ensure that the models deployed are safe, ethically responsible, and continuously adapt to changes in patient populations and clinical environments.






