# 🧠 Convolutional Neural Networks with VGG16 – CIFAR-10 Image Classification

This project explores the power of **Convolutional Neural Networks (CNNs)** in image classification using the popular **CIFAR-10 dataset**. By leveraging **transfer learning** with the **VGG16 architecture**, we classify 60,000 color images (32×32 pixels) into 10 distinct categories.

## 🎯 Objectives

- Load and preprocess the CIFAR-10 dataset effectively.
- Fine-tune a **pretrained VGG16** model for CIFAR-10.
- Train and validate a robust CNN classifier.
- Visualize and evaluate the model’s performance.
- Analyze the contributions of convolutional vs. dense layers.

## 📦 Dataset

- **CIFAR-10**: 60,000 images (50,000 training + 10,000 testing)
- 10 categories: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

## 🧪 Preprocessing

- Pixel normalization (scaling to [0,1])
- Resize images to match **VGG16 input** shape (224x224)
- One-hot encoding of class labels

## 🧱 Model Architecture

- Base: **VGG16 pretrained on ImageNet**
- **Convolutional layers** optionally frozen to preserve learned features
- Custom **Fully Connected (FC)** layers added for CIFAR-10 classification

## 🏋️‍♀️ Training Configuration

- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Batch Size**: 32
- **Epochs**: 20+ (tunable)
- Real-time monitoring of accuracy and loss

## 📊 Evaluation

- Accuracy & Loss curves across epochs
- Confusion Matrix on test set
- Insightful discussion of **feature extraction vs classification**

## 🔬 Key Concepts

- CNNs extract hierarchical features: **edges → textures → shapes**
- FC layers serve as classifiers built on extracted features
- **Transfer learning** drastically boosts performance by reusing pretrained knowledge

---

> Course: *Artificial Intelligence*
> Instructor: Dr. YaghoobZadeh
> University of Tehran | School of Electrical & Computer Engineering