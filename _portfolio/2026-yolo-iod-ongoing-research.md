---
title: "Class-Incremental Object Detection via Knowledge Distillation"
excerpt: "Reproducing incremental-detection baselines on COCO, adapting YOLO-World with newer backbones, and redesigning KD distance measures to ease forgetting and overfitting."
collection: portfolio
priority: 1
---

Independent research (2026 - Present) · Computer Vision / Continual Learning

**Code:** [YOLO-IOD reproduction/adaptation](https://github.com/dspsrh/YOLO-IOD) · [ERD reproduction](https://github.com/dspsrh/ERD)

## Research Question

How can an object detector learn new COCO categories sequentially while retaining performance on previously learned classes without relying on large exemplar memories?

## Current Direction

I am reproducing and benchmarking continual-learning and incremental-detection baselines, including LwF, iCaRL, ERD, and YOLO-IOD. I am also rebuilding the YOLO-World open-vocabulary detection backbone with newer-generation YOLO architectures to test whether stronger feature extractors improve COCO performance under an incremental protocol.

## Technical Focus

- Studying catastrophic forgetting when detectors absorb new object categories sequentially.
- Reproducing and benchmarking LwF, iCaRL, ERD, and YOLO-IOD to analyze degradation of old-class performance under sequential class addition.
- Designing teacher-student schemes that distill logit- and feature-level knowledge from a frozen prior-task detector.
- Rebuilding the YOLO-World open-vocabulary detection backbone with newer-generation YOLO architectures.
- Redesigning the distance computation at the core of the distillation objective by replacing classic L2 distance and KL divergence between teacher and student outputs with alternative distance measures.
- Testing redesigned loss functions and direct metric substitutions to ease catastrophic forgetting and overfitting.

## Evaluation

- COCO incremental-detection splits.
- Per-step mAP and average mAP.
- Forgetting, backward transfer, and forward transfer.
- Sensitivity to the selected teacher-student distance measure in the distillation objective.

## Status

Reproduction, YOLO-World backbone, and KD distance-measure experiments are in progress; manuscript in preparation.
