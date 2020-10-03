# CGIAR-Wheat-Growth-Stage-Challenge-by-CGIAR-Platform-for-Big-Data-in-Agriculture
Automates a part of a data processing pipeline by  estimating the growth stage of a wheat crop based on an image sent in by the farmer. The images are automatically cropped to show a section of the field. The model takes in an image and output a prediction for the growth stage of the wheat shown, on a scale from 1 (crop just showing) to 7 (mature crop).


# Summary of Approach
Create an ensemble from a library of diverse models with different architectures and augmentations. All models are pretrained models and they are fine-tuned on the dataset. Made use of Google Colab GPU.


# Model Architecture

The following architecturs are included in the library of models:

1. Resnet
2. Vgg16_bn
3. Densenet

# Data Augmentations
The following augmentations are included:

1. Rotation
2. Random cropping and resizing
3. Horizontal flipping
4. Wrapping
5. Brightness augmentation
6. Zoom

# Common Configuration
The following configurations is applied:

1. Cyclic Learning
2. FP16 precision

