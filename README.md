# Traffic Sign Classification Benchmark

A comparative study of classical and deep-learning methods for classifying German traffic signs (GTSRB), enhanced by image-preprocessing and ensemble techniques
using Python and TensorFlow.

---

## 📖 Project Overview

This repository explores how different machine-learning models and preprocessing pipelines impact traffic sign classification on the German Traffic Sign Recognition Benchmark (GTSRB) dataset:

1. **Classical Models**  
   - Multinomial Logistic Regression  
   - Support Vector Machine (RBF kernel)

2. **Deep Convolutional Networks**  
   - **AlexNet1**: Six-layer CNN with ReLU + Dropout  
   - **AlexNet2**: AlexNet1 + Batch Normalization

3. **Ensemble Method**  
   - Three “expert” CNNs trained on differently preprocessed images (original, bilateral filtered, gamma corrected)  
   - Meta-classifier (SVM or Logistic Regression) to fuse expert outputs

4. **Preprocessing & Feature Engineering**  
   - RGB images resized to 32×32  
   - Histogram of Oriented Gradients (HOG)  
   - Gamma correction, Gaussian/Median smoothing, bilateral filtering  
   - Dimensionality reduction: PCA & Mutual Information

5. **Data Augmentation**  
   - Minor rotations, translations, shear transforms to improve generalization

---

## ⚙️ Quick Start

1. **Clone the repository**  
   ```bash
   git clone https://github.com/Quancoder260503/gtsrb-classification.git
   cd gtsrb-classification

--
## Instruction

1. Run Sequentially: Execute the notebook from top to bottom without skipping cells to ensure correct initialization and reproducible outcomes.
2. Training Time: Model training may take up to 45 minutes, depending on your hardware configuration.
3. Hardware Recommendation: For best performance, run the notebook on a machine with GPU support, such as Google Colab, a CUDA-enabled local setup, or any other compatible environment.
4. File Paths: The default file paths reflect the directory structure used during Kaggle-based training. If you're running the notebook locally or in a different environment, make sure to update the file paths accordingly to match your folder setup.
