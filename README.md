[![arXiv](https://img.shields.io/badge/arXiv-2501.XXXXX-b31b1b.svg)](https://arxiv.org/abs/2501.XXXXX)
[![ORCID](https://img.shields.io/badge/ORCID-0000--0002--3900--7184-green.svg)](https://orcid.org/0000-0002-3900-7184)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-ee4c2c.svg)](https://pytorch.org/)

# GraViT: Transfer Learning with Vision Transformers and MLP-Mixer for Strong Gravitational Lens Discovery
> ## René Parlange, Juan C. Cuevas-Tello, Octavio Valenzuela, Omar de J. Cabrera-Rosas, Tomás Verdugo, Anupreeta More, Anton T. Jaelani
> #### 📘 [arXiv pre-print](https://arxiv.org/)

## Systematic comparison of neural networks used in discovering strong gravitational lenses
> ### Anupreeta More, Raoul Canameras, Anton T. Jaelani, Yiping Shu, Yuichiro Ishida, Kenneth C. Wong, Kaiki Taro Inoue, Stefan Schuldt, Alessandro Sonnenfeld
> #### 📘 [Monthly Notices of the Royal Astronomical Society (MNRAS)](https://academic.oup.com/mnras/article/533/1/525/7700722)

---
### 🌌 Dataset: HOLISMOKES VI (Cañameras et al., 2021) (C21) 
> ### 🔗 [Astronomy & Astrophysics (A&A)](https://www.aanda.org/articles/aa/abs/2021/09/aa41758-21/aa41758-21.html)
> #### Training: 40,000 mocklenses and 40,000 non-lenses. Validation: 500 of each class.
> #### Hyper Suprime-Cam (HSC) _gri_ bands and Hubble Ultra Deep Field (HUDF) ACS and WFC3 bands


### 🌌 Dataset: SuGOHI X (Jaelani et al., 2024)(J24)
> ### 🔗 [Monthly Notices of the Royal Astronomical Society (MNRAS)](https://academic.oup.com/mnras/article/535/2/1625/7842018)
> #### 18,660 lenses and 18,660 non-lens objects
> #### Hyper Suprime-Cam (HSC) _gri_ bands
> #### No validation dataset (partitioned 95% for training and 5% for validation)  

---

## 🧪 Experiments

### HOLISMOKES VI (C21)
| Notebook | Description |
|----------|-------------|
| [a1-C21-classification-head.ipynb](experiments/a1-C21-classification-head.ipynb) | Fine-tune only the classification head |
| [a2-C21-half.ipynb](experiments/a2-C21-half.ipynb) | Fine-tune half of the layers |
| [a3-C21-all-blocks+ResNet18.ipynb](experiments/a3-C21-all-blocks+ResNet18.ipynb) | Train all layers + ResNet18 |


### SuGOHI X (J24)
| Notebook | Description |
|----------|-------------|
| [b1-J24-classification-head.ipynb](experiments/b1-J24-classification-head.ipynb) | Fine-tune only the classification head |
| [b2-J24-half.ipynb](experiments/b2-J24-half.ipynb) | Fine-tune half of the layers |
| [b3-J24-all-blocks.ipynb](experiments/b3-J24-all-blocks.ipynb) | Train all layers |


### Combined (C21 + J24)
| Notebook | Description |
|----------|-------------|
| [c1-C21+J24-classification-head.ipynb](experiments/c1-C21+J24-classification-head.ipynb) | Fine-tune only the classification head |
| [c2-C21+J24-half.ipynb](experiments/c2-C21+J24-half.ipynb) | Fine-tune half of the layers |
| [c3-C21+J24-all-blocks+ResNet18.ipynb](experiments/c3-C21+J24-all-blocks+ResNet18.ipynb) | Train all transformer blocks + ResNet18 |


### Subsampled C21 (18,660 samples)
| Notebook | Description |
|----------|-------------|
| [s1-C21-18660-classification-head.ipynb](experiments/s1-C21-18660-classification-head.ipynb) | Fine-tune only the classification head |
| [s2-C21-18660-half.ipynb](experiments/s2-C21-18660-half.ipynb) | Fine-tune half of the layers |
| [s3-C21-18660-all-blocks+ResNet18.ipynb](experiments/s3-C21-18660-all-blocks+ResNet18.ipynb) | Train all layers + ResNet18 |


### Inference
| Notebook | Description |
|----------|-------------|
| [L2-inference.ipynb](experiments/L2-inference.ipynb) | Recall for search in L2 subset (138 lenses) |


