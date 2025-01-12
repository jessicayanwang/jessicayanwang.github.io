---
layout: page
title: Beyond Gender: Addressing Age and Disability Biases with Context-Debias
description: A project extending Context-Debias to mitigate biases related to age and disability in pre-trained language models.
img: assets/img/debiasing-logo.png
importance: 1
category: work

---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/nlp-debiasing.png" title="timeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Project Overview
Language models encode social biases present in their training data, which can lead to unfair outcomes in NLP applications. While existing methods address gender and racial biases, this project extends **Context-Debias** to mitigate biases related to **age** and **disability**.

Our approach combines **orthogonal projection techniques** with contextualized word embeddings (e.g., BERT) to address stereotypes while preserving downstream task performance.

---

### Methodology
- **Debiasing Loss:** Mitigates biased associations by minimizing the inner product between contextualized and non-contextualized embeddings of target and attribute words.
- **Regularization Loss:** Preserves semantic integrity by minimizing the distance between original and debiased embeddings.
- **Evaluation:** Uses SEAT (Sentence Encoder Association Test) for bias reduction and GLEU benchmarks for downstream performance.

![Method Overview](/assets/images/projects/debiasing-method.png)

---

### Results
1. **Bias Reduction:** Reduced effect sizes in SEAT tests for age and disability-related biases.
2. **Downstream Task Performance:** Maintained GLEU scores comparable to original embeddings across tasks like sentiment analysis, paraphrase detection, and textual entailment.

---

### Key Contributions
- Expanded bias mitigation methods to underexplored dimensions (age, disability).
- Achieved significant bias reduction while preserving downstream utility.
- Provided insights into cross-dimensional interactions in bias mitigation.

---

### Impact Statement
By addressing age and disability biases, this project contributes to the development of more equitable NLP systems. Our findings are critical for ensuring fairness in applications like hiring algorithms, healthcare systems, and chatbots.

---

### References
For more details, check out our [GitHub repository](https://github.com/Evenlii/auto-debias-reproduction).







