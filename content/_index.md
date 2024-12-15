---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "3rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/cv.pdf
    design:
      css_class: dark
      font_size: 10 rem
      background:
        color: dark
        # image:
        #   # Add your image background to `assets/media/`.
        #   filename: bg.jpg
        #   filters:
        #     brightness: 0.25
        #   size: cover
        #   position: center
        #   parallax: false
      # spacing:
      #   padding: [-20px, -20px, -20px, -20px]
  # - block: markdown
  #   content:
  #     title: ' News'
  #     subtitle: ''
  #     text: |-
  #       Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

  #       I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
        
  #       Please reach out to collaborate 😃
    # design:
    #   columns: '1'
  - block: collection
    id: publications
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
      count: 4
    design:
      # Choose a layout view
      view: article-grid
  - block: collection
    id: blogs
    content:
      title: Blogs
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blogs
      # Choose how many pages you would like to display (0 = all pages)
      count: 4
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
