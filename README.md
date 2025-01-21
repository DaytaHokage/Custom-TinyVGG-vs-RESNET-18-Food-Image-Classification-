# Custom-TinyVGG-vs-RESNET-18-Food-Image-Classification-

This repository contains the FoodVision project, where I developed an image classification system to differentiate between three popular food categories: **pizza**, **steak**, and **sushi**. The project aimed to explore the potential of lightweight custom models compared to pre-trained architectures.

## Overview

FoodVision showcases the development and evaluation of two models:

1. **Custom TinyVGG**: A lightweight convolutional neural network built from scratch for efficient image classification.
2. **ResNet-18**: A widely used pre-trained deep learning model.

Both models were trained on a dataset of **1,007 images**, with the goal of achieving high classification accuracy while balancing computational efficiency.

## Key Features

- **Custom TinyVGG**:
  - Achieved **87% test accuracy**.
  - Lightweight design suitable for applications requiring small model sizes.
- **ResNet-18**:
  - Achieved **92% test accuracy**.
  - Leveraged transfer learning to optimize performance.
- **Data Augmentation**:
  - Techniques such as cropping, zooming, and color adjustments were used to improve model generalization.
- **Model Insights**:
  - Grad-CAM visualizations to understand model focus.
  - LIME explanations for feature validation.
- **Deployment**:
  - The final model is deployed on **Hugging Face Spaces**, allowing real-time image classification through a user-friendly interface.

## Project Motivation

The primary goal was to determine whether a custom model like TinyVGG could achieve comparable accuracy to ResNet-18 while significantly reducing model size. This has implications for real-world applications, such as:
- **Restaurant menu identification**.
- **Dietary tracking tools**.
- **Social media food recognition**.

## Results

| Model       | Test Accuracy | Remarks                  |
|-------------|---------------|--------------------------|
| TinyVGG     | 87%           | Lightweight, efficient   |
| ResNet-18   | 92%           | Higher accuracy, larger size |

Grad-CAM and LIME visualizations were used to interpret model predictions and understand their focus during classification tasks.

## Methodology

1. **Data Collection**: 
   - The dataset consisted of 1,007 images divided into three categories: pizza, steak, and sushi.
2. **Model Design**:
   - TinyVGG was built from scratch with a focus on simplicity and efficiency.
   - ResNet-18 utilized transfer learning for optimal performance.
3. **Training**:
   - Both models were trained on the dataset with appropriate data augmentation techniques to improve robustness.
4. **Evaluation**:
   - Performance metrics were computed, and interpretability tools were applied.

## Improvements and Limitations

### Improvements
- Incorporating more diverse datasets for better generalization.
- Optimizing the TinyVGG architecture to close the accuracy gap further.

### Limitations
- Limited dataset size, which may affect the generalizability of the models.
- TinyVGG achieved slightly lower accuracy compared to ResNet-18.

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/FoodVision.git
   cd FoodVision
   ```
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the training script or deploy the model:
   ```bash
   python train.py
   ```
4. Access the deployed app via Hugging Face Spaces (link to be provided).

## Acknowledgments

- **Mentor**: Mark Shepherd
- **Faculty Advisor**: Professor Bill Franks
- **Institution**: Kennesaw State University

## License

This project is open-source and available under the [MIT License](LICENSE).

## Contact

For questions or collaboration opportunities, feel free to reach out via [email/LinkedIn].
