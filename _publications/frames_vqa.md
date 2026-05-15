---
title: "FRAMES-VQA: Benchmarking Fine-Tuning Robustness across Multi-Modal Shifts in Visual Question Answering"
collection: publications
permalink: /publications/frames_vqa
excerpt: 'We introduce FRAMES-VQA, a benchmark designed to evaluate robust fine-tuning strategies for visual question answering (VQA) under diverse multi-modal distribution shifts. By leveraging ten existing VQA datasets categorized into in-distribution (ID), near-OOD, and far-OOD scenarios, we systematically analyze the impact of uni-modal, multi-modal, and adversarial shifts. Our study compares existing robust fine-tuning methods, quantifies distribution shifts using Mahalanobis distance, and explores the interactions between uni- and multi-modal shifts, providing valuable insights for developing more robust VQA models.'
date: 2025-02-26
venue: 'CVPR'
paperurl: 'https://arxiv.org/abs/2505.21755'
authors: 'Chengyue Huang, Brisa Maneechotesuwan, Shivang Chopra, Zsolt Kira'
header:
  teaser: vqa_pics.png
---
![An illustration of FRAMES-VQA method.](/images/vqa_pics.png)

Visual question answering (VQA) systems face significant challenges when adapting to real-world data shifts, especially in multi-modal contexts. While robust fine-tuning strategies are essential for maintaining performance across in-distribution (ID) and out-of-distribution (OOD) scenarios, current evaluation settings are primarily unimodal or particular to some types of OOD, offering limited insight into the complexities of multi-modal contexts. In this work, we propose a new benchmark FRAMES-VQA (Fine-Tuning Robustness across Multi-Modal Shifts in VQA) for evaluating robust fine-tuning for VQA tasks. We utilize ten existing VQA benchmarks, including VQAv2, IV-VQA, VQA-CP, OK-VQA and others, and categorize them into ID, near and far OOD datasets covering uni-modal, multi-modal and adversarial distribution shifts. We first conduct a comprehensive comparison of existing robust fine-tuning methods. We then quantify the distribution shifts by calculating the Mahalanobis distance using uni-modal and multi-modal embeddings extracted from various models. Further, we perform an extensive analysis to explore the interactions between uni- and multi-modal shifts as well as modality importance for ID and OOD samples. These analyses offer valuable guidance on developing more robust fine-tuning methods to handle multi-modal distribution shifts.

[Download paper here.](https://arxiv.org/abs/2505.21755)
