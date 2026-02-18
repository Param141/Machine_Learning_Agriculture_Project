

# Machine Learning for Ridge Gourd Classification 🌱

## Overview
This project focuses on applying **machine learning and deep learning techniques** to classify ridge gourd images. The dataset was **self-created and preprocessed** to ensure quality and consistency, followed by training with multiple models to benchmark performance. This Project Resulted in an Conference Paper Presented at MIND 2025 conference.

## Key Features
- 📸 **Custom Dataset**: Ridge gourd images collected and curated manually.  
- 🧹 **Preprocessing**: Image resizing, normalization, and augmentation for robust training.  
- 🤖 **Model Training**: Implemented and compared multiple ML/DL models including:
  - Convolutional Neural Networks (CNNs)
  - Hybrid CNN architectures
  - MobileNet & MobileNetV2
  - Custom CNN variants
  - SVM + CNN combinations  
- 📊 **Performance Evaluation**: Accuracy and loss metrics tracked across models.

## Repository Structure
```
├── .gitattributes
├── Normal_CNN.py                # Standard CNN implementation
├── hybridcnn(dn121).py          # Hybrid CNN with DenseNet121
├── customcnn.py                 # Custom CNN architecture
├── copy_of_mobilenet.py         # MobileNet model
├── copy_of_mobilenetv2_softmax.py # MobileNetV2 with softmax
├── svm+cnn.py                   # SVM combined with CNN
```

## Future Work
- Expanding dataset with more agricultural crops.  
- Hyperparameter tuning for improved accuracy.  
- Deployment of trained models for real-world agricultural applications.  

## About
This project demonstrates the potential of **AI in agriculture**, specifically in crop classification and recognition tasks. By building a dataset from scratch and experimenting with diverse models, it showcases end-to-end workflow from **data collection → preprocessing → training → evaluation**.



