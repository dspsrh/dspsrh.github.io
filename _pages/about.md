---
permalink: /
title: "Shuaipeng (Frank) Dong"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

My research interests are in **computer vision**, **continual learning**, and **knowledge distillation**, especially class-incremental object detection: how detectors can learn new categories over time while retaining old ones under realistic memory and compute constraints.

Current Research Focus
======
**Knowledge Distillation for Class-Incremental Object Detection** (2026 - Present)

I am fine-tuning and adapting YOLO-World on COCO while reproducing state-of-the-art incremental object detection baselines, with the goal of developing a more stable KD objective for sequential class learning.

- Reproducing incremental-learning and KD baselines for object detection, including YOLO-IOD, Elastic Response Distillation (ERD), Learning without Forgetting (LwF), and iCaRL-style rehearsal/distillation comparisons.
- Fine-tuning YOLO-World on COCO and replacing / testing backbone variants to study how representation strength affects retention and plasticity in incremental detection.
- Investigating gradient instability caused by noisy teacher responses and false pseudo-labels during distillation.
- Designing a smoother KD loss that reduces gradient explosion while preserving old-class detection performance.
- Evaluating under standard COCO incremental-detection protocols using per-step mAP, average mAP, forgetting, backward transfer, and forward transfer.

**Code:** [YOLO-IOD reproduction/adaptation](https://github.com/dspsrh/YOLO-IOD) · [ERD reproduction](https://github.com/dspsrh/ERD)  
**Status:** Manuscript in preparation · [Read more about this research](/portfolio/2026-yolo-iod-ongoing-research/)

Research Outputs
======
- Manuscript in preparation: Knowledge Distillation for Class-Incremental Object Detection.
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
