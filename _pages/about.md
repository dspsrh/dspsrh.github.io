---
permalink: /
title: "Shuaipeng (Frank) Dong"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

My research interests include **computer vision**, **continual learning**, and **knowledge distillation**, with a focus on class-incremental visual recognition and memory-efficient lifelong learning for image classification and object detection.

Current Research Focus
======
**Knowledge Distillation for Class-Incremental Object Detection** (2026 - Present)

I study catastrophic forgetting in class-incremental object detection on COCO, where detectors must learn new categories sequentially while retaining performance on previously learned classes.

- Reproducing and benchmarking continual-learning and incremental-detection baselines, including LwF, iCaRL, ERD, and YOLO-IOD, to analyze degradation of old-class performance under sequential class addition.
- Designing teacher-student schemes that distill logit- and feature-level knowledge from a frozen prior-task detector, testing whether response and feature distillation preserve old-class accuracy without large exemplar memories.
- Completed a controlled YOLO-World backbone-swap benchmark on COCO, replacing the YOLOv8-S image backbone with YOLOv9-S, YOLOv10-S, YOLO11-S, YOLO12-S, and YOLO26-S through a non-invasive adapter.
- Found that YOLO12-S and YOLO26-S gave the strongest accuracy gains over the YOLOv8-S baseline (+0.042 and +0.041 best mAP), while YOLOv10-S was a Pareto improvement with +0.020 mAP using fewer vision parameters and FLOPs.
- Redesigning the distance computation at the core of the distillation objective by replacing classic L2 distance and KL divergence between teacher and student outputs with alternative distance measures, through redesigned loss functions or direct metric substitution.
- Quantifying retention and plasticity under standard COCO incremental-detection protocols using per-step and average mAP, forgetting, and backward/forward transfer.

**Code:** [YOLO-World backbone swap benchmark](https://github.com/dspsrh/yolo-world-backbone-swap) · [YOLO-IOD reproduction/adaptation](https://github.com/dspsrh/YOLO-IOD) · [ERD reproduction](https://github.com/dspsrh/ERD)  
**Status:** Manuscript in preparation · [Read more about this research](/portfolio/2026-yolo-iod-ongoing-research/)

Research Outputs
======
- Manuscript in preparation: Knowledge Distillation for Class-Incremental Object Detection.
- Completed benchmark: [YOLO-World backbone swap](https://github.com/dspsrh/yolo-world-backbone-swap), a controlled COCO ablation comparing YOLOv8-S through YOLO26-S backbones.
- Code in progress: [YOLO-IOD reproduction/adaptation](https://github.com/dspsrh/YOLO-IOD) and [ERD reproduction](https://github.com/dspsrh/ERD).
- Prior first-author publication: depth-wise CNN for invasive ductal carcinoma detection, ICAIE 2022.
- Applied ML publication and pending patent from satellite bandwidth prediction work at Hughes Network Systems.

Education
======
**The Pennsylvania State University**, University Park, PA  
B.S. in Computer Science · B.S. in Mathematics (Systems Analysis) — May 2023  
Cumulative GPA: 3.55 / 4.00 · Dean's List (multiple semesters) · College Honors Student

Technical skills
======
* **Languages:** Python, C++, C, Java, MATLAB
* **ML / DL:** PyTorch, TensorFlow, Keras, MMDetection, OpenCV, Scikit-learn, NumPy, Pandas; CNNs, 3D-CNNs, LSTMs; object detection (YOLO, YOLO-World), knowledge distillation, continual learning
* **Systems / Tools:** Linux, Docker, Kubernetes, Git, FastAPI, PostgreSQL, Jenkins

Relevant coursework
======
* **Machine Learning & AI:** Machine Learning & Artificial Intelligence (A−)
* **Mathematics & Statistics:** Linear Algebra (A), Real Analysis (A), Probability Theory (A), Linear Programming (A−), Matrices (A), Multivariable & Vector Calculus (A), Differential Equations (A−), Mathematical Statistics, Discrete Mathematics, Graph Theory
* **Computer Science:** Programming Language Concepts (A−), Digital Logic Design (A−), Numerical Analysis I & II, Data Structures & Algorithms, Theory of Computation, Operating Systems, Systems Programming

[Download Academic CV](/files/cv.pdf) · [Google Scholar](https://scholar.google.com/citations?user=epH7UyoAAAAJ&hl=en) · [GitHub](https://github.com/dspsrh) · [LinkedIn](https://www.linkedin.com/in/shuaipeng-dong-596484234/)
