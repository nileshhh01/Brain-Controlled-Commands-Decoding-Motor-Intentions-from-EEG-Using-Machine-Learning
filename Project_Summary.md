# 🧠 Brain-Controlled Commands: Decoding Motor Intentions from EEG

##  Project Definition

This project aims to decode motor-related brain activity using EEG signals to classify imagined hand movements (e.g., left vs. right). The goal is to demonstrate the potential of Brain-Computer Interfaces (BCI) for controlling external systems using just brain signals.

##  Project Scope
Explore EEG signal processing and classification
Implement and compare traditional ML (CSP + SVM) with Deep Learning (EEGNet)
Demonstrate proof-of-concept for brain-driven command recognition
Lay the foundation for assistive technology using EEG

## Dataset
- Source: PhysioNet EEG Motor Movement/Imagery Dataset
- Type: Multi-subject EEG data (.edf format)
- Channels: 64 EEG electrodes
- Tasks: T1 = left hand, T2 = right hand motor imagery
  
##  Methodology
Data Loading & Preprocessing:
- Loaded raw .edf files using MNE
- Visualized signals and extracted motor-related epochs (T1 vs T2)
Feature Engineering:
- Applied Common Spatial Patterns (CSP) to extract spatial discriminative patterns
- Visualized spatial filters with topographic maps
Modeling:
- Classical ML: Logistic Regression, SVM trained on CSP features
- Deep Learning: Implemented EEGNet, a CNN architecture tailored for EEG
Evaluation:
- Accuracy, confusion matrix, and overfitting analysis

## Discussed challenges with generalization on limited data:
Technologies Used
- Python, JupyterLab
- Libraries: MNE, NumPy, scikit-learn, TensorFlow/Keras, Matplotlib
- GitHub for version control and collaboration
## Project Outcomes
- Successfully loaded and processed multi-channel EEG data
- Achieved ~60–70% accuracy using CSP + ML models
- Implemented EEGNet with moderate performance due to dataset size
- Built visualizations for CSP filters and EEG signal dynamics
- Created a modular project structure with clear documentation on GitHub
##  Real-World Impact

This project serves as a prototype for assistive technologies like prosthetic control, communication devices for paralyzed individuals, or hands-free UI systems. With larger datasets and training, this approach can evolve into real-time BCI applications.
