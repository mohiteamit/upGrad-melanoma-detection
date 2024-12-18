# upGrad - Skin Lesion Classification Using Convolutional Neural Networks

This project classifies various types of skin lesions using Convolutional Neural Networks (CNNs). It addresses challenges such as class imbalance and overfitting by employing data augmentation, dropout layers, and sample balancing techniques.

---

## Table of Contents
1. [Dataset](#dataset)
2. [Class Distribution](#class-distribution)
3. [Model Architecture](#model-architecture)
4. [Data Augmentation and Handling Imbalance](#data-augmentation-and-handling-imbalance)
5. [Conclusion](#conclusion)

---

## Dataset

The dataset consists of images of skin lesions categorized into nine classes:
- **Actinic Keratosis**
- **Basal Cell Carcinoma**
- **Dermatofibroma**
- **Melanoma**
- **Nevus**
- **Pigmented Benign Keratosis**
- **Seborrheic Keratosis**
- **Squamous Cell Carcinoma**
- **Vascular Lesion**

The dataset is highly imbalanced, requiring special handling to ensure fair representation of all classes.

---

## Class Distribution

The class distribution in the training dataset is as follows:

![Class Imbalance](readme-images/Class%20imbalance.png)

---

## Model Architecture

### ModelA: Initial Baseline Model
- A simple CNN with basic convolutional and pooling layers.
- Suffered from overfitting and limited generalization.

![ModelA Architecture](readme-images/ModelA.png)  
![ModelA Summary](readme-images/ModelA-summary.png)

---

### ModelB: Improved with Data Augmentation and Dropout
- Introduced data augmentation to diversify the training data.
- Added dropout layers to mitigate overfitting.

![ModelB Architecture](readme-images/ModelB.png)  
![ModelB Summary](readme-images/ModelB-summary.png)

---

### ModelC: Final Model with Augmented + Original Data
- Balanced the dataset using additional augmented samples.
- Retained data augmentation and dropout layers from ModelB.

![ModelC Architecture](readme-images/ModelC.png)  
![ModelC Summary](readme-images/ModelC-summary.png)

---

## Data Augmentation and Handling Imbalance

1. **Data Augmentation**:
   - Applied transformations like flips, rotations, and brightness adjustments to increase data variability.

2. **Class Balancing**:
   - Used additional augmented samples to balance underrepresented classes.

---

## Conclusion

This project highlights the challenges of classifying imbalanced datasets and the importance of techniques like augmentation and dropout to improve model generalization. The final model demonstrates better handling of class imbalance but still faces challenges with underrepresented and visually similar classes.

## Author

**Amit Mohite**  

This project is assignment of `Master of Science in Artificial Intelligence and Machine Learning` from Liverpool John Moores University and International Institute of Information Technology, Bangalore.