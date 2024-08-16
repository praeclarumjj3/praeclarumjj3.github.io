---
title: "AOT-GAN Experiments"
subtiltle: 
summary: "Experiments conducted with AOT-GAN"
tags:
- Deep Learning
date: "2021-05-19T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: ""
  focal_point: ""

#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: "https://github.com/praeclarumjj3/AOT-GAN-Experiments"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
---

I conducted various experiments with **AOT-GAN** proposed in the paper: [Aggregated Contextual Transformations for High-Resolution Image Inpainting](https://arxiv.org/abs/2104.01431)) on the [Places2](http://places2.csail.mit.edu/download.html) dataset using the [PConv Free Form Masks for Inpainting](https://nv-adlr.github.io/publication/partialconv-inpainting).

In particular, I focused on finding the effectivity of different losses while training the framework. I made several observations:

- The **adversarial loss** doesn't seem to be contributing to the learning of the model as it stays almost the same throughout the training.

- Training for longer than `1e4` iterations doesn't add much improvement to the results.

- Training **without style loss** produces blurry results. Therefore, style loss is an important component for texture related synthesis of images.

- Training **without adversarial loss** also produces good quality results!

For more info, please see the Code on `GitHub`.