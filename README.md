# Autism Spectrum Disorder Classification Using Deep Learning Models

This project employs a deep learning model that uses facial images to classify autism spectrum disorder (ASD). VGG16, VGG19, and AlexNet are the models that were trained and evaluated for subtle features that define facial expressions of ASD.

## Publication Details
**Published in**: *International Journal of Medical Toxicology & Legal Medicine*  
**Volume**: 27, No. 2, 2024  
**Pages**: 194-201  
**ISSN**: e-ISSN: 0974-4614, p-ISSN: 0972-0448  
**DOI**: (https://ijmtlm.org)

## Authors
- **A. Sampath Dakshina Murthy** - Associate Professor, Department of ECE, Vignan's Institute of Information Technology, Duvvada, Visakhapatnam, India.  
- **Syamala Rao P.** - Assistant Professor, Department of IT, SRKR Engineering College, Bhimavaram, India.  
- **N. Sirisha** - Department of CSE, MLR Institute of Technology, Hyderabad, Telangana, India.  
- **V. Rajesh, Y. Sudhanshu Varma, S. Tanweer Ahmed, V. Sri Sravan, Kayam Saikumar** - Department of ECE, Koneru Lakshmaiah Educational Foundation, Guntur & Hyderabad, Telangana, India.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architectures](#model-architectures)
- [Preprocessing and Augmentation](#preprocessing-and-augmentation)
- [Training and Evaluation](#training-and-evaluation)
- [Results](#results)
- [Conclusion and Future Work](#conclusion-and-future-work)

## Introduction
Autism Spectrum Disorder (ASD) is a developmental condition characterized by difficulties with interpersonal communication, social interaction, and repetitive behaviors. Early diagnosis is essential for effective intervention, but current diagnostic methods can be subjective and resource-intensive. This project uses a deep learning model to analyze facial images and automate ASD detection.

## Dataset
The dataset includes images of faces labeled as "autistic" or "non-autistic." VGG16, VGG19, and AlexNet models are used, with images pre-processed and resized to match the required input dimensions.

## Model Architectures
- **VGG16**: A deep convolutional neural network with 16 layers known for its accuracy in image classification tasks.
- **VGG19**: An extended version of VGG16 with 19 layers, offering additional depth.
- **AlexNet**: A CNN architecture with 8 layers, optimized for faster training but less accurate in this application.

## Preprocessing and Augmentation
- **Normalization**: Scales pixel values to a [0, 1] range.
- **Augmentation**: Enhances data diversity and reduces overfitting through transformations such as rotation, zoom, and flips.

## Training and Evaluation
Models were trained using categorical cross-entropy loss and tested on a separate test dataset. Performance metrics include accuracy, precision, recall, and F1-score, which help measure the effectiveness of each model.

## Results

| Model     | Accuracy | Precision (ASD) | Recall (ASD) | F1-Score (ASD) |
|-----------|----------|-----------------|--------------|----------------|
| VGG16     | 72%      | 82%             | 57%          | 67%            |
| AlexNet   | 50%      | 50%             | 50%          | 50%            |
| VGG19     | 75%      | 67%             | 73%          | 70%            |

**Observations**:
- VGG19 achieved the highest accuracy (75%) and balanced performance across metrics.
- VGG16 demonstrated good recall and precision for ASD classification.
- AlexNet performed similarly to random guessing, suggesting limited suitability for this task.

## Conclusion and Future Work
This project demonstrates the potential of deep learning in automating ASD detection through non-invasive facial analysis. Future improvements may include:
- Integrating multi-modal data such as MRI or EEG.
- Applying advanced explainability techniques.
- Testing on larger, diverse datasets to improve model robustness.
