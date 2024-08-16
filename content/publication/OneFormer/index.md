---
title: "OneFormer: One Transformer to Rule Universal Image Segmentation"
subtitle: ""
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Jiachen Li
- MangTik Chiu
- Ali Hassani
- Nikita Orlov
- Humphrey Shi

# # Author notes (optional)
author_notes:
-
- "Equal contribution"
- "Equal contribution"

date: "2022-11-11T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["Conference Paper"]

external_link: "https://praeclarumjj3.github.io/oneformer/"

# Publication name and optional abbreviated publication name.
publication: IEEE Conference on Computer Vision and Pattern Recognition (CVPR)
publication_short: CVPR

abstract: Universal Image Segmentation is not a new concept. Past attempts to unify image segmentation in  the last decades include scene parsing, panoptic segmentation, and, more recently, new panoptic architectures. However, such panoptic architectures do not truly unify image segmentation because they need to be trained  individually on the semantic, instance, or panoptic segmentation to achieve the best performance.  Ideally, a truly universal framework should be trained only once and achieve SOTA performance across all three image segmentation tasks. To that end, we propose OneFormer, a universal image segmentation framework that unifies segmentation with a multi-task train-once design. We first propose a task-conditioned joint training strategy that enables training on ground truths of each domain (semantic, instance, and panoptic segmentation) within a single multi-task training process. Secondly, we introduce a task token to condition our model on the task at hand, making our model task-dynamic to support multi-task training and inference. Thirdly, we propose using a query-text contrastive loss during training to establish better inter-task and inter-class distinctions. Notably, our single OneFormer model outperforms specialized Mask2Former models across all three segmentation tasks on ADE20k, CityScapes, and COCO, despite the latter being trained on each of the three tasks individually with three times the resources. With new ConvNeXt and DiNAT backbones, we observe even more performance improvement. We believe OneFormer is a significant step towards making image segmentation more universal and accessible.

# Summary. An optional shortened abstract.
summary: 

tags: ["CVPR 2023"]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
# - name: Colab
#   url: https://colab.research.google.com/github/SHI-Labs/OneFormer/blob/main/colab/oneformer_colab.ipynb
- name: Demo
  url: https://huggingface.co/spaces/shi-labs/OneFormer

url_project: 'https://praeclarumjj3.github.io/oneformer/'
url_pdf: 'https://openaccess.thecvf.com/content/CVPR2023/papers/Jain_OneFormer_One_Transformer_To_Rule_Universal_Image_Segmentation_CVPR_2023_paper.pdf'
url_preprint: 'https://arxiv.org/abs/2211.06220'
url_code: 'https://github.com/SHI-Labs/OneFormer'
url_dataset: ''
url_poster: 'https://drive.google.com/file/d/1-U3hCYVNVht26NM-zbE87p1V4idc5bCt/view?usp=sharing'
url_slides: 'https://drive.google.com/file/d/12XhiOXD08_LwzBwosoLVk7i8D45V8YfW/view?usp=sharing'
url_source: ''
url_video: 'https://youtu.be/CIU3udcaoW4'

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