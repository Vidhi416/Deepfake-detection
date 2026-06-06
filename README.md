# DeepFake Detection Using CNN-ViT Fusion Model

## Overview

Deepfakes have become increasingly sophisticated, making it difficult to distinguish manipulated media from authentic content. This project presents a hybrid DeepFake Detection system that combines the strengths of Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs) to improve detection accuracy.

The CNN component captures local spatial features such as texture inconsistencies and facial artifacts, while the Vision Transformer learns global contextual relationships across the image. By fusing features from both architectures, the model achieves robust performance in identifying manipulated facial images.

---

## Features

* Hybrid CNN + Vision Transformer architecture
* Feature fusion for enhanced representation learning
* Binary classification: Real vs DeepFake
* Image preprocessing and augmentation pipeline
* Model evaluation using multiple performance metrics
* Modular and scalable implementation

---

## Architecture

Input Image
↓
CNN Feature Extractor
↓
Feature Fusion Layer ← Vision Transformer Encoder
↓
Fully Connected Layers
↓
Real / Fake Prediction

### Why CNN + ViT?

* CNNs excel at capturing local patterns and image artifacts.
* Vision Transformers capture long-range dependencies and global context.
* Feature fusion leverages the strengths of both models for improved DeepFake detection.

---

## Dataset

The model was trained and evaluated on publicly available DeepFake datasets containing real and manipulated facial images.

Typical preprocessing steps include:

* Face extraction and alignment
* Image resizing
* Normalization
* Data augmentation

---

## Tech Stack

* Python
* PyTorch
* OpenCV
* NumPy
* Scikit-learn
* Matplotlib

---

## Project Structure

```text
DeepFake-Detection/
│
├── dataset/
├── models/
│   ├── cnn_model.py
│   ├── vit_model.py
│   └── fusion_model.py
│
├── training/
│   └── train.py
│
├── evaluation/
│   └── evaluate.py
│
├── utils/
│   └── preprocessing.py
│
├── requirements.txt
└── README.md
```

## Installation

```bash
git clone https://github.com/your-username/deepfake-detection.git

cd deepfake-detection

pip install -r requirements.txt
```

## Training

```bash
python train.py
```

## Evaluation

```bash
python evaluate.py
```

## Results

The CNN-ViT fusion model demonstrated strong performance in distinguishing real and manipulated facial images.

Evaluation Metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

> Replace this section with your actual experimental results and screenshots.

---

## Future Improvements

* Real-time video DeepFake detection
* Multi-class manipulation detection
* Attention visualization for explainability
* Deployment as a web application
* Model optimization for edge devices

---

## Applications

* Social media content verification
* Digital forensics
* Media authenticity validation
* Cybersecurity and misinformation detection

---

## Contributors

Vidhi Agrawal

---

## License

This project is intended for educational and research purposes.
