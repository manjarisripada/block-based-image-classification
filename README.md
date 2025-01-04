# Image Classification with MobileNet CNN and Decision Tree

## Project Overview
This project focuses on classifying natural landscape images into one of five categories: `grass`, `sky`, `plant`, `mountain`, and `waterbody`. The process involves feature extraction using MobileNet, a pre-trained convolutional neural network (CNN), followed by classification using a Decision Tree.

The images are further subdivided into grids for detailed block-wise classification. Two grid configurations are explored: 2x2 (4 blocks) and 3x3 (9 blocks). The final classification for an image is determined using majority voting based on the predictions for its blocks.

---

## Features
1. **Feature Extraction**: 
   - MobileNet CNN is used to extract features from the images.
   - Features are saved after processing each category to handle potential interruptions.

2. **Classification**: 
   - A Decision Tree classifier is trained on the extracted features using an 80/20 train-test split.

3. **Block-wise Classification**: 
   - Images are divided into grids (2x2 and 3x3).
   - Each block is classified, and the majority vote determines the final classification.

4. **Accuracy Reporting**: 
   - Classification accuracy is calculated for both grid configurations.

---

## Requirements
- Python 3.8+
- Jupyter Notebook or Google Colab
- Libraries:
  - TensorFlow
  - NumPy
  - scikit-learn
  - Matplotlib
