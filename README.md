# Hi, I'm Juan D. Castro, Ph.D.
**Sr. Staff Applications Engineer @ Synopsys (formerly Ansys)**<br>
Deep Learning for Radar Perception · RF/Microwave Systems · AI-Driven Simulation

<p align="left">
  <a href="https://www.linkedin.com/in/juanddcastro"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://orcid.org/0000-0002-6817-7211"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"></a>
  <a href="mailto:juand.castro@synopsys.com"><img src="https://img.shields.io/badge/Email-6E4AA6?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://komarev.com/ghpvc/?username=ansjuandcastro&style=for-the-badge&color=6E4AA6" alt="Profile views">
</p>

---

## About Me
Sr. Staff Applications Engineer at Synopsys, spanning **RF/microwave simulation
and applied machine learning** for commercial customers. I build **CNN-based
detection models** on synthetic radar imagery with physics-informed data
pipelines, and ship deployable inference tools — working end to end from signal
processing to multi-GPU training to deployment.

---

## Highlight: Project LOCH NESS — Synthetic SAR Target Detection

An applied deep-learning project: end-to-end target detection on synthetic radar
Range-Doppler imagery (STK RF Channel Modeler), from raw radar data to a portable
evaluation tool.

**Built**
- Full pipeline: `.rsp` extraction → programmatic labeling → YOLOv8 training →
  held-out-elevation OOD evaluation (no train/val leakage into the test split).
- Multiple training runs across resolution, augmentation, capacity, and
  regularization, with observability-filtered labels under active evaluation as
  a label-quality extension.
- 4× NVIDIA Tesla M60 distributed training; H100 cluster for higher-resolution
  scaling experiments.

**Demonstrated**
- Best OOD result (Phase 9, Run A): **mAP@0.5 = 0.487** at 1024×1024 — a **+54%
  relative gain** over the 0.317 Phase 8 512×512 baseline. Per-class mAP@0.5:
  large aircraft 0.98, small aircraft 0.74, fire truck 0.40, helicopter 0.30,
  pickup truck 0.02 — strong on large aircraft, hardest on small,
  low-observability targets like pickups.
- Follow-on augmentation and higher-resolution runs did not beat that baseline,
  suggesting dataset breadth and label fidelity may matter more than model or
  resolution changes in this small-data OOD setting.

**Evaluation tooling**
- Portable local inference GUI (Gradio + conda-pack) that converts `.rsp` radar
  files to model-ready imagery and runs detector inference with annotated
  outputs, CSV export, and reproducible run artifacts.

---

## Currently
- Scaling the synthetic-SAR pipeline to larger data lakes and multi-material scenes.
- Cross-scene OOD generalization (leave-one-out evaluation).
- Agentic AI workflows: a coder/auditor reflection loop applied to tool hardening, review, and release-readiness artifacts.
- Exploring ML surrogates for RF channel and antenna modeling.

---

## Talks & Publications
- **Synopsys Converge / SNUG 2026** (Simulation World, Silicon Valley) —
  *Data-Centric Supervision Strategies for Deep Learning Object Detection in
  Complex Synthetic SAR Scenes*. [Session](https://events.synopsys.com/event/converge2026/agenda?session=3b69d15e-e8e2-47b8-9dfa-903450f03a68&shareLink=true)

---

## Focus Areas
- **Deep Learning** — CNN detection, YOLO family, OOD generalization, data-centric AI.
- **Radar & RF** — synthetic SAR, Range-Doppler processing, antenna design, 5G/6G.
- **Deployment** — model packaging, portable inference tools, reproducible pipelines.
- **Simulation** — physics-based synthetic data, ML surrogates, cloud-native HPC.

---

## Tech Stack
- **DL/ML:**  
  ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
  ![YOLOv8](https://img.shields.io/badge/Ultralytics%20YOLOv8-6E4AA6?style=flat)
  ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
  ![Keras](https://img.shields.io/badge/Keras-D00000?style=flat&logo=keras&logoColor=white)
  ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
  ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
  ![Gradio](https://img.shields.io/badge/Gradio-FF4B4B?style=flat&logo=gradio&logoColor=white)
  ![LLMs](https://img.shields.io/badge/LLMs-6E4AA6?style=flat)

- **Simulation:**  
  ![STK](https://img.shields.io/badge/STK-6E4AA6?style=flat)
  ![RF Channel Modeler](https://img.shields.io/badge/RF%20Channel%20Modeler-6E4AA6?style=flat)
  ![HFSS](https://img.shields.io/badge/HFSS-6E4AA6?style=flat)
  ![AEDT](https://img.shields.io/badge/AEDT-6E4AA6?style=flat)

- **Infra:**  
  ![NVIDIA](https://img.shields.io/badge/NVIDIA_M60%20%2F%20H100-76B900?style=flat&logo=nvidia&logoColor=white)
  ![Multi-GPU](https://img.shields.io/badge/Multi--GPU%20Training-6E4AA6?style=flat)
  ![Slurm](https://img.shields.io/badge/Slurm-6E4AA6?style=flat)
  ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)
  ![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)

- **Languages:**  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
  ![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)
  ![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat)

---

## Connect
- [juand.castro@synopsys.com](mailto:juand.castro@synopsys.com)
- [LinkedIn](https://www.linkedin.com/in/juanddcastro)
- [ORCID](https://orcid.org/0000-0002-6817-7211)

---

## GitHub Activity
<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=ansjuandcastro&show_icons=true&hide_border=true&title_color=6E4AA6&icon_color=6E4AA6" height="160" alt="GitHub stats">
  <img src="https://streak-stats.demolab.com/?user=ansjuandcastro&hide_border=true&ring=6E4AA6&fire=6E4AA6&currStreakLabel=6E4AA6" height="160" alt="GitHub streak stats">
</p>

---

> "From RF signals to radar intelligence — bridging physics and deep learning."
