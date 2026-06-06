---
title: "Class-Incremental Object Detection via Knowledge Distillation"
excerpt: "Ongoing research on catastrophic forgetting in incremental detection on COCO."
collection: portfolio
---

**[View code on GitHub](https://github.com/dspsrh/YOLO-IOD)** · Related baseline: [ERD](https://github.com/dspsrh/ERD)

Independent research (2026 – Present) · Computer Vision / Continual Learning

* Studying catastrophic forgetting in class-incremental object detection on the COCO benchmark, where a single detector must absorb new object categories sequentially while retaining prior ones—framing the problem as a measurable stability–plasticity trade-off.
* Reproducing and dissecting continual-learning and incremental-detection baselines—Learning without Forgetting (LwF), iCaRL, Elastic Response Distillation (ERD), and YOLO-IOD—to isolate where and why prior-class knowledge degrades under sequential class addition.
* Designing teacher–student schemes that distill logit- and feature-level knowledge from a frozen prior-task detector, testing the hypothesis that response and feature distillation preserve old-class accuracy without large exemplar memories.
* Rebuilding the YOLO-World open-vocabulary detection backbone with newer-generation YOLO architectures to test whether stronger feature extractors improve detection performance on COCO under the incremental protocol.
* Redesigning the standard knowledge-distillation loss to remain robust to the teacher detector's false pseudo-labels, easing the gradient explosion that these erroneous old-class targets induce during student training.
* Quantifying retention and plasticity under standard incremental-detection protocols on COCO—per-step and average mAP, forgetting, and backward/forward transfer; manuscript in preparation.

This work builds on the [YOLO-IOD](https://github.com/dspsrh/YOLO-IOD) framework (AAAI 2026) for real-time incremental object detection.
