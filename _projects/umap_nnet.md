---
layout: page
title: UMAP Network Connections
description: 
img: assets/img/umap1.webp
importance: 3
---
These graphs show the connections between different images as understood by a deep learning neural network - a Variational Autoencoder (VAE). The dataset consists of 60,000 low-resolution images of fashion items (shoes, shirts, bags, etc.). Each tiny dot in the graph corresponds to an image and the edges represent similarity relationships between those images. Images that are close together in the graph are similar to one another as understood by the neural network.

To generate this picture, I train the convolutional autoencoder on the [fashion-MNIST dataset](https://github.com/zalandoresearch/fashion-mnist), use the trained network to extract 256-dimensional representations of each image in the dataset, then use [Uniform Manifold Approximation and Projection (UMAP)](https://arxiv.org/abs/1802.03426) to compress those representations down into 2 dimensions. UMAP internally maps the data points onto a graph, the edges of which are represented in this image. To generate the visual, I used a slightly modified version of the plot connectivity utility in the [umap-learn python library](https://umap-learn.readthedocs.io/en/latest/). Code is available [on github](https://github.com/dhudsmith/nnet_umap).

See more at [this reddit post](https://www.reddit.com/r/dataisbeautiful/comments/m5z0db/connections_between_60000_images_as_understood_by/). 

<div class="row">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.html path="assets/img/umap1.webp" title="Umap Nnet 1" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.html path="assets/img/umap2.webp" title="Umap Nnet 2" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.html path="assets/img/umap3.webp" title="Umap Nnet 3" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.html path="assets/img/umap4.webp" title="Umap Nnet 4" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


