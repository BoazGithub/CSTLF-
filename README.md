# <h1 align="center">  <b>CSTLF: Cross-Spatio-Temporal Learning Framework for Weakly Supervised Remote Sensing Change Detection </b>



</h1>

<h2 align="left">Authors 



</h2>

## Updates

| :zap:          | January, 2026: CSTLF Framework has been finalized for publication in IEEE Transactions on Geoscience and Remote Sensing. |
| --- | --- |


This study introduces the **Cross-Spatio-Temporal Learning Framework (CSTLF)**, a unified architecture for autonomous land-cover change detection. To address the limitations of bi-temporal snapshots and annotation bottlenecks, CSTLF harmonizes **CNN-based spatial primitives**, **LSTM-based sequential state propagation**, and **Transformer-driven global attention**. By leveraging weakly supervised pseudo-labels from low-resolution products (GLC10), the model achieves high-fidelity change mapping. CSTLF Model and the **sKwanda_v1** (Nyagatare, Kigali, Chesapeake Bay) datasets can be downloaded [[here](https://github.com/BoazGithub/CSTLF)].
 

## Graphical abstract: 

Graphical abstract illustrating the synergistic multi-scale and multi-temporal feature extraction within the CSTLF architecture. It highlights the integration of CNN, LSTM, and Transformer branches to resolve spatial heterogeneity and temporal dependencies in high-resolution imagery.

# Requirements:

## Description:

###  Study Area:
The Cross-Spatio-Temporal Learning Framework (CSTLF) was rigorously trained and validated over the Nyagatare agricultural district and the Kigali urban corridor. Migration testing was conducted on the Chesapeake Bay Land Cover dataset to evaluate global generalization and multi-temporal robustness.

###  Study Area Data descriptions:
| Image Ref. |      Site     | Image Acquisition Date  |   GT Date   |
| ---------- | ------------- | ----------- | ------------ | 
|   Img (1)  |   Kigali City   |  2020 -- 2024 |  2024-05-15 |
|   Img (2)  |   Nyagatare    |  2021 -- 2023 |  2023-11-20 |  
|   Img (3)  |   Chesapeake Bay |  2022 -- 2024 |  2024-01-10 |  

# CSTLF Architecture

The CSTLF architecture integrates three core components: the **Multi-Scale Feature Fusion Network (MSFFN)** for hierarchical representation, the **Dual-branch Temporal-Spatial Attention Mechanism (DbTSAM)** for dynamic dependency modeling, and the **Weakly Supervised Pseudo-Label Refinement (WS-PLR)** module. These components utilize cross-attention and residual learning to suppress stochastic noise while preserving sharp transition boundaries in heterogeneous landscapes.

### Algorithm flows:

1.

### CSTLF network workflows:

2.

# Results:

##### Tracking training progress:

Monitoring convergence across mIoU, OA, and Kappa metrics. The tri-branch fusion ensures a stable decline in loss while maximizing the F1-Score across both urban and agricultural classes.

#### Feature Pattern Recognition:

Visualization of the feature flow showing how MSFFN and DbTSAM improve pattern recognition for multiscale global and local dependencies.

# Quantitative Results:

# Qualitative Results:

## SoA (State-of-the-Art)

1.

2.

### 🔭 Baseline:

📖 📖 📖 

* :open_book: BIT (Bitemporal Image Transformer) [[here](https://www.google.com/search?q=https://ieeexplore.ieee.org/abstract/document/9491701)]
* :open_book: SNUNet-CD [[here](https://www.google.com/search?q=https://ieeexplore.ieee.org/document/9623290)]
* :open_book: ChangeFormer [[here](https://arxiv.org/abs/2201.01293)]
* :open_book: FC-Siam-diff [[here](https://arxiv.org/abs/1810.08462)]
* :open_book: STANet [[here](https://www.mdpi.com/2072-4292/12/10/1662)]
📖 📖 📖

💬 Dataset Preparation

### sKwanda_v1 Dataset Overview

The **sKwanda_v1** dataset consists of 512 × 512 pixel bi-temporal patches. It features high-resolution (0.5m) imagery paired with weakly supervised labels. The dataset supports multi-class change detection including built-up areas, forests, water, and arable land.

### Dataset Structure

```python
# CSTLF Dataset Loader Structure
- data/
  - train/
    - T1/ (Pre-change images)
    - T2/ (Post-change images)
    - label/ (Pseudo-labels)
  - val/
  - test/

```

### 🔭 Contact Information:

If you have any questions or would like to collaborate, please reach out to **aiboaz1896@gmail.com** or open an issue in the repository.

### License: 

The code and datasets are released for non-commercial and research purposes only.

### Acknowledgment:

This work was supported by the **Planetary Science group** at the State Key Laboratory of Information Engineering in Surveying, Mapping and Remote Sensing (LIESMARS), **Wuhan University**.

---

**Next Step:** Would you like me to create the BibTeX citation for this new CSTLF model so you can include it in the README?


