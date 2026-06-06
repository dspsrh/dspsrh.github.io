---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Download Academic CV (PDF): [cv.pdf](/files/cv.pdf)

Research Interests
======
Computer vision, continual learning, and knowledge distillation, with a focus on class-incremental visual recognition and memory-efficient lifelong learning for image classification and object detection.

Education
======
* **The Pennsylvania State University**, University Park, PA — May 2023
  * B.S. in Computer Science · B.S. in Mathematics (Systems Analysis)
  * Cumulative GPA: 3.55 / 4.00 · Dean's List (multiple semesters) · College Honors Student

Publications & Patents
======
{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}

Research Experience
======
* **Knowledge Distillation for Class-Incremental Visual Recognition** — 2026 – Present
  * Independent Research · Computer Vision / Continual Learning
  * Studying catastrophic forgetting in class-incremental object detection on COCO; reproducing LwF, iCaRL, ERD, and YOLO-IOD baselines; designing teacher–student distillation schemes; quantifying mAP, forgetting, and transfer.
  * Code: [YOLO-IOD](https://github.com/dspsrh/YOLO-IOD) · [ERD](https://github.com/dspsrh/ERD) · Manuscript in preparation.

* **Deep Convolutional Neural Networks for Medical Image Classification** — 2022
  * Undergraduate Research · The Pennsylvania State University
  * Designed a depth-wise separable CNN for invasive ductal carcinoma detection from histopathology; first-author publication at ICAIE 2022.
  * Code: [Breastcancer_CNN](https://github.com/dspsrh/Breastcancer_CNN)

Professional & Applied Research Experience
======
* **Hughes Network Systems** — June 2023 – Dec. 2025
  * Member of Technical Staff II, Software Engineering · Germantown, MD
  * Deep 3D-CNN rain-fade prediction (>90% accuracy); LSTM bandwidth prediction (ICSSC 2024, pending patent); end-to-end ML pipelines and distributed training (Docker, Kubernetes).

* **NextTier** — June 2024 – Sept. 2024
  * Software Engineer Intern — AI Reasoning Agents
  * Multi-agent LLM system with RAG, dynamic tool use, and structured evaluation (task success rate, tool-call efficiency, failure recovery).

Selected Projects
======
* **ResNet-50 from Scratch** — [Residual_Network](https://github.com/dspsrh/Residual_Network): ~87.5% test accuracy on six-class hand-sign classification.
* **Stacked LSTM Stock Forecasting** — [stock_prediction_model](https://github.com/dspsrh/stock_prediction_model): next-step forecasting for GOOG and ORCL.

Relevant Coursework
======
* **Machine Learning & AI:** Machine Learning & Artificial Intelligence (A−)
* **Mathematics & Statistics:** Linear Algebra (A), Real Analysis (A), Probability Theory (A), Linear Programming (A−), Matrices (A), Multivariable & Vector Calculus (A), Differential Equations (A−), Mathematical Statistics, Discrete Mathematics, Graph Theory
* **Computer Science:** Programming Language Concepts (A−), Digital Logic Design (A−), Numerical Analysis I & II, Data Structures & Algorithms, Theory of Computation, Operating Systems, Systems Programming

Technical Skills
======
* **Languages:** Python, C++, C, Java, MATLAB
* **ML / DL:** PyTorch, TensorFlow, Keras, MMDetection, OpenCV, Scikit-learn, NumPy, Pandas; CNNs, 3D-CNNs, LSTMs; object detection (YOLO, YOLO-World), knowledge distillation, continual learning
* **Systems / Tools:** Linux, Docker, Kubernetes, Git, FastAPI, PostgreSQL, Jenkins
