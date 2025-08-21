# GNNFingers Reproduction

This repository contains a reproduction of the paper:

> [You et al. (2024). "GNNFingers: A Fingerprinting Framework for Verifying the Ownership of Graph Neural Networks"](https://doi.org/10.1145/3589334.3645489)

---

## Overview
The reproduction includes the following from the paper:

- Train a **target GNN model** (GCN/GraphSAGE).  
- Generate **suspect models** (fine-tuned, partially retrained, independent).  
- Learn **fingerprints** to query and test models.  
- Train a **Univerifier classifier** to verify ownership.  
- Evaluate with **Robustness, Uniqueness, Accuracy, ARUC, and ROC-AUC**.

---
## Packages and pip installs

```
!pip install torch torch-scatter torch-sparse torch-cluster torch-spline-conv torch-geometric -f https://data.pyg.org/whl/torch-2.2.0+cu118.html 
```

---

## Results

<img width="536" height="393" alt="verification_curve" src="https://github.com/user-attachments/assets/3e243335-effd-44f6-99f2-e2ce46049e37" />
<img width="536" height="393" alt="ROC_Curve" src="https://github.com/user-attachments/assets/a3ced47a-2152-421a-901b-6b038a1e6273" />

ARUC: 0.99

ROC-AUC: 1.0

Mean test accuracy: 0.9900990099009901

---

## Acknowledgments

Under the supervision of [Dr. Yushun Dong](https://yushundong.github.io) and [Mr. Bolin Shen](https://blshen.org)

This project utilized text/code generated with the assistance of OpenAI's ChatGPT-3.5 (Nov 30 version, 2022). (Helped whenever I ran into bugs or issues)

---
