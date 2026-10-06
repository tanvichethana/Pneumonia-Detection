# Pneumonia Detection from Chest X-ray Images

This project uses deep learning to classify chest X-ray images into two classes:

- NORMAL
- PNEUMONIA

Two models were developed and compared:

1. Basic CNN
2. MobileNetV2 Transfer Learning

## Dataset

A chest X-ray dataset containing NORMAL and PNEUMONIA images was used.

The images were resized to 150 × 150 pixels for training and testing.

## Models

### 1. Basic CNN

A convolutional neural network was created using:

- Conv2D layers
- MaxPooling2D layers
- Flatten layer
- Dense layers
- Sigmoid output for binary classification

### 2. MobileNetV2

MobileNetV2 was used as a transfer learning model with ImageNet weights.

The base MobileNetV2 layers were frozen and additional classification layers were added for pneumonia detection.

## Results

| Model | Test Accuracy |
|---|---:|
| Basic CNN | 74.52% |
| MobileNetV2 | 72.28% |

In this experiment, the Basic CNN achieved slightly higher test accuracy than MobileNetV2.

## Result

The test accuracy comparison is shown in:

`download (3).png`

## Files

- `Pneumonia.ipynb` — Google Colab notebook containing the complete project
- `download (3).png` — CNN vs MobileNetV2 test accuracy comparison

## Conclusion

Both models were able to perform binary classification of chest X-ray images.

In this experiment, the Basic CNN achieved **74.52%** test accuracy, while MobileNetV2 achieved **72.28%** test accuracy.

The results show that transfer learning does not always outperform a simple CNN for every dataset and experiment.

## Disclaimer

This project is for educational purposes only. The model predictions should not be used as a medical diagnosis.
