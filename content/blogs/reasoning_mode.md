---
title: Why do we still have reasoning modes?
subtitle: 

# Summary for listings and search engines
summary: ''

# Date published
date: "2026-08-02T00:00:00Z"

# Date updated
lastmod: "2026-08-02T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ''
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- Research

categories:
- Experience
---

We find ourselves living in an age where we get a new frontier model almost every few months, if not weeks. Whenever a new generation of model comes out from the closed-source or open-source giants, we instinctively switch to the most “advanced” model whenever possible so we can make sure we have access to the best worker (or so claimed) available for our goal. After choosing a model, we as users are faced with another choice which I feel is not studied as much: what reasoning effort to choose?

Now, if this were a paper, I would go on to motivate why we need to scientifically study the effect of reasoning mode on a per-sample basis across about 30 benchmarks and how there would have been some interesting observations. However, I am going to question the whole reasoning mode choice premise here. Why?

Because I believe this whole setting where we expect the user to select reasoning mode/effort is very much anti-user-friendly. Moreover, the reasoning effort selection seemed a good way to train models for test-time scaling for varying task difficulties back in 2025, something that the frontier labs have done tremendously well at scale, leading to impressive performance on long-horizon tasks and the rise of the RSI (recursive self-improvement) field.

> Note that the current models already have some form of adaptive reasoning ability under the hood for each reasoning mode where they do not spend a lot of tokens on easier tasks with a focus on controlling the cost for executing a task. I am all for giving the user more control over how much work the model should do (or money should it spend) but this control may be bad when the user has no clue how the model was trained.

Therefore, I believe it’s time we move away from configuring the effort in reasoning modes and let the model handle it online adaptively at every turn. What would that look like? I feel there are numerous ways for us to get there.

Read more at: https://praeclarumjj3.substack.com/p/why-do-we-still-have-reasoning-modes