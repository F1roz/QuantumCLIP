# Quantum CLIP: Contrastive Language-Image Pretraining with Quantum Visual Encoder

This repository contains a reimplementation of **CLIP (Contrastive Language–Image Pre-training)** where the **Visual Encoder** is replaced with **Quantum Circuits**, and the **Text Encoder** is a pre-trained **BERT** model. The quantum visual encoder is wrapped with a PyTorch layer, enabling seamless hybrid classical-quantum training and fine-tuning.

---

## 🚀 Overview

This project explores the fusion of **Quantum Machine Learning** with **Multimodal Contrastive Learning**. Inspired by OpenAI's CLIP model, we propose a hybrid approach that incorporates **Quantum Circuits** as the image encoder to investigate the potential of quantum representations in aligning visual and textual modalities.

---

## 🧩 Architecture

- **Text Encoder**: Pretrained `BERT` model from HuggingFace
- **Visual Encoder**: Custom **Quantum Circuit** built with `PennyLane` and wrapped using `TorchLayer` for PyTorch compatibility
- **Projection Heads**: Linear layers to project both modalities into a joint embedding space
- **Loss Function**: Symmetric Contrastive Loss (CLIP-style InfoNCE)
- **Hyperparameter Tuning**: Includes grid/random search for learning rate, batch size, and circuit depth

---

## 🛠️ Features

- ✅ Quantum Visual Encoder via PennyLane and PyTorch integration  
- ✅ BERT-based Text Encoder  
- ✅ CLIP-style contrastive training  
- ✅ End-to-end fine-tuning  
- ✅ Modular code for easy experimentation  
- ✅ Hyperparameter tuning utilities  

---

## 🧪 Datasets

- **MEDMNIST**, or any custom image-text dataset
- Images are resized and normalized
- Text is tokenized using `BERTTokenizer`

---

## ⚙️ Installation

```bash
git clone https://github.com/F1roz/QuantumCLIP
cd QuantumCLIP
pip install -r requirements.txt
```

### Main dependencies

- `torch`
- `transformers`
- `pennylane`
- `scikit-learn`
- `matplotlib`
- `wandb` *(optional, for logging)*

---


## 📈 Results & Evaluation

- Evaluation is based on image-text retrieval accuracy (Recall@K)
- Embedding visualizations using t-SNE
- Includes comparison between classical and quantum visual encoders

---

## 🌌 Research Directions

This project is part of ongoing research into:

- 🌐 **Hybrid Quantum-Classical Feature Fusion**
- 🔗 **Quantum-Inspired Contrastive Learning**
- 🧠 Enhancing **multimodal representation learning** using quantum state expressivity

---

## 📜 Citation

If this repo helps in your research or learning, please consider citing:

```
@misc{quantumclip2025,
  author = {SM Firoz Ahmed Fahim},
  title = {Quantum CLIP: Multimodal Representation Learning with Quantum Visual Encoding},
  year = {2025},
  url = {https://github.com/F1roz/QuantumCLIP}
}
```

---

## 📬 Contact

For collaboration, questions, or discussions:

📧 firozfahim@n3xchain.com  
📘 [LinkedIn](https://linkedin.com/in/firozfahim)  
🐦 [Twitter](https://twitter.com/firozfahimm)

---
