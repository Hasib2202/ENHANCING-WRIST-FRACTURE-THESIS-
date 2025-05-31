

# Wrist Fracture Detection using Deep Learning – WristNet 🩺🤖

## 📘 Project Title
**Enhancing Wrist Fracture Detection in Wrist X-Ray Images Using Deep Learning Models**

---

## 🧠 Overview

Wrist fractures are among the most common orthopedic injuries, especially from falls. Traditional X-ray interpretation can be error-prone due to human limitations and overlapping anatomy.

This project presents **WristNet**, a deep learning-based solution designed to assist in early and accurate detection of wrist fractures using X-ray images.

---

## 🎯 Objectives & Goals

- **Objective:** Improve fracture detection accuracy using feature concatenation across top-performing CNN models.
- **Goal:** Develop a clinically viable, robust AI tool to support radiologists.

---

## ❓ Problem Statement

- Limited labeled wrist X-ray datasets.
- Diagnostic challenges due to complex wrist anatomy.
- Need for a lightweight, accurate model for small-data scenarios.

---

## 🧪 Methodology

1. **Dataset**
   - 193 wrist X-rays (111 fractures, 82 normal)
   - Augmentation: Flipping, rotation, contrast adjustment

2. **Models Used**
   - EfficientNetB2
   - DenseNet169
   - InceptionV3
   - Xception
   - NASNetMobile

3. **Feature Concatenation**
   - Combined DenseNet169 and InceptionV3
   - Final fused model named **WristNet**

4. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-score
   - Technique: Cross-validation & Hyperparameter tuning

---

## 🧱 WristNet Architecture

![WristNet Architecture](screenshots/architecture.png)  
*A combination of DenseNet169 and InceptionV3 feature maps*

---

## 📊 Results

| Model        | Accuracy | Precision | Recall | F1-Score |
|--------------|----------|-----------|--------|----------|
| WristNet     | **97.5%** | Improved  | Improved | Improved |
| LSNet (baseline) | 86.5%    | Lower    | Lower  | Lower    |

📈 **Loss Curve of WristNet**
![Loss Curve](screenshots/loss_curve.png)

🖼️ **Prediction Samples**
![Predictions](screenshots/predictions.png)

---

## 🔬 Key Contributions

- Designed a novel deep learning model, **WristNet**, for small medical datasets.
- Achieved **97.5%** accuracy — **+11%** improvement over LSNet.
- Demonstrated the effectiveness of **feature-level fusion** over ensemble methods.

---

## 🔮 Future Work

- Expand dataset with diverse X-ray samples.
- Explore newer architectures for better performance.
- Deploy real-time clinical versions.
- Build GUI for radiologists.

---

## 📚 References

- [DeepLOC](https://paperswithcode.com/paper/deeploc-deep-learning-based-bone-pathology)
- [PubMed Fracture Detection](https://pubmed.ncbi.nlm.nih.gov/33937780/)
- [MDPI Fracture Detection](https://www.mdpi.com/1424-8220/22/3/1285)
- Additional citations in `references.bib`

---

## 📁 Repository Structure

```

📂 wrist-fracture-detection/
├── 📁 models/                # Model architectures
├── 📁 data/                  # X-ray images
├── 📁 notebooks/             # Training and analysis notebooks
├── 📁 utils/                 # Helper functions
├── 📁 screenshots/           # Result screenshots (add loss\_curve.png, predictions.png, etc.)
├── 📄 README.md              # This file
├── 📄 requirements.txt       # Python dependencies
└── 📄 wristnet.py            # Final WristNet model

````

---

## 🚀 How to Run

```bash
git clone https://github.com/your-username/wrist-fracture-detection.git
cd wrist-fracture-detection
pip install -r requirements.txt
python wristnet.py
````

---

## 🙌 Acknowledgments

This work is part of the **Undergraduate Thesis** submitted to the **Department of Computer Science, Faculty of Science and Technology**.

---

## 📸 Screenshots

![Image](https://github.com/user-attachments/assets/3fd68c9f-2753-425d-9456-a355325b0735)

---

## 📬 Contact

For queries, contact **\[Md. Mostofa Hasib]** at \[(hasibammostofahasib@gmail.com)].



