# Brain Tumor Segmentation using U-Net

This project focuses on segmenting brain tumors from MRI images using a U-Net model. The dataset includes 3 different MRI scans/views of the brain along with a ground truth segmented image, which serves as the target for our segmentation task.

## Project Overview

The goal of this project is to segment brain tumors from MRI scans using an advanced deep learning approach (U-Net). The process involves several preprocessing steps to prepare the data, followed by training and evaluation of the model's performance using the DICE score, which measures the overlap between the predicted segmentation and the ground truth.

## Dataset Description
The dataset used for this project is the BraTS (Brain Tumor Segmentation) dataset, available on [Kaggle](https://www.kaggle.com/datasets/awsaf49/brats2020-training-data). The dataset includes various MRI modalities, allowing for comprehensive analysis of brain tumors.

The dataset consists of:
- 3 different MRI scans/views of the brain.
- **MRI Modalities**:
  - T1-weighted
  - T2-weighted
  - Fluid-attenuated inversion recovery (FLAIR)
- Ground truth segmented images highlighting the tumor.
- **Image Dimensions**: 240×240×155 pixels

### Model
The segmentation task was performed using the **U-Net** model, which is particularly well-suited for image segmentation tasks due to its encoder-decoder architecture and skip connections. This model is ideal for medical image analysis, where precise pixel-level segmentation is required.

## Model Architecture
- **Encoding Layer**: Extracts features from the input image.
- **Decoding Layer**: Upsamples feature maps and generates the segmentation mask.
- **Skip Connections**: Captures fine-grained spatial details by connecting the encoding and decoding paths.
- **Fully Convolutional Layer**: Processes images of any size and produces segmentation masks of the same size.

### Evaluation
The performance of the model was evaluated using the **DICE score**, which measures the overlap between the predicted segmentation and the ground truth segmentation. A higher DICE score indicates better performance, with a score of 1.0 representing a perfect overlap.

## Kaggle Notebook

You can view the complete code implementation and analysis in my Kaggle notebook:  
[Kaggle Notebook Link](https://www.kaggle.com/code/varshithpsingh/brain-tumor-image-segmentation)
