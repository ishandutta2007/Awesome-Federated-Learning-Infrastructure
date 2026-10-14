# Awesome-Federated-Learning-Infrastructure

## Top Federated Learning Infrastructure Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Privacy-Preserving Local Training, Secure Weight Aggregation & Cross-Silo Collaboration*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Federated Learning Infrastructure**. These tools enable organizations to collaboratively train AI models without sharing raw data—local training clusters push model weights to aggregators, which combine them into a global model that never sees sensitive source data.



**Examples** include Flower, FedML, OpenMined PySyft, Rhino Health, Owkin, IBM Federated Learning, Apheris, Octavian, Decentriq, and Sherpa.ai (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, cross-silo orchestration, and open secure computation — ideal for ML engineers, healthcare researchers, financial institutions, and developers seeking transparent, vendor-independent federated infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Apheris](https://www.apheris.com/)**  

  Federated data networks for drug discovery. Provides the **technical and scientific framework** for pharma companies to collaboratively train models without sharing proprietary data. **ADMET Network** (launched Feb 2026) with founding members Lundbeck, Orion Pharma, Recursion, and Servier — assembling one of the largest distributed ADMET data foundations . **AISB Network** includes AbbVie, Astex, AstraZeneca, Boehringer Ingelheim, Bristol Myers Squibb, Genentech, J&J, Sanofi, and Takeda . **Secure local inference**: models run in your environment so data, queries, and outputs stay in-house. Fine-tune models on own proprietary data within your own environment. Federated models trained across network, fine-tuned locally, with resulting models remaining private to each participant .



- **[Sherpa.ai](https://sherpa.ai/)**  

  Federated learning platform with production deployments across **finance, insurance, and healthcare**. **Inter-Bank Default Prediction**: five banks collaboratively train a global credit-risk model without transferring customer-level data — achieving **35% improvement in F1-Score and 8% in ROC-AUC** over the strongest single-bank baseline . **Fraud detection**: federated model flags coordinated structuring schemes across five banks as a single scheme — a feat impossible for any single institution. Reduces false positives by **over 30%** . **Rare disease diagnosis**: platform provided for collaboration between **U.S. National Institutes of Health (NIH) and University College London (UCL)** — federated AI models can diagnose rare diseases years earlier, slashing the "diagnostic odyssey" that lasts 5-7 years .



- **[Decentriq](https://www.decentriq.com/)**  

  Confidential computing and **trusted data clean rooms** built on **Trusted Execution Environments (TEEs)** . Enables computations on combined datasets while raw data remains encrypted and inaccessible — **even to Decentriq itself** . **Hardware-backed TEEs** with cryptographic attestation verifying only approved code runs on approved data. Meets **GDPR, HIPAA, and emerging AI regulations** . **Complements federated learning**: while FL excels at distributed model training, Decentriq enables flexible exploratory computations — cohort discovery, multi-party record linkage, cross-institutional quality assessments — on pooled sensitive data within secure enclaves . **iCARE4CVD consortium**: 30+ academic and industry institutions with 1M patient records — data linkage and AI model development time reduced by **66%** . **Swiss Re partnership**: marine insurance risk assessment without exposing portfolio data .



- **[Rhino Health](https://www.rhinohealth.com/)**  

  Federated learning platform for healthcare and life sciences. Enables multi-institutional collaboration on patient data without data movement.



- **[Owkin](https://www.owkin.com/)**  

  AI platform for biomedical research with federated learning capabilities. Features federated learning for multi-institutional data analysis and predictive biomarker discovery.



- **[Octavian](https://octavian.ai/)**  

  Federated learning infrastructure for enterprise AI. Focuses on secure multi-party model training across organizational boundaries.



## Open-Source GitHub Projects



- **[Flower (flwr)](https://github.com/adap/flower)**  

  **The leading open-source federated AI framework** — originated from a research project at the University of Oxford . **Framework-agnostic**: works with PyTorch, TensorFlow, Hugging Face Transformers, PyTorch Lightning, scikit-learn, JAX, TFLite, MONAI, fastai, MLX, XGBoost, CatBoost, LeRobot (federated robots), Pandas (federated analytics), or raw NumPy . **Customizable and extendable** — many components can be overridden for state-of-the-art systems. **Flower Baselines**: 22+ community-contributed projects reproducing popular FL publications (DASHA, FedBN, FedProx, FedNova, FedOpt, FedAvg, MOON, niid-Bench, etc.) . **Usage examples**: Android (TFLite), iOS (CoreML), Raspberry Pi & Nvidia Jetson, vertical FL, federated finetuning of Whisper, LLMs, and Vision Transformers . **The most widely adopted open-source FL framework for research and production.**



- **[FedML](https://github.com/FedML-AI/FedML)**  

  **Unified and scalable ML library for distributed training, model serving, and federated learning** (4,048+ GitHub stars) . **FEDML Launch**: cross-cloud scheduler enabling running any AI jobs on any GPU cloud or on-premise cluster . **Ecosystem**: FedNLP (NLP, NAACL 2022), FedGraphNN (Graph Neural Networks, ICLR'2021), FedCV (Computer Vision), FedIoT (IoT anomaly detection), FedML-Mobile (Android/iOS) . **Enterprise backing**: TensorOpera AI generative AI platform built on this library .



- **[IBM Federated Learning Library](https://github.com/IBM/federated-learning-lib)**  

  **Library for federated learning in an enterprise environment** (493 GitHub stars) . **Multi-backend support**: Scikit-learn, PyTorch, Keras (TensorFlow v1), TensorFlow v2, RLlib — installable in any combination . **Homomorphic Encryption (HE) support**: setup with `crypto` flag enables fully homomorphic encryption for secure aggregation — Linux only (x86 and IBM Z) . **Tutorials** for TensorFlow, PyTorch, and Scikit-learn with FHE . **Designed for enterprise-grade** federated learning deployments.



- **[OpenMined PySyft](https://github.com/OpenMined/PySyft)**  

  **Perform data science on data that remains in someone else's server** (9,469 GitHub stars) . Library for encrypted, privacy-preserving machine learning. **Note**: `syft.cpp` (SOON TO BE DEPRECATED) — OpenMined is transitioning architecture . **The foundational open-source privacy-preserving ML library** that pioneered remote data science concepts.



- **[FEDn](https://github.com/scaleoutsystems/fedn)**  

  Enterprise-ready federated learning framework — Python framework, CLI, and API . **Scalable, secure federated learning** for production deployments.



- **[FedScale](https://github.com/FedML-AI/FedScale)**  

  Scalable and extensible open-source federated learning platform (385 GitHub stars) .



### Additional Strong Open-Source Options



- **[FedJAX](https://github.com/google/fedjax)** — JAX-based open source library for Federated Learning simulations emphasizing ease-of-use in research (252 GitHub stars) .

- **[FLSim](https://github.com/facebookresearch/FLSim)** — Federated Learning Simulator — flexible, standalone core library simulating FL settings with minimal API .

- **[LEAF](https://github.com/TalwalkarLab/leaf)** — A Benchmark for Federated Settings (830 GitHub stars) .

- **[FedProx](https://github.com/litian96/FedProx)** — Federated Optimization in Heterogeneous Networks (MLSys '20) .

- **[Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter)** — Open-source library to audit data privacy in statistical and ML algorithms (581 GitHub stars) .

- **[Opacus](https://github.com/pytorch/opacus)** — Training PyTorch models with differential privacy (1,678 GitHub stars) .

- **[Google Differential Privacy](https://github.com/google/differential-privacy)** — The Python Differential Privacy Library (500 GitHub stars) .

- Community **n8n** workflows for federated training orchestration and model update routing.



**Frameworks for building custom systems**: Combine **Flower** for framework-agnostic federated orchestration with **FedML** for cross-cloud scheduling, **IBM FL** for homomorphic encryption-based secure aggregation, **Decentriq** for TEE-based exploratory computation, and **PostgreSQL** for persistence — creating a fully self-hosted, enterprise-grade federated learning infrastructure.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Federated learning systems handling sensitive data must comply with data protection regulations (GDPR, HIPAA, PIPL, etc.) and industry-specific requirements. **Privacy guarantees depend on the aggregation protocol** — standard FedAvg does not provide differential privacy or secure aggregation by default.

- **Federated learning and confidential computing are complementary, not competing.** FL excels at distributed model training where data stays local. TEE-based clean rooms (Decentriq) enable flexible exploratory computations — cohort discovery, record linkage, interactive queries — that FL cannot support . Production ecosystems often combine both.

- **Differential Privacy (DP), Secure Aggregation, and Homomorphic Encryption (HE) are the core privacy mechanisms** . Standard federated learning without these mechanisms is vulnerable to gradient leakage attacks. IBM FL provides HE support ; Opacus and Google DP provide DP primitives .

- **Open-source FL frameworks are mature for research and production.** Flower is the most widely adopted framework with 22+ baselines and framework-agnostic design . FedML provides cross-cloud scheduling with specialized domains (NLP, Graph NN, CV, IoT) . IBM FL provides enterprise-grade HE support .

- Self-hosted open-source solutions require proper security hardening, communication encryption, and ongoing maintenance. Federated learning introduces new attack surfaces — model poisoning, backdoor attacks, and inference attacks on aggregated updates — that require defensive measures beyond standard ML security.



---



**Made for ML engineers, healthcare researchers, financial institutions, and developers building transparent federated learning infrastructure.**

Let's make Federated Learning more open, data-driven, and privacy-preserving.
