---
layout: page
title: Education Platform Student Answer Prediction
description: Predicting student responses using Item Response Theory and machine learning models.
img: assets/img/Student_Answer_Prediction.png
importance: 6
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Student_Answer_Prediction.png" title="Student Answer Prediction" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Check out the full report [here](https://drive.google.com/file/d/1d3ENOa27pM0PCc8TQ3z8M05peTuDTzpx/view?usp=sharing).

This project involved predicting student answers on an educational platform by implementing a learning-based **Item Response Theory (IRT) Model**. The goal was to model student ability against question difficulty to formulate a probability distribution for correct responses.

### Key Achievements:
- **Item Response Theory Model**: Developed a 1-parameter and 3-parameter IRT model to predict student success rates based on question difficulty and student ability.
- **Model Optimization**: Experimented with **Autoencoders**, **Matrix Factorization**, **Neural Networks**, and **Ensemble methods** to enhance prediction accuracy.
- **Data Processing \& Accuracy**: Achieved a final validation accuracy of 71.1\% and test accuracy of 70.3\% using the IRT model, improving accuracy by adding guessing and discrimination parameters.