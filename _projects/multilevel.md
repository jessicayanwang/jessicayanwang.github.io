---
layout: page
title: "Runoff Efficiency in a Changing Climate: A Multilevel Approach"
description: "A multilevel model exploring the relationships between climatic indices and runoff efficiency across watersheds and clusters."
img: assets/img/runoff_efficiency.png
importance: 4
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/research_questions.png" title="Research Questions" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Project Overview
This project explores the dynamics of **runoff efficiency**—the ratio of streamflow to precipitation—across 3,022 watersheds worldwide. By developing a three-level multilevel model, we analyze the effects of climatic covariates such as **Aridity Index (AI)**, **Seasonality Index (SI)**, and **Snow Fraction (SF)** on runoff efficiency.

Our findings underscore the complex interplay between **climate, hydrology, and geography**, highlighting the role of snow-dominated systems in sustaining water resources amid climatic variability.

---

### Methodology

1. **Data Sources**:
   - Streamflow and precipitation data from global gauge records.
   - Climatic indices derived from global datasets.
   - BIOME-based clustering to group watersheds by climate and physical characteristics.

2. **Three-Level Hierarchical Model**:
   - **Level 1**: Year-to-year variability within watersheds, driven by temporal climate fluctuations.
   - **Level 2**: Variability between watersheds, influenced by geographic and hydrological factors.
   - **Level 3**: Regional differences across BIOME-based clusters, reflecting ecological and climatic characteristics.

3. **Model Specification**:
   - Fixed effects for climatic averages and deviations.
   - Random effects to capture unobserved variability at watershed and cluster levels.
   
  <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/multilevel-model.png" title="model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

### Key Findings

1. **Climatic Covariates**:
   - Higher **aridity** and **seasonality** indices reduce runoff efficiency.
   - Higher **snow fraction** enhances runoff efficiency, reflecting its role in delayed water release.

2. **Variability**:
   - **Watersheds**: 50% of runoff efficiency variability attributed to watershed-level differences.
   - **Clusters**: 36% variability attributed to regional cluster characteristics.

3. **Impact of Yearly Deviations**:
   - Short-term increases in aridity reduce efficiency, while above-average snowfall years improve efficiency.

---

### Results

#### Fixed Effects Summary
| Term         | Estimate | Std. Error | p-value   |
|--------------|----------|------------|-----------|
| (Intercept)  | 0.498    | 0.026      | <0.001    |
| Mean AI      | -0.149   | 0.005      | <0.001    |
| Mean SF      | 0.241    | 0.022      | <0.001    |

 <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fixed-effect.png" title="fixed-effect" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

#### Random Effects Summary
- Variability across watersheds and clusters highlights the influence of **regional characteristics**.

 <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/random-effect.png" title="random-effect" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

### Contributions
- Developed a comprehensive multilevel model to analyze runoff efficiency across temporal and spatial scales.
- Provided actionable insights for **water resource management** in the context of climate change.

---

### Limitations & Future Work
- **Linear Assumptions**: Nonlinear or machine learning models could capture more complex relationships.
- **Additional Covariates**: Land use, soil type, and anthropogenic factors could further refine the analysis.

---

### Acknowledgments
This project is a collaborative effort by **Jessica Wang**, **Qianyi Wang**, and **Even Li**.

---

### References
- [Project Report](https://github.com/jessicayanwang/Multilevel-Approach-to-Runoff-Efficiency/blob/main/Report.pdf)
