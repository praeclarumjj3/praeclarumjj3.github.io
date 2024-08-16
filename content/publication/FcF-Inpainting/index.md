---
title: "Keys to Better Image Inpainting: Structure and Texture Go Hand in Hand"
subtitle: ""
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Yuqian Zhou
- Ning Yu
- Humphrey Shi

# # Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2022-08-11T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["Conference Paper"]

external_link: "https://praeclarumjj3.github.io/fcf-inpainting/"

# Publication name and optional abbreviated publication name.
publication: IEEE/CVF Winter Conference on Applications of Computer Vision 2023
publication_short: WACV 2023

abstract: Deep image inpainting has made impressive progress with recent advances in image generation and processing algorithms. We claim that the performance of inpainting algorithms can be better judged by the generated structures and textures. Structures refer to the generated object boundary or novel geometric structures within the hole, while texture refers to high-frequency details, especially man-made repeating patterns filled inside the structural regions. We believe that better structures are usually obtained from a coarse-to-fine GAN-based generator network while repeating patterns nowadays can be better modeled using state-of-the-art high-frequency fast fourier convolutional layers. In this paper, we propose a novel inpainting network combining the advantages of the two designs. Therefore, our model achieves a remarkable visual quality to match state-of-the-art performance in both structure generation and repeating texture synthesis using a single network. Extensive experiments demonstrate the effectiveness of the method, and our conclusions further highlight the two critical factors of image inpainting quality, structures, and textures, as the future design directions of inpainting networks.

# Summary. An optional shortened abstract.
summary:

tags: ["WACV 2023"]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Colab
  url: https://colab.research.google.com/github/SHI-Labs/FcF-Inpainting/blob/main/colab/FcF_Inpainting.ipynb
url_project: 'https://praeclarumjj3.github.io/fcf-inpainting/'
url_pdf: 'https://openaccess.thecvf.com/content/WACV2023/papers/Jain_Keys_To_Better_Image_Inpainting_Structure_and_Texture_Go_Hand_WACV_2023_paper.pdf'
url_preprint: 'https://arxiv.org/abs/2208.03382'
url_code: 'https://github.com/SHI-Labs/FcF-Inpainting'
url_dataset: ''
url_poster: 'https://drive.google.com/file/d/1fwJr01QtwWt9tOFz24INPAFk5ZhRMazs/view?usp=sharing'
url_slides: 'https://drive.google.com/file/d/1p9Q-mOfyAFqOEr6-ZE-KdtzlOFoHb99E/view?usp=sharing'
url_source: ''
url_video: 'https://youtu.be/-V1p2vU62VA'

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