**🦴 Wrist Fracture Detection using DETR**


**🚀 Project Overview**

This project implements a Deep Learning object detection system using the DETR (DEtection TRansformer) architecture to identify wrist fractures in X-ray images. Leveraging the power of transformers, DETR enables end-to-end object detection with remarkable performance and less post-processing.

The model achieves an IoU of 0.81, demonstrating its effectiveness in accurately detecting fracture regions.

**🎯 Objective**

To build a robust model capable of:

Automatically detecting fractures in wrist X-rays

Outputting annotated images with bounding boxes

Assisting radiologists in diagnostics by reducing human error

**📊 Dataset Summary**

Original images: 20,000 wrist X-ray scans

Filtered: Retained only fracture class images (~9,000)

Augmentation: Rotation applied (±7 degrees)

Final training set size: ~20,000 images post augmentation

Split:

Training: 15,000+ images

Validation: 1,500+ images

Testing: 700 images

**⚙️ Tools & Libraries**

DETR (Facebook AI Research)

PyTorch

Torchvision

Albumentations (for augmentations)

Matplotlib (for visualizations)

Roboflow (used for dataset augmentation and preprocessing)

**🧪 Model Training**

Model architecture: DETR (ResNet50 backbone)

Input: Preprocessed and augmented X-ray images

Loss Function: Combination of Hungarian matching + bounding box loss

Optimizer: AdamW

Epochs: Configurable (best model reached at ~30 epochs)

**📈 Results**

Intersection over Union (IoU): 0.81

Precision: High for fracture class

Recall: Strong generalization across validation and test set

Annotated test images clearly highlight fracture regions, confirming the model's diagnostic utility.

