---
title: "Elastic Response Distillation (ERD) Reproduction"
excerpt: "Reproducing ERD for incremental object detection as a continual-learning baseline."
collection: portfolio
priority: 2
hidden: true
---

**[View code on GitHub](https://github.com/dspsrh/ERD)** · [Flagship research project](/portfolio/2026-yolo-iod-ongoing-research/)

This project reproduces Elastic Response Distillation as a baseline for class-incremental object detection. I use it to compare how response-level distillation behaves against YOLO-IOD-style teacher-student training and against my planned distance-measure redesign for YOLO-World-based incremental detection.

The reproduction focuses on matching the original protocol closely enough to make later backbone and loss-function changes interpretable rather than mixing implementation changes with method changes.
