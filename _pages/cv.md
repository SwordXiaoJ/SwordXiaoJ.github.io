---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Ph.D. in Computer Science & Engineering**, Washington University in St. Louis, Aug. 2025 – Present
  * Advisor: Dr. Ning Zhang
  * Research focus: AI security, with emphasis on distributed AI security, Agent security, and LLM security
* **M.Eng. in Computer Engineering**, Duke University, Aug. 2022 – May 2024
  * GPA: 3.91 / 4.00
  * Key Courses: Algorithms, Computer System, Robust Server, Reliable System, Advanced Computer Network
* **B.Eng. in Software Engineering**, Beijing Jiaotong University, Sep. 2017 – June 2021
  * GPA: 3.9 / 4.00 (top 3% out of 172)
  * Key Courses: Calculus, Discrete Mathematics, Probability Theory and Mathematical Statistics, Geometry and Algebra, Computer Network, Operating System

Research Experience
======
* **Three-Layer Federated Learning with Momentum to Solve Non-IID** (Dec. 2023 – Aug 2025)
  * Research Assistant; Advisors: Dr. Enmao Diao and Prof. Jie Ding, University of Minnesota (ColAI)
  * Proposed a three-layer Federated Learning algorithm (local, fed, global) with momentum to address non-IID issues, managing variance at different levels: local for within-client iterations, fed for coordination across clients, and global for coordination across iterations. The structure reduces to FedAvg through hyperparameter adjustments.
  * Enhanced the FLPipe code to integrate Ray for federated learning. Deployed Ray on AWS and modularized the federated learning logic into client, controller, and server files. The controller manages the server and its local database, enabling experiment resumption and testing through local parameter saving and restoration.
  * Used SGD and CosineAnnealingLR with full gradient descent in a CIFAR-10 CNN setup with non-IID data. By adjusting only the local learning rate and momentum, reached up to 79.60% accuracy in an extreme case. Further tuning of the fed-level parameters increased accuracy to ~82.00%, compared to ~84.00% under IID.
  * Implemented a code resumption mechanism, enabling complete replication of results under a round-robin sampling strategy after interruptions, ensuring consistent experimental outcomes.
  * Designed and implemented a robust benchmarking framework for evaluating advanced federated learning algorithms across diverse neural network architectures, optimizers, datasets, and hyperparameter configurations.
  * Currently porting FedDyn, FedGen, FedProx, FedNova, and SCAFFOLD into the proposed framework to expand its functionality and adaptability.

* **DXF Drawings AutoGrader** (April 2024 – Aug 2025)
  * Research Assistant; Advisor: Prof. Rabih Younes, Duke University
  * Designed and deployed a scalable CAD grader using React and Flask to automate assessment of DXF files. Used Nginx, Gunicorn, and systemctl for deployment and Locust for performance testing on a Linux server.
  * Leveraged the `ezdxf` library for automated detection of geometric entities and error types, including color, lineweight, scale, rotation, and hatching errors, ensuring modular and extensible back-end development.
  * Exploring CNN for image recognition and geometric feature extraction, and GNN for precise error detection and classification of entities, scaling, and rotation errors, with plans to enhance model accuracy and generalization through advanced data augmentation.

* **Students Acceptance Optimizer** (May 2023 – Oct. 2023)
  * Research Assistant; Advisor: Prof. Rabih Younes, Duke University
  * Developed a student acceptance optimizer that predicts students' first-year GPA at Duke based on application metrics (GPA, undergraduate institution, GRE, TOEFL, etc.) to provide references for the ECE admissions team.
  * Implemented two-level cross-validation to select the optimal LASSO regression model with the highest coefficient of determination. Fine-tuned a pre-trained BERT model and used the resulting sentiment scores to label letters of recommendation as positive, negative, or neutral.
  * Developed a user-friendly GUI with PyQt. Used Nuitka to package the Python project into executables for Windows and macOS.

* **Improved Two-stream Network for Action Recognition** (June 2020 – May 2021)
  * Research Assistant; Advisor: Prof. Weiwei Xing, Beijing Jiaotong University
  * Participated in developing a multi-stream model combining LSTM and DenseNet for action recognition. The model uses RGB video frames and optical flow, with a spatial stream for frame analysis, a temporal stream for flow processing, and an SVM fusion layer for final classification.
  * Contributed to integrating CNN and LSTM in the spatial stream for capturing both spatial and temporal patterns from RGB video frames.
  * Achieved 91.25% accuracy on the UCF-101 dataset using an improved two-stream network with DenseNet and LSTM.

* **Computer Vision-Based Railway Signal Light Distance Measurement** (June 2020 – May 2021)
  * Research Assistant; Advisor: Prof. Weiwei Xing, Beijing Jiaotong University
  * Proposed a distance measurement method to detect the distance between a train and a signal light based on signal-light position and railway track line expression, helping drivers make better decisions and avoid risks.
  * For the signal-lamp component, used different datasets to handle single and multiple signal lamps. Applied OpenCV with a Hough-transform-based recognition method and left-right track line screening for straight tracks; used a perspective-transform-and-fitting method for curved tracks.
  * Experimented under multiple weather conditions and at various distances; achieved error rates as low as 3%.
  * Awarded excellent thesis recommendation (Top 10%) for senior thesis.

Course Projects
======
* **HTTP Caching Proxy Server** — C++, Socket Programming (Jan. 2023 – March 2023)
  * Developed an HTTP caching proxy server in C++ that handles GET, POST, and CONNECT requests.
  * Used multi-threading to handle concurrent requests, a read-write lock for log management, socket programming for packet handling, and RAII / smart pointers to ensure strong exception guarantees.
  * Improved performance by caching responses with an LRU policy. Implemented validation and expiration rules following RFC 7234, including ETag and Last-Modified for re-validation, and `max-age` / `no-store` / `no-cache` / `must-revalidate` handling in the Cache-Control field.

Technical Skills
======
* **Languages**: C/C++, Python (PyTorch, scikit-learn, Pandas, NumPy), Java, SQL, JavaScript, HTML/CSS
* **Developer Tools**: Git, Linux, Vim, Docker, Kubernetes, Visual Studio, PyCharm, AWS, Ray

Awards
======
* University-Level Outstanding Student Award — Dec. 2018, 2019, 2020
* First-class Outstanding Academic Performance Scholarship (top 3%) — Dec. 2020
* Second-class Outstanding Academic Performance Scholarship (top 10%) — Dec. 2018, 2019
* Wntime Scholarship of Beijing Jiaotong University (2 / 171) — Dec. 2020

<!-- Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul> -->


