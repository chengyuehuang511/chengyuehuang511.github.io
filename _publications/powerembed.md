---
title: "From Local to Global: Spectral-Inspired Graph Neural Networks"
collection: publications
permalink: /publications/powerembed
excerpt: 'This paper is about mitigating over-smoothing and over-squashing issues in deep GNNs by proposing a normalization technique in message-passing algorithms (PowerEmbed) to encode global spectra information inspired by spectral embeddings.'
date: 2022-09-24
venue: 'NeurIPS GLFrontiers Workshop'
paperurl: 'https://openreview.net/forum?id=DhICIwGint_'
---
![An illustration of PowerEmbed method.](/images/power_sign_pic.png)

Graph Neural Networks (GNNs) are powerful deep learning methods for Non-Euclidean data. Popular GNNs are message-passing algorithms (MPNNs) that aggregate and combine signals in a local graph neighborhood. However, shallow MPNNs tend to miss long-range signals and perform poorly on some heterophilous graphs, while deep MPNNs can suffer from issues like over-smoothing or over-squashing. To mitigate such issues, existing works typically borrow normalization techniques from training neural networks on Euclidean data or modify the graph structures. Yet these approaches are not well-understood theoretically and could increase the overall computational complexity. In this work, we draw inspirations from spectral graph embedding and propose PowerEmbed -- a simple layer-wise normalization technique to boost MPNNs. We show PowerEmbed can provably express the top-k leading eigenvectors of the graph operator, which prevents over-smoothing and is agnostic to the graph topology; meanwhile, it produces a list of representations ranging from local features to global signals, which avoids over-squashing. We apply PowerEmbed in a wide range of simulated and real graphs and demonstrate its competitive performance, particularly for heterophilous graphs.

[Download paper here.](https://openreview.net/forum?id=DhICIwGint_)

[Download slides here.](https://chengyuehuang511.github.io/files/spectral_inspired_gnn_pre.pdf)
