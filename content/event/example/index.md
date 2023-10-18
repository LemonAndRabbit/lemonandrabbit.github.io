---
title: "2023HPCA ViTALiTy"

event: HPCA 2023
event_url: https://hpca-conf.org/2023/

location: Montreal, QC, Canada

summary: "ViTALiTy: Unifying Low-rank and Sparse Approximation for Vision Transformer Acceleration with a Linear Taylor Attention"
abstract: "Vision Transformer (ViT) has emerged as a competitive alternative to convolutional neural networks for various computer vision applications. Specifically, ViT multi-head attention layers make it possible to embed information globally across the overall image. Nevertheless, computing and storing such attention matrices incurs a quadratic cost dependency on the number of patches, limiting its achievable efficiency and scalability and prohibiting more extensive real-world ViT applications on resource-constrained devices. Sparse attention has been shown to be a promising direction for improving hardware acceleration efficiency for NLP models. However, a systematic counterpart approach is still missing for accelerating ViT models. To close the above gap, we propose a first-of-its-kind algorithm-hardware codesigned framework, dubbed ViTALiTy, for boosting the inference efficiency of ViTs. Unlike sparsity-based Transformer accelerators for NLP, ViTALiTy unifies both low-rank and sparse components of the attention in ViTs. At the algorithm level, we approximate the dot-product softmax operation via first-order Taylor attention with row-mean centering as the low-rank component to linearize the cost of attention blocks and further boost the accuracy by incorporating a sparsity-based regularization. At the hardware level, we develop a dedicated accelerator to better leverage the resulting workload and pipeline from ViTALiTy's linear Taylor attention which requires the execution of only the low-rank component, to further boost the hardware efficiency. Extensive experiments and ablation studies validate that ViTALiTy offers boosted end-to-end efficiency (e.g., 3× faster and 3× energy-efficient) under comparable accuracy, with respect to the state-of-the-art solution."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2023-02-27T13:00:00Z'
date_end: '2023-02-27T15:00:00Z'
all_day: false

# # Schedule page publish date (NOT talk date).
# publishDate: '2017-01-01T00:00:00Z'

# authors: []
# tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  caption: 'Image credit: [**HPCA 2023**](https://hpca-conf.org/2023/)'
  focal_point: Right

links:
  - icon: youtube
    icon_pack: fab
    name: Video
    url: https://www.youtube.com/watch?v=AxPVr0lzP2k
# url_code: ''
# url_pdf: ''
# url_slides: ''
# url_video: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
---

<!-- {{% callout note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /callout %}} -->