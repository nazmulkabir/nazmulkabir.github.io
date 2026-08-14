---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Download the full CV: [PDF](/cv/Full_CV.pdf) &middot; [short version](/cv/Resume_Sikder_short.pdf)

Publications appear under **M. N. K. Sikder**; pre-2016 work under **N. K. Sikder**.

Professional Summary
======

Research Assistant Professor focused on Generative AI security, cybersecurity, critical
infrastructure protection, and trustworthy embedded AI. Previously a Presidential
Postdoctoral Fellow specializing in secure, privacy-aware, and explainable AI for critical
infrastructure. My research spans hybrid AI — including LLMs, agentic AI, computer vision,
and time-series forecasting — to secure AI-enabled systems, support anomaly detection, and
enable robust decision-making in cyber-physical environments, with interdisciplinary
publications and contributions to NSF proposal development.

Areas of Expertise
======

* **Critical Infrastructure and Control Systems.** SCADA and industrial control system (ICS) security; water and wastewater treatment systems; operational technology (OT) monitoring; cyber-physical system resilience.
* **Cybersecurity.** Intrusion detection and automated response; IoT and cross-layer (network/host) threat detection; adversarial machine learning; threat-intelligence grounding (MITRE ATT&CK, CVE/NVD).
* **Artificial Intelligence.** Security and trustworthiness of large language models and agentic AI systems; AI assurance, validation, and explainability; anomaly detection; time-series forecasting; generative modeling (GANs, diffusion models).
* **Digital Media Forensics.** Detection and source attribution of synthetic and adversarially manipulated imagery.
* **Telecommunications.** LTE radio access network rollout, operations, and monitoring automation.

Academic Appointments
======

* **Research Assistant Professor**, Old Dominion University, Norfolk, VA — December 2025 to present
* **Presidential Postdoctoral Fellow**, Virginia Tech, Arlington, VA — January 2025 to December 2025
* **Graduate Research Assistant**, Virginia Tech, Arlington, VA — August 2019 to December 2024

Education
======

* **Ph.D., Computer Engineering**, Virginia Polytechnic Institute and State University, Arlington, VA — August 2019 to December 2024
  * Dissertation: *AI Methods for Anomaly Detection in Cyber-Physical Systems: With Application to Water and Agriculture*. Chair: Feras A. Batarseh. [Link](https://hdl.handle.net/10919/124470)
* **M.S., Computer Engineering**, Virginia Polytechnic Institute and State University, Falls Church, VA — August 2019 to May 2022
  * GPA: 3.67/4.0
* **B.S., Electrical and Electronic Engineering**, Bangladesh University of Engineering and Technology (BUET), Dhaka, Bangladesh — May 2010 to September 2015
  * GPA: 3.65/4.0

Honors, Awards, and Fellowships
======

* **Presidential Postdoctoral Fellow** (competitive university-wide fellowship), Virginia Tech, 2025
* **Winner**, [2022 Intelligent Water Systems Challenge](https://www.waterrf.org/news/2022-intelligent-water-systems-challenge), The Water Research Foundation
* 2nd best team, line following robot contest, BUET, 2014

Research Interests
======

Security and Trustworthiness of LLMs and Agentic AI; Cybersecurity; Trustworthy and Secure
Embedded AI for Cyber-Physical Systems; Anomaly Detection and AI Assurance.

Publications
======

  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Research Funding and Grant Activity
======

**Awarded**

* **Commonwealth Cyber Initiative (CCI).** *Agentic AI for Scalable and Cost-Effective Protection of Critical Infrastructure.* Total award: $100,000; period: 1 year. Role: Co-PI / Senior Personnel. PI: Daniel Takabi; Co-PI: Murat Kantarcioglu. Institutions: Old Dominion University, Virginia Tech.

**Submitted / Under Review**

* **National Science Foundation (Cyber-Physical Systems Program).** *Securing Water and Agricultural Cyber-Physical Systems Using Foundational AI.* Total budget: $1,000,000; duration: 4 years. Role: Senior Personnel and Methodology Lead. PI: Feras A. Batarseh; Co-PIs: Manish Bansal, Jonathan Czuba, Dong Ha, Abhilash Chandel, Azahar Ali. Institution: Virginia Tech.

**Planned / Targeted Proposals (PI or Co-PI)**

* **NSF Secure and Trustworthy Cyberspace (SaTC 2.0).** Secure and trustworthy generative-AI systems for cyber-physical and critical-infrastructure security. Target submission 2026.
* **NSF Cyber-Physical Systems (CPS).** AI-enabled security, privacy, and resilience for networked and embedded cyber-physical systems. Target submission 2026.
* **DARPA (I2O) Office-Wide BAA.** Robust and secure agentic-AI and generative-AI systems for cyber operations and critical-infrastructure defense. Rolling through 2026.
* **Office of Naval Research (ONR) Long-Range BAA.** Trustworthy AI and secure machine learning for resilient cyber-physical and autonomous systems. Rolling through 2026.
* **National Lab Partnerships (e.g., PNNL / DOE).** AI-accelerated adversary emulation and cyber-defense for water, energy, and industrial control systems.

Research Experience
======

**Research Assistant Professor — Old Dominion University**

* Co-Investigator on a CCI-funded program developing agentic AI for scalable, cost-constrained protection of critical infrastructure, spanning threat detection, automated response, and operational deployment cost.
* Designed and implemented **H-CLAIR**, a two-tier cross-layer intrusion detection and response framework pairing an always-on lightweight ensemble (isolation forest, random forest, autoencoder, TabNet, graph attention networks) fused by weight-of-evidence log-odds with an LLM verifier grounded in MITRE ATT&CK and CVE/NVD, and a constrained-MDP response agent over a bounded action space. Evaluated across network and host layers on ToN_IoT, SWaT, and WADI.
* Built a production-grade agentic anomaly detection pipeline for multilayer network data on the Wahab HPC cluster (SLURM scheduling, H100 GPUs, containerized inference, retrieval-augmented multi-model ensemble).
* Improved graph deviation network (GDN) anomaly detection on industrial control system benchmarks via orthogonal initialization, a frozen reconstruction decoder, and model ensembling.
* Authored or co-authored 2 federal and foundation proposals, including NSF SaTC and Schmidt Sciences submissions.
* Supervising 2 graduate students.

**Presidential Postdoctoral Fellow — Virginia Tech, Commonwealth Cyber Initiative (CCI)**

* Led design and prototyping of LLM- and computer-vision-based anomaly detection systems for critical infrastructure, including benchmarked evaluation harnesses comparing classical and deep learning approaches to reduce false alerts.
* Developed production-ready trustworthy-AI components: data-quality validation, retraining triggers, model cards, and containerized inference pipelines, with interdisciplinary engineering and operations teams.
* Senior Personnel and methodology lead on a large-scale NSF CPS proposal, contributing system architecture, experimental design, and evaluation frameworks.

**Graduate Research Assistant — Virginia Tech, Commonwealth Cyber Initiative (CCI)**

* Developed advanced AI models (High Confidence AutoEncoders, GANs) for real-time cyber-physical threat detection in water supply systems.
* Built a context-aware forecasting framework (Temporal Fusion Transformer) integrating external data for improved water systems prediction.
* Developed AI-based decision support and anomaly detection for SCADA using deep recurrent models (LSTM/GRU).
* Applied isolation-forest-based modeling for agricultural production forecasting and policy analysis.
* Contributed to AI assurance methods for fairness, security, and explainability.

**Graduate Research Assistant — Virginia Tech, Advanced Research Institute**

* Developed data-driven energy-efficient building models using real-time data to support HVAC optimization.
* Performed demand-response analysis for appliance scheduling and AI-based policy recommendations.

Industry and Professional Experience
======

**AI Systems Lead — DC Water Operational Analytics, Washington, DC (2023–2025)**

* Led development, deployment, and validation of AI-driven embedded systems for real-time wastewater tunnel monitoring and anomaly detection at one of the largest municipal water utilities in the United States.
* Delivered production components in live operational use: data-quality validation, retraining triggers, model cards, and containerized inference pipelines, with utility engineering and operations staff.
* Benchmarked deep learning approaches against classical baselines to reduce false alert rates supporting operator decision-making.

**BEM Controls LLC, McLean, VA — Graduate Research Intern (May 2020 – August 2020)**

* Developed and tested enterprise-level smart grid software (BEMOSS) for device-level load control across heterogeneous communication protocols and demand response estimation.

**Grameenphone Ltd., Dhaka, Bangladesh — System Engineer (October 2015 – July 2019)**

* Led LTE network rollout execution in Dhaka city; recognized for rapid rollout performance.
* Designed and maintained a Telegram bot Android application for network monitoring and maintenance.
* Developed protection systems and operational tools (billing automation, fuel generator controller) reducing operational expenditure.

Teaching
======

  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

**Teaching Interests:** Trustworthy and Secure AI; Cybersecurity and Critical Infrastructure;
Machine Learning for Cyber-Physical Systems; Generative AI and LLM Security; Applied Deep
Learning (Vision and Time Series); AI Assurance and Anomaly Detection.

Advising and Mentoring
======

* **Trey Ward** (M.S. student, Virginia Tech). Co-mentored for a journal manuscript in preparation on secure and trustworthy computer vision for agricultural cyber-physical systems. Supervised problem formulation, experimental design, model development, and manuscript preparation.
* **Shubham Deshmukh** (M.S. student, Virginia Tech). Co-mentored on the same project, contributing dataset generation, adversarial and generative modeling pipelines, and evaluation of detection and attribution models.
* **Research project:** *Unified Detection and Attribution of Synthetic and Adversarial Images in Agricultural Cyber-Physical Systems.* Designed a multi-generator evaluation framework using GANs (StyleGAN2, StyleGAN3, R3GAN) and diffusion models (InstructPix2Pix, BLIP-Diffusion, Dreamshaper-8) across apple, maize, and tomato, guiding use of CNN and Vision-Transformer backbones (EfficientNet-B0, ResNet-50, CLIP) for health-state classification, source detection, and generator attribution.
* Trained students in reproducible ML pipelines, dataset curation, cross-model evaluation, and scientific writing.

Professional Service
======

**Proposal Review and Panel Service**

* **Commonwealth Cyber Initiative (CCI), Virginia — External Reviewer (2025).** Reviewed and formally scored proposals for the CCI Request for Proposals: Cybersecurity for Critical Infrastructure.

**Peer Review and Editorial Service**

* Environmental Monitoring and Assessment (Springer Nature), 2026
* Journal of the ASABE (American Society of Agricultural and Biological Engineers), 2025
* Journal of Computer Virology and Hacking Techniques (Springer Nature), 2025
* Scientific Reports (Nature Portfolio), 2025
* International Journal of Data Science and Analytics (Springer Nature), 2025
* Environmental Health (Springer Nature), 2025
* SN Computer Science (Springer Nature), 2025
* Neural Computing and Applications (Springer Nature), 2025
* Journal of Cybersecurity and Privacy (MDPI), 2025

Leadership and Outreach
======

* **AI Systems Lead**, DC Water Operational Analytics, 2023–2025
* Volunteer, IEEE Innovation Smart Grid Technologies (ISGT), North America, 2020
* Volunteer, AEE World Energy Conference and Expo, Washington, DC, 2019
* Coordinator, Inter-university Project Show and Departmental Festival, 2014
* Organizing Member, PES 2014 Inter-university Robotics Competition, BUET Energy Club

Talks and Presentations
======

  <ul>{% for post in site.talks %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Open-Source Software and Datasets
======

* **[Context-Driven Forecasting](https://github.com/nazmulkabir/Context_water)** (dataset + code). Dataset and reproducible software package supporting the context-driven forecasting study: time-series data processing, modeling, and evaluation.
* **[AgriVision Synthetic/Adversarial Image Detection](https://github.com/AI-VTRC/AgriVision.AI)** (dataset + framework). Curated dataset for synthetic/adversarial image detection in agriculture, with a benchmark framework for detection and attribution experiments.

Projects
======

  <ul>{% for post in site.portfolio %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Technical Skills
======

* **Programming:** Python, C++, SQL
* **ML/AI:** PyTorch, TensorFlow, Keras; Hugging Face Transformers; Ray RLlib
* **Data:** Pandas, NumPy, Scikit-learn; Apache Spark
* **DevOps/MLOps:** Docker, Kubernetes, Jenkins, Apache Airflow; MLflow; Weights & Biases; Terraform
* **Cloud/Edge:** AWS (SageMaker), Azure, Google Cloud; TensorFlow Lite; AWS IoT
* **Security:** OpenSSL, JWT, PyCrypto

Professional Memberships
======

* Institute of Electrical and Electronics Engineers (IEEE) — Member; IEEE Computer Society
* Association for Computing Machinery (ACM) — Member

Media Coverage
======

* [Intelligent Water Systems Challenge winner coverage](https://www.waterrf.org/news/2022-intelligent-water-systems-challenge), The Water Research Foundation
* [Virginia Tech: AI solution implementation at DC Water](https://vtx.vt.edu/videos/k/2022/09/1_029flkz1.html)
* [Commonwealth Cyber Initiative: protecting water systems from cyber threats](https://cyberinitiative.org/cci-news/2022)

References
======

Available on request.
