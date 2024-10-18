
# Soil Type Classification

## Overview
Soil type classification is pivotal for agricultural decision-making, guiding farmers in optimal crop selection and fertilizer application. Understanding soil characteristics ensures tailored agricultural practices, maximizing crop yield and minimizing environmental impact. Accurate classification enables precision farming, facilitating data-driven decisions for irrigation, nutrient management, and crop planning. This not only enhances agricultural productivity but also promotes sustainable practices, conserving resources and mitigating potential risks. In essence, soil type classification serves as a fundamental tool to empower farmers with actionable insights, fostering efficient and sustainable agriculture practices.

## Dataset Metadata

The dataset comprises a total of 2067 images, each belonging to one of the following 8 classes:

1. Chalky Soil
2. Mary Soil
3. Sand
4. Slit Soil
5. Alluvial Soil
6. Black Soil
7. Clay Soil
8. Red Soil

## Dataset Augmentation

The dataset augmentation process involved the following parameters:

- Rescale: 1./255
- Rotation Range: 20 degrees
- Width Shift Range: 0.2
- Height Shift Range: 0.2
- Zoom Range: 0.2
- Horizontal Flip: True
- Vertical Flip: True
- Fill Mode: Nearest

## Dataset Link
You can access our augmented dataset from [here](https://drive.google.com/drive/folders/1AsCuS6oTudEfhIm3wrECaooHfXckEMw8?usp=sharing)
## Models

We have experimented with both Convolutional Neural Networks (CNNs) including custom architectures and pretrained models, as well as traditional machine-learning models.

## Performance Metrics

The models were evaluated using a test set of 418 images, and the performance metrics are recorded in the following table:

| Model        | Epochs | Loss   | Accuracy   | Precision | Recall  |
|--------------|--------|--------|------------|-----------|---------|
| DenseNet121  | 65     | 0.1263 | 0.9569     | 0.9500    | 0.9476  |
| ResNet50     | 50     | 0.2887 | 0.8947     | 0.8688    | 0.8666  |
| VGG16        | 50     | 0.4702 | 0.8349     | 0.7938    | 0.7772  |
| InceptionV3  | 50     | 0.3635 | 0.8851     | 0.8462    | 0.8602  |

## Acknowledgments

- Created by Anindya Mitra, Sayan Mukherjee and Nandana Mukherjee
