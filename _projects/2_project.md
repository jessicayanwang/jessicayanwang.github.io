---
layout: page
title: Developing a 3D deep learning pipeline for segmenting neuronal somas in whole-brain light sheet fluorescence microscopy rodent data
description: Funded by 2023 T-CAIREM AI in Medicine Summer Research Studentship Program 
img: assets/img/neurons.png
importance: 1
category: work
---

Mapping neuronal cell bodies is important to study how the brain functions, understand the machanims underlying neurodiseases, and also develop targeted interventions for neurodegenerative diseases. Mouse, often used as an important model organism, have 8–14 million of neurons that are in the scale of micrometres, how can people study them?

Thanks to recent advances in tissue clearing technology and light sheet fluorescence microscopy (LSFM) imaging techniques, we can obtain a transparent whole brain image of neuronal cell bodies in mice. Below is an example of the data that I have worked with.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/raw.gif" title="Raw Image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    2D slice image patch of a whole brain 3D light-sheet fluorescence microscopy image after tissue clearing on a healthy mouse. C-Fos immunostaining was used as a marker for neuronal cell bodies.
</div>

As current computational pipelines for identifying the neurons are either 2D-based, or have problems such as low speed, lack of generalizability, and requirement of lots of human intervention.
In this project, I have been working on developing an automatic 3D deep learning-based computational pipeline to segment neuron cell bodies in whole-brain LSFM image data.

The model I am working on is based on U-Net with some modifications that we specifically designed for dealing with 3D LSTM image data. Here are some preliminary results. Below I overlay the model prediction (in blue) and the ground-truth (in red). Note that the branches, colored in red are actually axons not neuron somas, which are mislabeled in groundtruth, whereas our model successfully avoids them. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Preliminary results. Visualized using Napari.
</div>

<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %} -->
