# ImageClassification

### Overview

This project investigates the efficacy of various machine learning techniques to automatically classify skin lesions, distinguishing between melanoma and nevi. By utilizing a subset of the 2018 ISIC Challenge dataset, the aim is to enhance classification accuracy through advanced techniques such as normalization, data augmentation, and transfer learning.

### Methodology

The project employs Convolutional Neural Networks (CNNs) to analyze skin lesion images. The approach includes:

* Normalization: Various normalization techniques were applied to prepare the data for training.
* Data Augmentation: Random flipping and grayscaling transformations were used to increase the diversity of the training dataset and improve model robustness.
* Transfer Learning: Leveraging pre-trained models like VGG16 for improved feature extraction and classification performance.

### Model Performance

The following table summarizes the performance of different models employed during the study:

| Model Number                          | Normalization | Transformation                          | Loss    | Validation Accuracy |
|---------------------------------------|---------------|-----------------------------------------|---------|---------------------|
| 1. (CNN)                              | None          | None                                    | 0.5221  | 76.58%              |
| 2. (CNN)                              | Batch         | Random flipping                         | 0.4239  | 75.23%              |
| 3. (CNN)                              | Batch         | Random flipping, Random grayscaling     | 0.4775  | 78.04%              |
| 4. (VGG16 Transfer Learning)          | Batch         | Random flipping, Random grayscaling     | 0.3581  | 83.71%              |

