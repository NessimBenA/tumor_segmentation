# Automatic MRI Tumor Segmentation with SAM-ViT

This notebook demonstrates how to use SAM-ViT for automatic tumor segmentation in MRI images. The dataset used is the LGG MRI Segmentation dataset from Kaggle, which consists of brain MRI images with corresponding ground truth masks. The segmentation model is SAM-ViT, a state-of-the-art model for automatic segmentation, pretrained on a large-scale dataset. This notebook walks you through the process of downloading the dataset, preparing the data, and using SAM-ViT to generate segmentation masks for MRI images.

## Table of Contents

1. [Setup and Dataset Download](#Setup-and-Dataset-Download)
2. [Data Preparation and Exploration](#Data-Preparation-and-Exploration)
3. [Visualizing MRI Images and Masks](#Visualizing-MRI-Images-and-Masks)
4. [Loading and Using SAM-ViT](#Loading-and-Using-SAM-ViT)
5. [Generating Segmentation Masks](#Generating-Segmentation-Masks)
6. [Customizing Mask Generation Parameters](#Customizing-Mask-Generation-Parameters)

### Setup and Dataset Download

This section shows how to install the necessary packages and download the LGG MRI Segmentation dataset from Kaggle.

### Data Preparation and Exploration

The data preparation step includes loading MRI images and their corresponding masks. It also counts the number of images with all-black masks, indicating no tumor present.

### Visualizing MRI Images and Masks

In this section, we visualize examples of MRI images alongside their corresponding ground truth masks.

### Loading and Using SAM-ViT

This part demonstrates how to load the pretrained SAM-ViT model and use it for generating segmentation masks.

### Generating Segmentation Masks

We use the SAM-ViT model to automatically generate segmentation masks for the MRI images. The results are visualized alongside the original images and ground truth masks.

### Customizing Mask Generation Parameters

In this section, we show how to customize the mask generation parameters to improve the quality of the generated masks. The new masks are visualized and compared to the original masks and ground truth masks.

## Usage

To run the notebook, make sure you have the necessary packages installed, including `cv2`, `matplotlib`, `numpy`, and `torch`. You can install these packages using `pip`. Additionally, you will need to download the `sam_vit_h_4b8939.pth` file from the specified URL.

```python
!{sys.executable} -m pip install 'git+https://github.com/facebookresearch/segment-anything.git'
!wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth
```