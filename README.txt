# Traffic Sign Classification Benchmark

A comparative study of classical and deep-learning methods for classifying German traffic signs (GTSRB), enhanced by image-preprocessing and ensemble techniques.

---

## 📖 Project Overview

This repository explores how different machine-learning models and preprocessing pipelines impact traffic sign classification on the German Traffic Sign Recognition Benchmark (GTSRB) dataset:

1. **Classical Models**  
   - Multinomial Logistic Regression  
   - Support Vector Machine (RBF kernel)

2. **Deep Convolutional Networks**  
   - **AlexNet1**: Six-layer CNN with ReLU + Dropout  
   - **AlexNet2**: AlexNet1 + Batch Normalization
   - Details about the architecture in the report

3. **Ensemble Method**  
   - Three “expert” CNNs trained on differently preprocessed images (original, bilateral filtered, gamma corrected)  
   - Meta-classifier (SVM or Logistic Regression) to fuse expert outputs

4. **Preprocessing & Feature Engineering**  
   - RGB images resized to 32×32  
   - Histogram of Oriented Gradients (HOG)  
   - Gamma correction, Gaussian/Median smoothing, bilateral filtering  
   - Dimensionality reduction: PCA & Mutual Information  

5. **Data Augmentation**  
   - Minor rotations, translations, shear transforms  
   - Improves generalization and combats overfitting

---

## ⚙️ Quick Start

1. **Clone the repository**  
   ```bash
   git clone https://github.com/<your-username>/gtsrb-classification.git
   cd gtsrb-classification
