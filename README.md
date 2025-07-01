#  Medical Image Classification using Deep Learning

This repository presents two deep learning projects focused on the classification of medical images using public datasets: **RetinaMNIST** and **ChestMNIST**. These projects explore different disease detection tasks using convolutional neural networks (CNNs), data augmentation, and performance evaluation techniques.

---

# Projects

### 1.  RetinaMNIST – Retinal Disease Classification

**Objective:** Classify retinal OCT images into 5 categories using a grayscale image dataset.

**Highlights:**
- Custom CNN model using TensorFlow/Keras
- Data augmentation to address class imbalance
- Training, validation, and testing workflow
- Accuracy/loss curves and confusion matrix analysis


Dataset Source: [MedMNIST - RetinaMNIST](https://medmnist.com/)

---

### 2. ChestMNIST – Chest X-ray Image Classification

**Objective:** Classify chest X-ray images into one dominant diagnostic category (single-label multi-class adaptation of a multi-label dataset).

**Highlights:**
- Label simplification to convert multi-label to single-label classification
- Custom CNN model
- Evaluation using confusion matrix and F1-score
- Exploratory data analysis and visualization of class distributions


Dataset Source: [MedMNIST - ChestMNIST](https://medmnist.com/)

---

## Tools & Libraries

- Python
- TensorFlow / Keras
- NumPy / Pandas
- scikit-learn
- Matplotlib / Seaborn

---

## Summary
This study demonstrated the application of both custom-designed lightweight CNNs and pre-trained deep learning models for multi-class medical image classification using the RetinaMNIST and ChestMNIST datasets. In both datasets, the simple custom CNNs achieved the best performance, highlighting its effectiveness over more complex pre-trained models. The experimental results showed that conventional CNNs, even when enhanced with data augmentation and hyperparameter optimization, faced limitations in accurately classifying low-resolution RetinaMNIST images. For the ChestMNIST dataset, classification performance was impacted by class imbalance, and dataset’s multi-label nature. Reformulating the dataset into a single-label task simplified training but likely reduced diagnostic accuracy by discarding additional clinical information. While pre-trained models were explored for the ChestMNIST, they could not be fully trained within the available computational resources. Hence, custom CNNs offered a practical alternative, achieving comparable performance with significantly reduced training time.

These findings highlight the need for dataset-specific modeling strategies. While pre-trained models offer strong generalization capabilities in many domains, lightweight CNNs remain equally effective with simple light-weight datasets. Future work may consider reintroducing multi-label learning frameworks to better align with the original ChestMNIST label structure, further fine-tuning of pre-trained models and the development of deeper custom CNN architectures.






