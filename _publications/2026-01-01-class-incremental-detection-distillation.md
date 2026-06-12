---
title: "Knowledge Distillation for Class-Incremental Object Detection"
collection: publications
category: manuscripts
permalink: /publication/2026-class-incremental-detection-distillation
excerpt: "Reproducing incremental-detection baselines on COCO, benchmarking YOLO-World backbone swaps, and redesigning KD distance measures to ease forgetting and overfitting."
date: 2026-01-01
venue: "Manuscript in preparation"
citation: "S. Dong, &quot;Knowledge Distillation for Class-Incremental Object Detection,&quot; manuscript in preparation, 2026."
---

Ongoing independent research on class-incremental object detection. The project reproduces and benchmarks continual-learning and incremental-detection baselines, including LwF, iCaRL, ERD, and YOLO-IOD; includes a completed controlled YOLO-World backbone-swap benchmark on COCO in which YOLO12-S and YOLO26-S improved best mAP over the YOLOv8-S baseline by +0.042 and +0.041; and redesigns the distance computation at the core of the distillation objective by replacing classic L2 distance and KL divergence with alternative distance measures.

**Code:** [YOLO-World backbone swap](https://github.com/dspsrh/yolo-world-backbone-swap) · [YOLO-IOD reproduction/adaptation](https://github.com/dspsrh/YOLO-IOD) · [ERD reproduction](https://github.com/dspsrh/ERD) · [Research page](/portfolio/2026-yolo-iod-ongoing-research/)
