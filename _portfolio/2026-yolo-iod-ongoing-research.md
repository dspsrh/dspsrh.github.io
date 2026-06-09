---
title: "Class-Incremental Object Detection via Knowledge Distillation"
excerpt: "Reproducing YOLO-IOD and ERD on COCO, adapting YOLO-World with alternative backbones, and developing a smoother KD loss for stable incremental detection."
collection: portfolio
priority: 1
---

Independent research (2026 - Present) · Computer Vision / Continual Learning

**Code:** [YOLO-IOD reproduction/adaptation](https://github.com/dspsrh/YOLO-IOD) · [ERD reproduction](https://github.com/dspsrh/ERD)

## Research Question

How can an object detector acquire new COCO categories sequentially while preserving old-category performance without storing large exemplar memories?

## Current Direction

I am reproducing strong incremental object detection baselines, focusing on YOLO-IOD and ERD, then adapting YOLO-World with alternative backbone variants to study whether stronger open-vocabulary representations improve the stability-plasticity trade-off.

## Technical Focus

- Fine-tuning YOLO-World on COCO under class-incremental protocols.
- Replacing and evaluating backbone variants inside the YOLO-World detection pipeline.
- Comparing reproduced baselines against teacher-student KD variants.
- Studying gradient explosion caused by noisy teacher responses and false pseudo-labels.
- Designing a smoother KD loss that down-weights unstable teacher signals while preserving useful old-class knowledge.

## Evaluation

- COCO incremental-detection splits.
- Per-step mAP and average mAP.
- Forgetting, backward transfer, and forward transfer.
- Stability of training dynamics, including KD-loss scale and gradient norms.

## Status

Reproduction and backbone experiments in progress; manuscript in preparation.
