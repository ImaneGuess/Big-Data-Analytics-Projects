# Description
This project focuses on leveraging deep learning for the automated classification of tomato leaf diseases, critical for enhancing agricultural productivity and reducing losses. The system uses Vision Transformers (ViT), a state-of-the-art model in image classification, to analyze leaf images and identify specific diseases affecting tomato plants.

The project involves a dataset of tomato leaf images categorized by disease type. By training and fine-tuning a pre-trained ViT model, we aim to achieve high accuracy in disease detection, offering farmers a reliable tool for early diagnosis. The workflow includes dataset preparation, training a custom ViT model, validating its performance, and testing on unseen images. The classification results include metrics such as precision, recall, and F1-score.

## Workflow
### Dataset Preparation:
Load, unzip, and organize the dataset into training, validation, and testing splits.
Apply transformations such as resizing and normalization.

### Model Training:
Load a pre-trained ViT model.
Fine-tune the model on the training dataset for tomato leaf disease classification.
Use Cross-Entropy Loss and Adam optimizer with a learning rate scheduler.

### Evaluation:
Validate the model's accuracy on unseen validation data.
Test the model and generate a classification report, confusion matrix, and visualization.

### Results:
Achieved a validation accuracy of ~99% and precise classification metrics for all categories.
Provides an easy-to-use framework for real-world application in agriculture.

# Technology Stack
1. Programming Language:
Python: Used for dataset handling, model training, and evaluation.
2. Frameworks and Libraries:
PyTorch: For deep learning model implementation and training.
Hugging Face Transformers: To load and fine-tune the Vision Transformer (ViT) model.
TorchVision: For dataset handling and image transformation.
scikit-learn: For generating classification reports and confusion matrices.
Matplotlib & Seaborn: For visualizing results (e.g., confusion matrices).
3. Dataset:
Tomato Leaf Dataset: Images of healthy and diseased tomato leaves classified into categories such as Bacterial Spot, Early Blight, Late Blight, Leaf Mold, etc.
4. Tools and Platforms:
Google Colab: For accessible cloud-based GPU training.
CUDA: Accelerates model training using GPU.
5. Pre-trained Model:
ViT (Vision Transformer): Pre-trained on ImageNet, then fine-tuned for the tomato leaf dataset.
6. File Management:
Google Drive: For storing and accessing the dataset.
shutil & zipfile: For managing and extracting data files.
