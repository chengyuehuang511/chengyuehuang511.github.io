---
title: "Rethinking Weight Decay for Robust Fine-Tuning of Foundation Models"
collection: publications
permalink: /publications/spd
excerpt: 'This paper introduces Selective Projection Decay (SPD), a weight decay technique that selectively regularizes certain layers to balance fitting and retaining pre-trained knowledge, improving generalization and robustness when fine-tuning foundation models.'
date: 2024-09-25
venue: 'NeurIPS 2024'
paperurl: 'https://openreview.net/forum?id=4neqdBz8eG'
---
![An illustration of PowerEmbed method.](/images/spd.png)

Modern optimizers such as AdamW, equipped with momentum and adaptive learning rate, are designed to escape local minima and explore the vast parameter space. This exploration is beneficial for finding good loss basins when training from scratch. It is not necessarily ideal when resuming from a powerful foundation model because it can lead to large deviations from the pre-trained initialization and, consequently, worse robustness and generalization. At the same time, strong regularization on all parameters can lead to under-fitting. We hypothesize that selectively regularizing the parameter space is the key to fitting and retraining the pre-trained knowledge. This paper proposes a new weight decay technique, Selective Projection Decay (SPD), that selectively imposes a strong penalty on certain layers while allowing others to change freely. Intuitively, SPD expands and contracts the parameter search space for layers with consistent and inconsistent loss reduction, respectively. Experimentally, when equipped with SPD, Adam consistently provides better in-distribution generalization and out-of-distribution robustness performance on multiple popular vision and language benchmarks.

[Download paper here.](https://openreview.net/forum?id=4neqdBz8eG)
