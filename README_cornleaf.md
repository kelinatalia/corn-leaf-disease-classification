# Corn Leaf Disease Classification

**Individual Project**

## Overview
Built a deep learning model to classify corn leaf images into four categories: Blight, Common Rust, Gray Leaf Spot, and Healthy. The project progresses from a baseline CNN to a fine-tuned transfer learning model, with a thorough exploratory data analysis to understand image quality and consistency before modeling.

## What I Did
- Performed exploratory data analysis on image dimensions, color distribution, brightness, rotation, and feature blockage to assess dataset quality and consistency.
- Built a baseline model by manually implementing the AlexNet architecture.
- Improved on the baseline using transfer learning with MobileNetV2.
- Fine-tuned the MobileNetV2 model with a lower learning rate and extended training to further boost performance, especially on harder-to-distinguish classes.

## Results
| Model | Accuracy | Macro F1 |
|---|---|---|
| Baseline (AlexNet) | 0.89 | 0.87 |
| MobileNetV2 (transfer learning) | 0.93 | 0.92 |
| MobileNetV2 (fine-tuned) | 0.95 | 0.94 |

Fine-tuning gave the biggest improvement on the hardest class to classify, Gray Leaf Spot, raising its F1-score from 0.74 to 0.86.

## Tech Stack
Python, TensorFlow/Keras, MobileNetV2, NumPy, Matplotlib, OpenCV

## What I Learned
Learned how to systematically validate image dataset quality before modeling, and gained hands-on experience comparing a manually built CNN architecture against transfer learning, including the impact of fine-tuning on class-level performance.
