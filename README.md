# 🧠 Brain-Controlled Commands: Decoding Motor Intentions from EEG

This project explores the use of machine learning and deep learning to decode motor-related brain activity from EEG signals.

---

## 📌 Project Goal

To classify imagined motor tasks (like left-hand vs right-hand movement) using EEG recordings and recognize brain-driven commands — a key step toward Brain-Computer Interfaces (BCI).

---

## 🔬 Dataset

- **Source:** [EEG Motor Movement/Imagery Dataset – PhysioNet](https://physionet.org/content/eegmmidb/1.0.0/)
- **Data Format:** `.edf` (64-channel EEG recordings)
- **Subjects:** Performing or imagining motor tasks (T1 = left hand, T2 = right hand)

---

## 🧪 What We Did

### ✅ 1. EEG Preprocessing & Visualization
- Loaded EEG `.edf` files using MNE
- Extracted events and plotted signal segments
- Visualized annotations (T1, T2) and time series

### ✅ 2. Common Spatial Patterns (CSP)
- Applied CSP for spatial feature extraction
- Visualized topographic patterns for motor task discrimination
- Trained classical ML models (LogReg, SVM)

### ✅ 3. Deep Learning with EEGNet
- Implemented EEGNet CNN architecture
- Trained model on small dataset (limited generalization)
- Plotted training/validation accuracy & loss

---

## ⚠️ Challenges Faced

- Missing electrode coordinates → fixed using standard montages
- Small dataset → EEGNet tended to overfit
- Class imbalance in predictions → accuracy was misleading

---

## 📁 Folder Structure
📁 Brain-Controlled-Commands-Decoding-Motor-Intentions-from-EEG-Using-Machine-Learning 
-  ├── notebooks/ # Jupyter notebooks (Preprocessing, CSP, EEGNet) │ 
-  ├── EEG_Preprocessing_and_Visualization.ipynb │ 
-  ├── CSP_and_Channel_Analysis.ipynb │ 
-     └── EEGNet_Deep_Learning_Model.ipynb │ 
-  ├── data/ # Raw EDF EEG files │ 
    └── s001r04.edf, ... │ 
-  ├── scripts/ # Python scripts (future expansion) │ 
-  ├── models/ # Saved models (if any) │ 
-  ├── figures/ # CSP filters, EEG signal plots, etc. │ 
-  ├── requirements.txt # All required Python packages 
-     └── README.md

## 📊 Next Steps

- Expand dataset using more subjects
- Add data augmentation (noise, channel flipping)
- Improve EEGNet generalization with cross-validation

---

## ✨ Credits

- Dataset: PhysioNet EEG Motor Imagery
- Deep learning: EEGNet by Lawhern et al. (2018)

