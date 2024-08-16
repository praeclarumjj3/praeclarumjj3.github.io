---
title: "OLIE"
subtiltle: 
summary: "Object Level Image Editing using Instance Segmentation Maps"
tags:
- other
date: "2021-04-10T00:00:00Z"

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
url_code: "https://github.com/praeclarumjj3/OLIE"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
---

OLIE was aimed to reconstruct the original image with the objects removed (editing) by incorporating the mask features as input to the reconstructor.

After performing many experiments, we scrapped the idea. However, some of the experiments that I performed were:

- **Using a Perturbator Model:** Taking inspiration from [GanPaint](https://ganpaint.io/), I tried editing images using perturbations in the reconstructor, however it didn't work well.

- **Using Gated Convolutions:** Taking inspiration from [Free-Form Image Inpainting with Gated Convolution](https://paperswithcode.com/paper/free-form-image-inpainting-with-gated), I used `Gated Modules` instead of standard modules which gave even **poorer results**.

- **Using Two Stage Model:** Getting hole images from the reconstructor and then passing that into an inpainting model gave somewhat good results as the generating the hole image could be learned accurately to an extent, however, the results were no better than the common inpainting ones.

Our aim was to come up with a **Single Stage Model** for image editing using instance maps.

For more info, please see the Code on `GitHub`.
