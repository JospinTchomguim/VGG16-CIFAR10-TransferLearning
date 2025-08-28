# VGG16-CIFAR10-TransferLearning
# Transfer Learning with VGG16 on CIFAR-10 for image classification

This project implements **Transfer Learning** using the pre-trained **VGG-16** network (ImageNet weights, via Keras), applied to the **CIFAR-10** dataset.
The objective is to compare different adaptation strategies for the pre-trained model in order to evaluate their effectiveness on a relatively different dataset from ImageNet.

--

## 📌Objectives
- Exploit the **VGG-16** model provided by `keras.applications`.
- Implement three Transfer Learning strategies:
1. **Feature Extraction**: All layers of the pre-trained model are frozen and only the final classifier is trained.
2. **Partial Fine-tuning**: Only the last convolutional layers are retrained; the rest are frozen.
3. Total Fine-tuning: All network layers are thawed and retrained on CIFAR-10.
- Compare performance in terms of accuracy and loss on the validation set.

---

## 📂 Dataset
CIFAR-10: 60,000 images (32x32x3), divided into 10 classes (airplane, car, bird, cat, deer, dog, frog, horse, boat, truck). 
Loaded directly from Keras
