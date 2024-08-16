---
title: "VCoder: Versatile Vision Encoders for Multimodal Large Language Models"
subtitle: ""
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jianwei Wang
- Humphrey Shi

# # Author notes (optional)
# author_notes:

date: "2023-12-12T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["Conference Paper"]

external_link: "https://praeclarumjj3.github.io/vcoder/"

# Publication name and optional abbreviated publication name.
publication: IEEE Conference on Computer Vision and Pattern Recognition (CVPR)
publication_short: CVPR

abstract: Humans possess the remarkable skill of Visual Perception, the ability to see and understand the seen, helping them make sense of the visual world and, in turn, reason. Multimodal Large Language Models (MLLM) have recently achieved impressive performance on vision-language tasks ranging from visual question-answering and image captioning to visual reasoning and image generation. However, when prompted to identify or count (perceive) the entities in a given image, existing MLLM systems fail. Working towards developing an accurate MLLM system for perception and reasoning, we propose using Versatile vision enCoders (VCoder) as perception eyes for Multimodal LLMs. We feed the VCoder with perception modalities such as segmentation or depth maps, improving the MLLM's perception abilities. Secondly, we leverage the images from COCO and outputs from off-the-shelf vision perception models to create our COCO Segmentation Text (COST) dataset for training and evaluating MLLMs on the object perception task. Thirdly, we introduce metrics to assess the object perception abilities in MLLMs on our COST dataset. Lastly, we provide extensive experimental evidence proving the VCoder's improved object-level perception skills over existing Multimodal LLMs, including GPT-4V.

# Summary. An optional shortened abstract.
summary: 

tags: ["CVPR 2024"]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
# - name: Colab
#   url: https://colab.research.google.com/github/SHI-Labs/OneFormer/blob/main/colab/oneformer_colab.ipynb
# - name: Demo
  # url: https://huggingface.co/spaces/shi-labs/VCoder

url_project: 'https://praeclarumjj3.github.io/vcoder/'
url_pdf: 'https://arxiv.org/pdf/2312.14233.pdf'
url_preprint: 'https://arxiv.org/abs/2312.14233'
url_code: 'https://github.com/SHI-Labs/VCoder'
url_dataset: ''
# url_poster: 'https://drive.google.com/file/d/1-U3hCYVNVht26NM-zbE87p1V4idc5bCt/view?usp=sharing'
# url_slides: 'https://drive.google.com/file/d/12XhiOXD08_LwzBwosoLVk7i8D45V8YfW/view?usp=sharing'
url_source: ''
url_video: 'https://youtu.be/go493IGgVWo'

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