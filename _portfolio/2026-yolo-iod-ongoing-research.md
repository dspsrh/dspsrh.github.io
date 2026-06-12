---
title: "Class-Incremental Object Detection via Knowledge Distillation"
excerpt: "Reproducing incremental-detection baselines on COCO, benchmarking YOLO-World backbone swaps, and redesigning KD distance measures to ease forgetting and overfitting."
collection: portfolio
priority: 1
---

Independent research (2026 - Present) · Computer Vision / Continual Learning

**Code:** [YOLO-World backbone swap benchmark](https://github.com/dspsrh/yolo-world-backbone-swap) · [YOLO-IOD reproduction/adaptation](https://github.com/dspsrh/YOLO-IOD) · [ERD reproduction](https://github.com/dspsrh/ERD)

## Research Question

How can an object detector learn new COCO categories sequentially while retaining performance on previously learned classes without relying on large exemplar memories, and how much does the detector backbone affect that stability-plasticity trade-off?

## Current Direction

I am reproducing and benchmarking continual-learning and incremental-detection baselines, including LwF, iCaRL, ERD, and YOLO-IOD. As a foundation for that work, I completed a controlled YOLO-World backbone-swap benchmark on COCO, replacing the default YOLOv8-S image backbone with YOLOv9-S, YOLOv10-S, YOLO11-S, YOLO12-S, and YOLO26-S while holding the text encoder, neck/head recipe, training data, and evaluation protocol fixed.

## Technical Focus

- Studying catastrophic forgetting when detectors absorb new object categories sequentially.
- Reproducing and benchmarking LwF, iCaRL, ERD, and YOLO-IOD to analyze degradation of old-class performance under sequential class addition.
- Designing teacher-student schemes that distill logit- and feature-level knowledge from a frozen prior-task detector.
- Building a non-invasive `UltralyticsYOLOBackbone` adapter that plugs newer Ultralytics YOLO backbones into YOLO-World through the MMYOLO registry without editing YOLO-World source.
- Probing P3/P4/P5 feature channels automatically so each YOLO-World neck/head config matches the substituted backbone.
- Redesigning the distance computation at the core of the distillation objective by replacing classic L2 distance and KL divergence between teacher and student outputs with alternative distance measures.
- Testing redesigned loss functions and direct metric substitutions to ease catastrophic forgetting and overfitting.

## Backbone-Swap Benchmark

I trained YOLO-World-S variants on COCO 2017 under an identical recipe. The YOLOv8-S baseline was trained for 80 epochs; newer backbones were first screened for 40 epochs, then contenders were promoted to 80 epochs. The 40-epoch ranking matched the final 80-epoch ranking, supporting the screen-to-promote workflow.

| backbone | mAP@40 | best mAP | best epoch | vision params | GFLOPs | fp16 FPS | vs v8 best |
| --- | --- | --- | --- | --- | --- | --- | --- |
| YOLO12-S | 0.462 | **0.470** | 71 | 17.05M | 30.0 | 64.6 | **+0.042** |
| YOLO26-S | 0.455 | **0.469** | 77 | 17.04M | 28.6 | 83.8 | **+0.041** |
| YOLO11-S | 0.452 | 0.458 | 69 | 17.04M | 28.6 | 85.0 | +0.030 |
| YOLOv10-S | 0.444 | 0.448 | 65 | 11.57M | 16.0 | 84.8 | +0.020 |
| YOLOv8-S baseline | 0.421 | 0.428 | 69 | 12.76M | 16.4 | 95.6 | baseline |
| YOLOv9-S | 0.415 | 0.415 | 40 | 7.09M | 13.3 | 58.8 | -0.013 |

Key findings: every newer backbone except YOLOv9-S improved over the YOLOv8-S baseline; YOLO12-S and YOLO26-S gave the largest mAP gains; YOLOv10-S was the strongest Pareto option because it improved mAP while using fewer vision parameters and FLOPs than YOLOv8-S. The gains from YOLO11/12/26 appear to come largely from small-object performance, consistent with their wider P3 feature maps.

## Evaluation

- COCO incremental-detection splits.
- Per-step mAP and average mAP.
- Forgetting, backward transfer, and forward transfer.
- Sensitivity to the selected teacher-student distance measure in the distillation objective.
- Backbone-ablation metrics: COCO val2017 bbox mAP, AP50/AP75, AP-small/medium/large, vision parameters, GFLOPs, and batch-1 latency/FPS with cached text features.

## Status

Backbone-swap benchmark complete; incremental-detection baseline reproduction and KD distance-measure experiments are in progress; manuscript in preparation.
