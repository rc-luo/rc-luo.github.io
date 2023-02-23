---
title: "Rethinking client reweighting for selfish federated learning"
collection: publications
permalink: /publication/2022-10-01-Rethinking-client-reweighting-for selfish-federated-learning
excerpt: 'This work studys a novel setting in FL to consider biased objectives and internal/external partitions and we also propose a novel algorithm for solving it via gradients variance reduction.'
date: 2022-10-01
venue: 'In submission'
paperurl: ''
citation: 'Luo, R., Hu, S., Yu, L. et al. Rethinking client reweighting for selfish federated learning (2022). [in submission]'
featured: yes
---

*Abstract.* Most federated learning (FL) algorithms aim to learn a model which achieves optimal overall performance across all clients. However, for some clients, the model obtained by conventional federated training may perform even worse than that obtained by local training. Therefore, for a stakeholder who only cares about the performance of a few, the outcome of conventional federated learning may be unsatisfactory. To this end, we study a new variant of federated learning, in which the ultimate objective is to learn a model with optimal performance on internal clients instead of all clients. We further propose Variance Reduction Selfish Learning (VaRSeL), a novel algorithm that reweights the external clients based on variance reduction for learning a model desired in this setting. Within each round of federated training, it guides the model to update towards the direction favored by the internal clients. We give a convergence analysis for both strongly-convex and non-convex cases, highlighting its fine-tune effect. Finally, we perform extensive experiments on both synthesized and real-world datasets, covering image classification, language modeling, and medical image segmentation. Experimental results empirically justify our theoretical results and show the advantage of VaRSeL over related FL algorithms. One-sentence Summary: This work studys a novel setting in FL to consider biased objectives and internal/external partitions and we also propose a novel algorithm for solving it via gradients variance reduction.

<!-- [Download paper here](/about/) -->
