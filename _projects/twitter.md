---
layout: page
title: Twitter Sentiment Analysis Under COVID-19
description: Analyzing political sentiment and tweet popularity during the pandemic.
img: assets/img/Twitter_Analysis.png
importance: 4
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Twitter_Analysis.png" title="Twitter Sentiment Analysis" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Check out the full report [here](https://drive.google.com/file/d/13YD3Vb4k0vSMUJ0LCmSpLQ4Vg15xQCUG/view?usp=sharing).

This project analyzes the popularity of political tweets during the COVID-19 pandemic. Using 10,000 political tweets extracted with Twitter’s API, we built a Naive Bayes classifier to predict tweet popularity, incorporating retweets, favorites, and follower counts.

### Key Achievements:
- **Naive Bayes Classifier**: Classified tweets into "Not Popular", "Popular", and "Very Popular" categories, achieving a **48% improvement** in precision for predicting "Very Popular" tweets compared to the baseline.
- **Popularity Score**: Engineered a custom metric combining retweets and favorites normalized by follower count to better capture tweet popularity trends.
- **Exploratory Data Analysis (EDA)**: Performed detailed analysis of skewed engagement metrics, handling over 1,500 outliers and visualizing insights using log transformations and correlation analysis.