---
title: "SeMask: Semantically Masked Transformers for Semantic Segmentation"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Anukriti Singh
- Nikita Orlov
- Zilong Huang
- Jiachen Li
- Steven Walton
- Humphrey Shi

# # Author notes (optional)
# author_notes:
# -

date: "2021-12-12T00:00:00Z"
doi: ""

external_link: https://github.com/Picsart-AI-Research/SeMask-Segmentation

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["Workshop Paper"]

# Publication name and optional abbreviated publication name.
publication: <mark>NIVT Workshop @ICCV 2023<\mark>
publication_short: NIVT Workshop @ICCV 2023

abstract: Finetuning a pretrained backbone in the encoder part of an image transformer network has been the traditional approach for the semantic segmentation task. However, such an approach leaves out the semantic context that an image provides during the encoding stage. This paper argues that incorporating semantic information of the image into pretrained hierarchical transformer-based backbones while finetuning improves the performance considerably. To achieve this, we propose SeMask, a simple and effective framework that incorporates semantic information into the encoder with the help of a semantic attention operation. In addition, we use a lightweight semantic decoder during training to provide supervision to the intermediate semantic prior maps at every stage. Our experiments demonstrate that incorporating semantic priors enhances the performance of the established hierarchical encoders with a slight increase in the number of FLOPs. We provide empirical proof by integrating SeMask into each variant of the Swin-Transformer as our encoder paired with different decoders. Our framework achieves a new state-of-the-art of 58.22% mIoU on the ADE20K dataset and improvements of over 3% in the mIoU metric on the Cityscapes dataset. The code and checkpoints are publicly available at [this https URL](https://github.com/Picsart-AI-Research/SeMask-Segmentation).

# Summary. An optional shortened abstract.
summary:

tags: ["NIVT Workshop @ICCV 2023"]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2112.12782.pdf'
url_preprint: 'https://arxiv.org/abs/2112.12782'
url_code: 'https://github.com/Picsart-AI-Research/SeMask-Segmentation'
url_dataset: ''
url_poster: 'https://drive.google.com/file/d/1ehrtVI0Zk7y98LOmB-k9q4m_WtAS_9P7/view?usp=sharing'
url_project: ''
url_slides: 'https://drive.google.com/file/d/119sgTYiy1IbCZw6fiGseRe9pDGbOeEM9/view?usp=sharing'
url_source: ''
url_video: 'https://www.youtube.com/watch?v=eLg2rmFWiGs'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---