You’re right — **what’s in your repo now looks bad because the Markdown is broken**, not because the content is wrong.

The problems are:

* Sections merged together (no blank lines)
* Code blocks not closed
* Repository tree not in a fenced block
* Extra explanation text accidentally pasted into `README.md`
* Headings like *Training / Results / Datasets* missing `##`

Below is a **clean, minimal, GitHub-native README.md** that will **render correctly**, look **professional**, and is **concise**.
👉 **Delete your current README.md and replace it 100% with the text below.**

---

## ✅ **FINAL README.md (COPY–PASTE ONLY THIS)**

````md
# CSTLF

CNN–Semantic Transformer Learning Framework for fine-scale land-cover mapping
from multimodal remote sensing imagery under weak supervision.

---

## Overview

CSTLF is a CNN–Transformer hybrid deep learning framework for high-resolution
semantic segmentation of aerial, drone, and satellite imagery. It combines
convolutional neural networks for local spatial feature extraction with Vision
Transformers for global semantic context modeling.

The framework targets weakly supervised scenarios where high-resolution imagery
is paired with low-resolution or noisy annotations.

---

## Framework

<!-- Add framework figure here -->
<!-- Example: images/cstlf_framework.png -->

CSTLF adopts parallel CNN and Transformer branches followed by a contextual
semantic fusion module to produce fine-scale predictions.

---

## Features

- CNN–Transformer hybrid architecture  
- Weakly supervised learning  
- Multimodal remote sensing data  
- Pixel-level semantic segmentation  
- Reproducible experiments  

---

## Repository Structure

```text
CSTLF/
├── configs/        # Training configurations
├── datasets/       # Dataset loaders and preprocessing
├── models/         # CNN, Transformer, and fusion modules
├── losses/         # Segmentation and weak supervision losses
├── trainers/       # Training and evaluation pipelines
├── utils/          # Utilities and visualization
├── train.py
└── requirements.txt
````

---

## Installation

```bash
git clone https://github.com/BoazGithub/CSTLF.git
cd CSTLF
pip install -r requirements.txt
```

---

## Training

```bash
python train.py --config configs/cstlf.yaml
```

---

## Results

<!-- Add qualitative and quantitative results here -->

Evaluation metrics include Overall Accuracy (OA), mean IoU, and F1-score.

---

## Datasets

The framework supports high-resolution aerial, drone, and satellite datasets.
Due to licensing restrictions, datasets are not distributed. Dataset format
descriptions and preprocessing scripts are provided.

---

## Reproducibility

* Fixed random seeds
* Configuration-based experiments
* Consistent dataset splits

---

## Citation

If you use this repository, please cite:

```bibtex
@article{CSTLF2025,
  title   = {CSTLF: CNN–Semantic Transformer Learning Framework for Fine-Scale Land-Cover Mapping under Weak Supervision},
  author  = {Mwubahimana, Boaz and others},
  journal = {IEEE Transactions on Image Processing},
  year    = {2025}
}
```

---

## License

MIT License

---

## Contact

Boaz Mwubahimana
[https://github.com/BoazGithub](https://github.com/BoazGithub)
